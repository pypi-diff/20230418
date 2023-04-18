# Comparing `tmp/pyees-1.1.7.tar.gz` & `tmp/pyees-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.1.7.tar", last modified: Tue Apr 18 11:07:23 2023, max compression
+gzip compressed data, was "pyees-1.1.8.tar", last modified: Tue Apr 18 11:09:29 2023, max compression
```

## Comparing `pyees-1.1.7.tar` & `pyees-1.1.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 11:07:23.800359 pyees-1.1.7/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0      616 2023-04-18 11:07:23.815984 pyees-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 11:07:23.396661 pyees-1.1.7/pyees/
--rw-rw-rw-   0        0        0      619 2023-03-30 05:48:48.000000 pyees-1.1.7/pyees/__init__.py
--rw-rw-rw-   0        0        0    15688 2023-03-11 13:10:44.000000 pyees-1.1.7/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.1.7/pyees/profilePyees.py
--rw-rw-rw-   0        0        0     8922 2023-04-03 12:12:15.000000 pyees-1.1.7/pyees/prop.py
--rw-rw-rw-   0        0        0    14054 2023-04-18 11:06:16.000000 pyees-1.1.7/pyees/readData.py
--rw-rw-rw-   0        0        0    10138 2023-04-05 08:09:23.000000 pyees-1.1.7/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.1.7/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     3249 2023-03-13 12:35:20.000000 pyees-1.1.7/pyees/testFit.py
--rw-rw-rw-   0        0        0     1671 2023-03-07 14:26:33.000000 pyees-1.1.7/pyees/testProp.py
--rw-rw-rw-   0        0        0     1059 2023-04-16 08:44:33.000000 pyees-1.1.7/pyees/testPyees.py
--rw-rw-rw-   0        0        0    11884 2023-04-16 08:11:52.000000 pyees-1.1.7/pyees/testReadData.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.1.7/pyees/testSolve.py
--rw-rw-rw-   0        0        0     8958 2023-04-15 19:26:44.000000 pyees-1.1.7/pyees/testUnit.py
--rw-rw-rw-   0        0        0    81154 2023-04-14 08:23:21.000000 pyees-1.1.7/pyees/testVariable.py
--rw-rw-rw-   0        0        0    45294 2023-04-15 19:24:42.000000 pyees-1.1.7/pyees/unit.py
--rw-rw-rw-   0        0        0    34872 2023-04-14 08:21:49.000000 pyees-1.1.7/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-04-18 11:07:23.753481 pyees-1.1.7/pyees.egg-info/
--rw-rw-rw-   0        0        0      616 2023-04-18 11:07:21.000000 pyees-1.1.7/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-04-18 11:07:21.000000 pyees-1.1.7/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 11:07:21.000000 pyees-1.1.7/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-18 11:07:21.000000 pyees-1.1.7/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-18 11:07:21.000000 pyees-1.1.7/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-18 11:07:23.847235 pyees-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-04-18 11:06:19.000000 pyees-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:09:29.557144 pyees-1.1.8/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      616 2023-04-18 11:09:29.572770 pyees-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 11:09:29.307133 pyees-1.1.8/pyees/
+-rw-rw-rw-   0        0        0      641 2023-04-18 11:09:16.000000 pyees-1.1.8/pyees/__init__.py
+-rw-rw-rw-   0        0        0    15688 2023-03-11 13:10:44.000000 pyees-1.1.8/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.1.8/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0     8922 2023-04-03 12:12:15.000000 pyees-1.1.8/pyees/prop.py
+-rw-rw-rw-   0        0        0    14054 2023-04-18 11:06:16.000000 pyees-1.1.8/pyees/readData.py
+-rw-rw-rw-   0        0        0    10138 2023-04-05 08:09:23.000000 pyees-1.1.8/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.1.8/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     3249 2023-03-13 12:35:20.000000 pyees-1.1.8/pyees/testFit.py
+-rw-rw-rw-   0        0        0     1671 2023-03-07 14:26:33.000000 pyees-1.1.8/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1059 2023-04-16 08:44:33.000000 pyees-1.1.8/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    11884 2023-04-16 08:11:52.000000 pyees-1.1.8/pyees/testReadData.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.1.8/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     8958 2023-04-15 19:26:44.000000 pyees-1.1.8/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    81154 2023-04-14 08:23:21.000000 pyees-1.1.8/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    45294 2023-04-15 19:24:42.000000 pyees-1.1.8/pyees/unit.py
+-rw-rw-rw-   0        0        0    34872 2023-04-14 08:21:49.000000 pyees-1.1.8/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-04-18 11:09:29.510267 pyees-1.1.8/pyees.egg-info/
+-rw-rw-rw-   0        0        0      616 2023-04-18 11:09:27.000000 pyees-1.1.8/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-04-18 11:09:28.000000 pyees-1.1.8/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 11:09:27.000000 pyees-1.1.8/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-18 11:09:27.000000 pyees-1.1.8/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-18 11:09:27.000000 pyees-1.1.8/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-18 11:09:29.604022 pyees-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2023-04-18 11:09:21.000000 pyees-1.1.8/setup.py
```

### Comparing `pyees-1.1.7/LICENSE.txt` & `pyees-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/PKG-INFO` & `pyees-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.1.7
+Version: 1.1.8
 Summary: EES but for python
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.1.7/README.md` & `pyees-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees/fit.py` & `pyees-1.1.8/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees/profilePyees.py` & `pyees-1.1.8/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees/prop.py` & `pyees-1.1.8/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees/readData.py` & `pyees-1.1.8/pyees/readData.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees/solve.py` & `pyees-1.1.8/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees/stackOverflowODR.py` & `pyees-1.1.8/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees/testFit.py` & `pyees-1.1.8/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees/testProp.py` & `pyees-1.1.8/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees/testPyees.py` & `pyees-1.1.8/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees/testReadData.py` & `pyees-1.1.8/pyees/testReadData.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees/testSolve.py` & `pyees-1.1.8/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees/testUnit.py` & `pyees-1.1.8/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees/testVariable.py` & `pyees-1.1.8/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees/unit.py` & `pyees-1.1.8/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees/variable.py` & `pyees-1.1.8/pyees/variable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.7/pyees.egg-info/PKG-INFO` & `pyees-1.1.8/pyees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.1.7
+Version: 1.1.8
 Summary: EES but for python
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.1.7/setup.py` & `pyees-1.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.1.7',
+    version='1.1.8',
     license='MIT',
     description='EES but for python',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

