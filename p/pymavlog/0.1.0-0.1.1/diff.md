# Comparing `tmp/pymavlog-0.1.0.tar.gz` & `tmp/pymavlog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymavlog-0.1.0.tar", max compression
+gzip compressed data, was "pymavlog-0.1.1.tar", max compression
```

## Comparing `pymavlog-0.1.0.tar` & `pymavlog-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1495 2023-04-13 00:49:49.047643 pymavlog-0.1.0/README.md
--rw-r--r--   0        0        0      176 2023-04-12 18:52:07.896628 pymavlog-0.1.0/pymavlog/__init__.py
--rw-r--r--   0        0        0     5914 2023-04-12 20:46:30.811107 pymavlog-0.1.0/pymavlog/core.py
--rw-r--r--   0        0        0      137 2023-04-12 18:59:31.372393 pymavlog-0.1.0/pymavlog/errors.py
--rw-r--r--   0        0        0      121 2023-04-12 17:15:29.013966 pymavlog-0.1.0/pymavlog/helpers.py
--rw-r--r--   0        0        0      846 2023-04-13 01:07:52.704411 pymavlog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2612 1970-01-01 00:00:00.000000 pymavlog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-18 18:08:48.698553 pymavlog-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1651 2023-04-18 18:08:48.698553 pymavlog-0.1.1/README.md
+-rw-r--r--   0        0        0      176 2023-04-18 18:08:48.698553 pymavlog-0.1.1/pymavlog/__init__.py
+-rw-r--r--   0        0        0     5914 2023-04-18 18:08:48.698553 pymavlog-0.1.1/pymavlog/core.py
+-rw-r--r--   0        0        0      137 2023-04-18 18:08:48.698553 pymavlog-0.1.1/pymavlog/errors.py
+-rw-r--r--   0        0        0      121 2023-04-18 18:08:48.698553 pymavlog-0.1.1/pymavlog/helpers.py
+-rw-r--r--   0        0        0     1072 2023-04-18 18:08:57.818637 pymavlog-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 pymavlog-0.1.1/PKG-INFO
```

### Comparing `pymavlog-0.1.0/README.md` & `pymavlog-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [![codecov](https://codecov.io/gh/rmargar/pymavlog/branch/main/graph/badge.svg?token=0APOFRD0BT)](https://codecov.io/gh/rmargar/pymavlog)
+![test](https://github.com/rmargar/pymavlog/actions/workflows/test.yaml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/pymavlog.svg)](https://badge.fury.io/py/pymavlog)
 
 # pyulog
 
-A lightweight python to parse log files from ArduPilot vehicles based on the [MavLink](https://mavlink.io/) protocol. It is built on top of [pymavlink](https://github.com/ArduPilot/pymavlink) and uses [NumPy](https://numpy.org/) under the hood to vectorize messages.
+A lightweight python library to parse log files from ArduPilot vehicles based on the [MavLink](https://mavlink.io/) protocol. It is built on top of [pymavlink](https://github.com/ArduPilot/pymavlink) and uses [NumPy](https://numpy.org/) under the hood to vectorize messages.
 
 ## Installation
 
 Installation with pip:
 
 ```bash
 pip install pyulog
 ```
 
 or via Poetry
 
-Installation from source:
-
 ```bash
 poetry add pyulog
 ```
 
 ## Development
 
 Install the package in editable mode:
```

### Comparing `pymavlog-0.1.0/pymavlog/core.py` & `pymavlog-0.1.1/pymavlog/core.py`

 * *Files identical despite different names*

### Comparing `pymavlog-0.1.0/PKG-INFO` & `pymavlog-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymavlog
-Version: 0.1.0
+Version: 0.1.1
 Summary: A lightweight python library to parse MavLink log files
 Home-page: https://github.com/rmargar/pymavlog
 License: MIT
 Author: Ricardo Martinez
 Author-email: rik@rmargar.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 1 - Planning
@@ -23,31 +23,31 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: numpy (>=1.21,<2.0)
 Requires-Dist: pymavlink (>=2.4,<3.0)
 Project-URL: Repository, https://github.com/rmargar/pymavlog
 Description-Content-Type: text/markdown
 
 [![codecov](https://codecov.io/gh/rmargar/pymavlog/branch/main/graph/badge.svg?token=0APOFRD0BT)](https://codecov.io/gh/rmargar/pymavlog)
+![test](https://github.com/rmargar/pymavlog/actions/workflows/test.yaml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/pymavlog.svg)](https://badge.fury.io/py/pymavlog)
 
 # pyulog
 
-A lightweight python to parse log files from ArduPilot vehicles based on the [MavLink](https://mavlink.io/) protocol. It is built on top of [pymavlink](https://github.com/ArduPilot/pymavlink) and uses [NumPy](https://numpy.org/) under the hood to vectorize messages.
+A lightweight python library to parse log files from ArduPilot vehicles based on the [MavLink](https://mavlink.io/) protocol. It is built on top of [pymavlink](https://github.com/ArduPilot/pymavlink) and uses [NumPy](https://numpy.org/) under the hood to vectorize messages.
 
 ## Installation
 
 Installation with pip:
 
 ```bash
 pip install pyulog
 ```
 
 or via Poetry
 
-Installation from source:
-
 ```bash
 poetry add pyulog
 ```
 
 ## Development
 
 Install the package in editable mode:
```

