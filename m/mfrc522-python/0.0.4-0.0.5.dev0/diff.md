# Comparing `tmp/mfrc522-python-0.0.4.tar.gz` & `tmp/mfrc522-python-0.0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfrc522-python-0.0.4.tar", last modified: Mon Apr 17 09:47:47 2023, max compression
+gzip compressed data, was "mfrc522-python-0.0.5.dev0.tar", last modified: Tue Apr 18 16:33:47 2023, max compression
```

## Comparing `mfrc522-python-0.0.4.tar` & `mfrc522-python-0.0.5.dev0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 09:47:47.744548 mfrc522-python-0.0.4/
--rw-rw-rw-   0        0        0    35823 2023-04-15 05:57:40.000000 mfrc522-python-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3013 2023-04-17 09:47:47.744548 mfrc522-python-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2433 2023-04-17 09:44:23.000000 mfrc522-python-0.0.4/README.md
--rw-rw-rw-   0        0        0      660 2023-04-17 09:46:51.000000 mfrc522-python-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 09:47:47.744548 mfrc522-python-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 09:47:47.712512 mfrc522-python-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 09:47:47.720509 mfrc522-python-0.0.4/src/mfrc522/
--rw-rw-rw-   0        0        0    22655 2023-04-17 09:42:23.000000 mfrc522-python-0.0.4/src/mfrc522/MFRC522.py
--rw-rw-rw-   0        0        0       50 2023-04-15 05:57:40.000000 mfrc522-python-0.0.4/src/mfrc522/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 09:47:47.744548 mfrc522-python-0.0.4/src/mfrc522_python.egg-info/
--rw-rw-rw-   0        0        0     3013 2023-04-17 09:47:47.000000 mfrc522-python-0.0.4/src/mfrc522_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-04-17 09:47:47.000000 mfrc522-python-0.0.4/src/mfrc522_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 09:47:47.000000 mfrc522-python-0.0.4/src/mfrc522_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 09:47:47.000000 mfrc522-python-0.0.4/src/mfrc522_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 16:33:47.990706 mfrc522-python-0.0.5.dev0/
+-rw-rw-rw-   0        0        0    35823 2023-04-15 05:57:40.000000 mfrc522-python-0.0.5.dev0/LICENSE
+-rw-rw-rw-   0        0        0     3018 2023-04-18 16:33:47.990706 mfrc522-python-0.0.5.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     2433 2023-04-17 10:38:04.000000 mfrc522-python-0.0.5.dev0/README.md
+-rw-rw-rw-   0        0        0      664 2023-04-18 16:31:03.000000 mfrc522-python-0.0.5.dev0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 16:33:47.991706 mfrc522-python-0.0.5.dev0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 16:33:47.954705 mfrc522-python-0.0.5.dev0/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 16:33:47.965709 mfrc522-python-0.0.5.dev0/src/mfrc522/
+-rw-rw-rw-   0        0        0    22655 2023-04-17 12:07:31.000000 mfrc522-python-0.0.5.dev0/src/mfrc522/MFRC522.py
+-rw-rw-rw-   0        0        0     5614 2023-04-18 16:30:50.000000 mfrc522-python-0.0.5.dev0/src/mfrc522/SimpleMFRC522.py
+-rw-rw-rw-   0        0        0       50 2023-04-15 05:57:40.000000 mfrc522-python-0.0.5.dev0/src/mfrc522/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:33:47.988705 mfrc522-python-0.0.5.dev0/src/mfrc522_python.egg-info/
+-rw-rw-rw-   0        0        0     3018 2023-04-18 16:33:47.000000 mfrc522-python-0.0.5.dev0/src/mfrc522_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-04-18 16:33:47.000000 mfrc522-python-0.0.5.dev0/src/mfrc522_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 16:33:47.000000 mfrc522-python-0.0.5.dev0/src/mfrc522_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-18 16:33:47.000000 mfrc522-python-0.0.5.dev0/src/mfrc522_python.egg-info/top_level.txt
```

### Comparing `mfrc522-python-0.0.4/LICENSE` & `mfrc522-python-0.0.5.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.4/PKG-INFO` & `mfrc522-python-0.0.5.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfrc522-python
-Version: 0.0.4
+Version: 0.0.5.dev0
 Summary: The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip
 Author: Aditya
 Project-URL: Homepage, https://github.com/1AdityaX/mfrc522-python
 Project-URL: Bug Tracker, https://github.com/1AdityaX/mfrc522-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `mfrc522-python-0.0.4/README.md` & `mfrc522-python-0.0.5.dev0/README.md`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.4/pyproject.toml` & `mfrc522-python-0.0.5.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mfrc522-python"
-version = "0.0.4"
+version = "0.0.5.dev"
 authors = [
   { name="Aditya"},
 ]
 description = "The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mfrc522-python-0.0.4/src/mfrc522/MFRC522.py` & `mfrc522-python-0.0.5.dev0/src/mfrc522/MFRC522.py`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.4/src/mfrc522_python.egg-info/PKG-INFO` & `mfrc522-python-0.0.5.dev0/src/mfrc522_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfrc522-python
-Version: 0.0.4
+Version: 0.0.5.dev0
 Summary: The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip
 Author: Aditya
 Project-URL: Homepage, https://github.com/1AdityaX/mfrc522-python
 Project-URL: Bug Tracker, https://github.com/1AdityaX/mfrc522-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

