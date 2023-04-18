# Comparing `tmp/pysetns-0.2.3.tar.gz` & `tmp/pysetns-0.2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysetns-0.2.3.tar", last modified: Tue Apr 18 15:52:26 2023, max compression
+gzip compressed data, was "pysetns-0.2.3.1.tar", last modified: Tue Apr 18 16:18:54 2023, max compression
```

## Comparing `pysetns-0.2.3.tar` & `pysetns-0.2.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:52:26.440292 pysetns-0.2.3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-04-18 15:52:15.000000 pysetns-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-18 15:52:26.440292 pysetns-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-18 15:52:15.000000 pysetns-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:52:26.440292 pysetns-0.2.3/pysetns/
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-04-18 15:52:15.000000 pysetns-0.2.3/pysetns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:52:26.440292 pysetns-0.2.3/pysetns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-18 15:52:26.000000 pysetns-0.2.3/pysetns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-18 15:52:26.000000 pysetns-0.2.3/pysetns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:52:26.000000 pysetns-0.2.3/pysetns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 15:52:26.000000 pysetns-0.2.3/pysetns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:52:26.440292 pysetns-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-18 15:52:15.000000 pysetns-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:52:26.440292 pysetns-0.2.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-18 15:52:15.000000 pysetns-0.2.3/src/ext.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:18:54.611884 pysetns-0.2.3.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-04-18 16:18:40.000000 pysetns-0.2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-18 16:18:54.611884 pysetns-0.2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-18 16:18:40.000000 pysetns-0.2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:18:54.611884 pysetns-0.2.3.1/pysetns/
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-04-18 16:18:40.000000 pysetns-0.2.3.1/pysetns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:18:54.611884 pysetns-0.2.3.1/pysetns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-18 16:18:54.000000 pysetns-0.2.3.1/pysetns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-18 16:18:54.000000 pysetns-0.2.3.1/pysetns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:18:54.000000 pysetns-0.2.3.1/pysetns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 16:18:54.000000 pysetns-0.2.3.1/pysetns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:18:54.611884 pysetns-0.2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-18 16:18:40.000000 pysetns-0.2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:18:54.611884 pysetns-0.2.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-18 16:18:40.000000 pysetns-0.2.3.1/src/ext.c
```

### Comparing `pysetns-0.2.3/LICENSE` & `pysetns-0.2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysetns-0.2.3/PKG-INFO` & `pysetns-0.2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pysetns
-Version: 0.2.3
+Version: 0.2.3.1
 Summary: Python wrapper for setns Linux syscall.
 Home-page: https://github.com/baskiton/pysetns
 Author: Alexander Baskikh
 Author-email: baskiton@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/baskiton/pysetns
 Project-URL: Bug Tracker, https://github.com/baskiton/pysetns/issues
 Keywords: linux kernel namespace setns
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: System :: Operating System Kernels :: Linux
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysetns
 [![pypi](https://img.shields.io/pypi/v/pysetns?logo=python&logoColor=white)](https://pypi.org/project/pysetns/)
 [![downloads](https://img.shields.io/pypi/dm/pysetns?logo=python&logoColor=white)](https://pypi.org/project/pysetns/)
 [![license](https://img.shields.io/pypi/l/pysetns?logo=open-source-initiative&logoColor=white)](https://github.com/baskiton/pysetns/blob/main/LICENSE)
@@ -31,15 +31,15 @@
 
 To detail see the [documentation][documentation]
 
 ### IMPORTANT!
 `setns` required execution from **ROOT**!
 
 ## Requirements
- * Python 3.6+
+ * Python 3.8+
 
 ## Installing
 ### Using PIP
 ```sh
 $ pip install pysetns
 ```
```

### Comparing `pysetns-0.2.3/README.md` & `pysetns-0.2.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 To detail see the [documentation][documentation]
 
 ### IMPORTANT!
 `setns` required execution from **ROOT**!
 
 ## Requirements
- * Python 3.6+
+ * Python 3.8+
 
 ## Installing
 ### Using PIP
 ```sh
 $ pip install pysetns
 ```
```

### Comparing `pysetns-0.2.3/pysetns/__init__.py` & `pysetns-0.2.3.1/pysetns/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import errno
 import os
 
 from typing import Callable, Union, Iterable
 
 from . import ext
 
-__version__ = '0.2.3'
+__version__ = '0.2.3.1'
 
 NS_TIME = ext.CLONE_NEWTIME     # time namespace (since Linux 5.8)
 NS_MNT = ext.CLONE_NEWNS        # mount namespace group (since Linux 3.8)
 NS_CGROUP = ext.CLONE_NEWCGROUP # cgroup namespace (since Linux 4.6)
 NS_UTS = ext.CLONE_NEWUTS       # utsname namespace (since Linux 3.0)
 NS_IPC = ext.CLONE_NEWIPC       # ipc namespace (since Linux 3.0)
 NS_USER = ext.CLONE_NEWUSER     # user namespace (since Linux 3.8)
```

### Comparing `pysetns-0.2.3/pysetns.egg-info/PKG-INFO` & `pysetns-0.2.3.1/pysetns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pysetns
-Version: 0.2.3
+Version: 0.2.3.1
 Summary: Python wrapper for setns Linux syscall.
 Home-page: https://github.com/baskiton/pysetns
 Author: Alexander Baskikh
 Author-email: baskiton@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/baskiton/pysetns
 Project-URL: Bug Tracker, https://github.com/baskiton/pysetns/issues
 Keywords: linux kernel namespace setns
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: System :: Operating System Kernels :: Linux
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysetns
 [![pypi](https://img.shields.io/pypi/v/pysetns?logo=python&logoColor=white)](https://pypi.org/project/pysetns/)
 [![downloads](https://img.shields.io/pypi/dm/pysetns?logo=python&logoColor=white)](https://pypi.org/project/pysetns/)
 [![license](https://img.shields.io/pypi/l/pysetns?logo=open-source-initiative&logoColor=white)](https://github.com/baskiton/pysetns/blob/main/LICENSE)
@@ -31,15 +31,15 @@
 
 To detail see the [documentation][documentation]
 
 ### IMPORTANT!
 `setns` required execution from **ROOT**!
 
 ## Requirements
- * Python 3.6+
+ * Python 3.8+
 
 ## Installing
 ### Using PIP
 ```sh
 $ pip install pysetns
 ```
```

### Comparing `pysetns-0.2.3/setup.py` & `pysetns-0.2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pathlib
 import sys
 
 from setuptools import find_packages, setup, Extension
 
 
-MINIMAL_PY_VERSION = (3, 6)
+MINIMAL_PY_VERSION = (3, 8)
 if sys.version_info < MINIMAL_PY_VERSION:
     raise RuntimeError('This app works only with Python {}+'.format('.'.join(map(str, MINIMAL_PY_VERSION))))
 
 
 def get_file(rel_path):
     return (pathlib.Path(__file__).parent / rel_path).read_text('utf-8')
 
@@ -47,12 +47,12 @@
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Operating System :: POSIX :: Linux',
         'Topic :: System :: Operating System Kernels :: Linux',
     ],
     keywords='linux kernel namespace setns',
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     package_data={
         '': ['examples/*']
     }
 )
```

### Comparing `pysetns-0.2.3/src/ext.c` & `pysetns-0.2.3.1/src/ext.c`

 * *Files identical despite different names*

