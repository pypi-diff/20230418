# Comparing `tmp/fs-mapping-tools-0.1.1.tar.gz` & `tmp/fs-mapping-tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fs-mapping-tools-0.1.1.tar", last modified: Fri Feb 24 02:57:17 2023, max compression
+gzip compressed data, was "fs-mapping-tools-0.2.0.tar", last modified: Tue Apr 18 18:31:07 2023, max compression
```

## Comparing `fs-mapping-tools-0.1.1.tar` & `fs-mapping-tools-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 02:57:17.415165 fs-mapping-tools-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-02-24 02:57:02.000000 fs-mapping-tools-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42023 2023-02-24 02:57:17.415165 fs-mapping-tools-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-24 02:57:02.000000 fs-mapping-tools-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-02-24 02:57:02.000000 fs-mapping-tools-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 02:57:17.415165 fs-mapping-tools-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 02:57:17.411165 fs-mapping-tools-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 02:57:17.415165 fs-mapping-tools-0.1.1/src/fs_mapping_tools/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-24 02:57:02.000000 fs-mapping-tools-0.1.1/src/fs_mapping_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-02-24 02:57:02.000000 fs-mapping-tools-0.1.1/src/fs_mapping_tools/cones.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-02-24 02:57:02.000000 fs-mapping-tools-0.1.1/src/fs_mapping_tools/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 02:57:17.415165 fs-mapping-tools-0.1.1/src/fs_mapping_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42023 2023-02-24 02:57:17.000000 fs-mapping-tools-0.1.1/src/fs_mapping_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-24 02:57:17.000000 fs-mapping-tools-0.1.1/src/fs_mapping_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 02:57:17.000000 fs-mapping-tools-0.1.1/src/fs_mapping_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-24 02:57:17.000000 fs-mapping-tools-0.1.1/src/fs_mapping_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 02:57:17.415165 fs-mapping-tools-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-02-24 02:57:02.000000 fs-mapping-tools-0.1.1/tests/test_cones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:31:07.378189 fs-mapping-tools-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-18 18:31:00.000000 fs-mapping-tools-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42026 2023-04-18 18:31:07.378189 fs-mapping-tools-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-18 18:31:00.000000 fs-mapping-tools-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-18 18:31:00.000000 fs-mapping-tools-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 18:31:07.378189 fs-mapping-tools-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:31:07.378189 fs-mapping-tools-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:31:07.378189 fs-mapping-tools-0.2.0/src/fs_mapping_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-18 18:31:00.000000 fs-mapping-tools-0.2.0/src/fs_mapping_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-18 18:31:00.000000 fs-mapping-tools-0.2.0/src/fs_mapping_tools/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:31:07.378189 fs-mapping-tools-0.2.0/src/fs_mapping_tools/track/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 18:31:00.000000 fs-mapping-tools-0.2.0/src/fs_mapping_tools/track/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14120 2023-04-18 18:31:00.000000 fs-mapping-tools-0.2.0/src/fs_mapping_tools/track/cones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:31:07.378189 fs-mapping-tools-0.2.0/src/fs_mapping_tools/vehicle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 18:31:00.000000 fs-mapping-tools-0.2.0/src/fs_mapping_tools/vehicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-04-18 18:31:00.000000 fs-mapping-tools-0.2.0/src/fs_mapping_tools/vehicle/car.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-04-18 18:31:00.000000 fs-mapping-tools-0.2.0/src/fs_mapping_tools/vehicle/detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:31:07.378189 fs-mapping-tools-0.2.0/src/fs_mapping_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42026 2023-04-18 18:31:07.000000 fs-mapping-tools-0.2.0/src/fs_mapping_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-18 18:31:07.000000 fs-mapping-tools-0.2.0/src/fs_mapping_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:31:07.000000 fs-mapping-tools-0.2.0/src/fs_mapping_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 18:31:07.000000 fs-mapping-tools-0.2.0/src/fs_mapping_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 18:31:07.000000 fs-mapping-tools-0.2.0/src/fs_mapping_tools.egg-info/top_level.txt
```

### Comparing `fs-mapping-tools-0.1.1/LICENSE` & `fs-mapping-tools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fs-mapping-tools-0.1.1/PKG-INFO` & `fs-mapping-tools-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs-mapping-tools
-Version: 0.1.1
+Version: 0.2.0
 Summary: A set of simple utilities for track mapping, designed for Formula Student autonomous events.
 Author-email: Paulo Sanchez <dev.szblzpaulo@gmail.com>
 Maintainer-email: Paulo Sanchez <dev.szblzpaulo@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -670,20 +670,20 @@
 Project-URL: Bug Tracker, https://github.com/erlete/fs-mapping-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Formula Student Mapping Tools
 
 [![Tests status](./reports/badges/tests.svg)](http://htmlpreview.github.io/?https://github.com/erlete/fs-mapping-tools/blob/dev/reports/data/tests/index.html) [![Coverage Status](https://coveralls.io/repos/github/erlete/fs-mapping-tools/badge.svg)](https://coveralls.io/github/erlete/fs-mapping-tools) [![Linter status](./reports/badges/linter.svg)](http://htmlpreview.github.io/?https://github.com/erlete/fs-mapping-tools/blob/dev/reports/data/linter/index.html)
```

### Comparing `fs-mapping-tools-0.1.1/README.md` & `fs-mapping-tools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fs-mapping-tools-0.1.1/pyproject.toml` & `fs-mapping-tools-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 [build-system]
 requires = [
-    "setuptools",
-    "matplotlib>=3.7.0",
-    "numpy>=1.24.2",
-    "bidimensional>=1.9.0"
+    "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fs-mapping-tools"
-version = "0.1.1"
+version = "0.2.0"
 description = "A set of simple utilities for track mapping, designed for Formula Student autonomous events."
 readme = "README.md"
 license = {file = "LICENSE"}
-requires-python = ">=3.8"
+requires-python = ">=3.8.10"
 authors = [
     {name = "Paulo Sanchez", email = "dev.szblzpaulo@gmail.com"}
 ]
 maintainers = [
     {name = "Paulo Sanchez", email = "dev.szblzpaulo@gmail.com"}
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Typing :: Typed"
 ]
+dependencies = [
+    "matplotlib>=3.7.0",
+    "numpy>=1.24.2",
+    "bidimensional>=1.9.0"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/erlete/fs-mapping-tools"
 "Bug Tracker" = "https://github.com/erlete/fs-mapping-tools/issues"
```

### Comparing `fs-mapping-tools-0.1.1/src/fs_mapping_tools/cones.py` & `fs-mapping-tools-0.2.0/src/fs_mapping_tools/track/cones.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from typing import Any, List, Sequence, Union
 
 import matplotlib
 from bidimensional import Coordinate
 from matplotlib import pyplot as plt
 
-from .config import CONES
+from ..config import CONES
 
 
 class Cone:
     """Cone representation class.
 
     This class represents a Formula Student cone. It supports any of the four
     types of cones defined in the FS rules: yellow, orange, orange-big and
@@ -270,15 +270,15 @@
     @property
     def type(self) -> str:
         """Get the type of cones in the array.
 
         Returns:
             str: type of cones in the array.
         """
-        return self.cones[0].type
+        return self.cones[0].type if self.cones else None
 
     def append(self, cone: Cone) -> None:
         """Append a cone to the array.
 
         Args:
             cone (Cone): cone to append to the array.
```

### Comparing `fs-mapping-tools-0.1.1/src/fs_mapping_tools/config.py` & `fs-mapping-tools-0.2.0/src/fs_mapping_tools/config.py`

 * *Files identical despite different names*

### Comparing `fs-mapping-tools-0.1.1/src/fs_mapping_tools.egg-info/PKG-INFO` & `fs-mapping-tools-0.2.0/src/fs_mapping_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fs-mapping-tools
-Version: 0.1.1
+Version: 0.2.0
 Summary: A set of simple utilities for track mapping, designed for Formula Student autonomous events.
 Author-email: Paulo Sanchez <dev.szblzpaulo@gmail.com>
 Maintainer-email: Paulo Sanchez <dev.szblzpaulo@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -670,20 +670,20 @@
 Project-URL: Bug Tracker, https://github.com/erlete/fs-mapping-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.8.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Formula Student Mapping Tools
 
 [![Tests status](./reports/badges/tests.svg)](http://htmlpreview.github.io/?https://github.com/erlete/fs-mapping-tools/blob/dev/reports/data/tests/index.html) [![Coverage Status](https://coveralls.io/repos/github/erlete/fs-mapping-tools/badge.svg)](https://coveralls.io/github/erlete/fs-mapping-tools) [![Linter status](./reports/badges/linter.svg)](http://htmlpreview.github.io/?https://github.com/erlete/fs-mapping-tools/blob/dev/reports/data/linter/index.html)
```

