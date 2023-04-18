# Comparing `tmp/lazy_streams-1.0.0.tar.gz` & `tmp/lazy_streams-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_streams-1.0.0.tar", last modified: Sun Aug 14 01:41:12 2022, max compression
+gzip compressed data, was "lazy_streams-1.0.1.tar", last modified: Tue Apr 18 20:48:31 2023, max compression
```

## Comparing `lazy_streams-1.0.0.tar` & `lazy_streams-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2022-08-14 01:41:12.786866 lazy_streams-1.0.0/
--rw-r--r--   0 steve      (501) staff       (20)    34523 2022-08-14 00:52:20.000000 lazy_streams-1.0.0/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)    46531 2022-08-14 01:41:12.787006 lazy_streams-1.0.0/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     6069 2022-08-14 01:00:36.000000 lazy_streams-1.0.0/README.md
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2022-08-14 01:41:12.786769 lazy_streams-1.0.0/lazy_streams.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    46531 2022-08-14 01:41:12.000000 lazy_streams-1.0.0/lazy_streams.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      211 2022-08-14 01:41:12.000000 lazy_streams-1.0.0/lazy_streams.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2022-08-14 01:41:12.000000 lazy_streams-1.0.0/lazy_streams.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       13 2022-08-14 01:41:12.000000 lazy_streams-1.0.0/lazy_streams.egg-info/top_level.txt
--rw-r--r--   0 steve      (501) staff       (20)    14169 2022-08-14 00:33:42.000000 lazy_streams-1.0.0/lazy_streams.py
--rw-r--r--   0 steve      (501) staff       (20)      824 2022-08-14 01:40:44.000000 lazy_streams-1.0.0/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)      152 2022-08-14 01:41:12.787236 lazy_streams-1.0.0/setup.cfg
--rw-r--r--   0 steve      (501) staff       (20)       61 2022-08-14 00:58:14.000000 lazy_streams-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:31.392197 lazy_streams-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-18 20:47:58.000000 lazy_streams-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46587 2023-04-18 20:48:31.392197 lazy_streams-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-18 20:47:58.000000 lazy_streams-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:31.388197 lazy_streams-1.0.1/lazy_streams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46587 2023-04-18 20:48:31.000000 lazy_streams-1.0.1/lazy_streams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-18 20:48:31.000000 lazy_streams-1.0.1/lazy_streams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:48:31.000000 lazy_streams-1.0.1/lazy_streams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 20:48:31.000000 lazy_streams-1.0.1/lazy_streams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 20:48:31.000000 lazy_streams-1.0.1/lazy_streams.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14169 2023-04-18 20:47:58.000000 lazy_streams-1.0.1/lazy_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-18 20:47:58.000000 lazy_streams-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-18 20:48:31.392197 lazy_streams-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-18 20:47:58.000000 lazy_streams-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:48:31.392197 lazy_streams-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-18 20:47:58.000000 lazy_streams-1.0.1/tests/test_lazy_streams.py
```

### Comparing `lazy_streams-1.0.0/LICENSE` & `lazy_streams-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lazy_streams-1.0.0/PKG-INFO` & `lazy_streams-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy_streams
-Version: 1.0.0
+Version: 1.0.1
 Summary: Java inspired streams in Python
 Author-email: Steve Brettschneider <steve@bluehousefamily.com>, Rémi Desgrange <remi.desgrange@camptocamp.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -666,14 +666,15 @@
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/brettschneider/python_lazy_streams
 Project-URL: Bug Tracker, https://github.com/brettschneider/python_lazy_streams/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Python lazy\_streams
 ====================
```

### Comparing `lazy_streams-1.0.0/README.md` & `lazy_streams-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lazy_streams-1.0.0/lazy_streams.egg-info/PKG-INFO` & `lazy_streams-1.0.1/lazy_streams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-streams
-Version: 1.0.0
+Version: 1.0.1
 Summary: Java inspired streams in Python
 Author-email: Steve Brettschneider <steve@bluehousefamily.com>, Rémi Desgrange <remi.desgrange@camptocamp.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -666,14 +666,15 @@
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Homepage, https://github.com/brettschneider/python_lazy_streams
 Project-URL: Bug Tracker, https://github.com/brettschneider/python_lazy_streams/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Python lazy\_streams
 ====================
```

### Comparing `lazy_streams-1.0.0/lazy_streams.py` & `lazy_streams-1.0.1/lazy_streams.py`

 * *Files identical despite different names*

