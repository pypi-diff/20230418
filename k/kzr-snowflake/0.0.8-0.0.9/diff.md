# Comparing `tmp/kzr_snowflake-0.0.8.tar.gz` & `tmp/kzr_snowflake-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kzr_snowflake-0.0.8.tar", last modified: Mon Apr 11 22:24:36 2022, max compression
+gzip compressed data, was "dist/kzr_snowflake-0.0.9.tar", last modified: Mon Apr 11 23:30:15 2022, max compression
```

## Comparing `kzr_snowflake-0.0.8.tar` & `kzr_snowflake-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 mrkfw      (504) staff       (20)        0 2022-04-11 22:24:36.365366 kzr_snowflake-0.0.8/
--rw-r--r--   0 mrkfw      (504) staff       (20)      169 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/AUTHORS.rst
--rw-r--r--   0 mrkfw      (504) staff       (20)     3605 2022-01-08 00:40:04.000000 kzr_snowflake-0.0.8/CONTRIBUTING.rst
--rw-r--r--   0 mrkfw      (504) staff       (20)       89 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/HISTORY.rst
--rw-r--r--   0 mrkfw      (504) staff       (20)     1547 2022-01-08 00:40:04.000000 kzr_snowflake-0.0.8/LICENSE
--rw-r--r--   0 mrkfw      (504) staff       (20)      262 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/MANIFEST.in
--rw-r--r--   0 mrkfw      (504) staff       (20)     1793 2022-04-11 22:24:36.366018 kzr_snowflake-0.0.8/PKG-INFO
--rw-r--r--   0 mrkfw      (504) staff       (20)      926 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/README.rst
-drwxr-xr-x   0 mrkfw      (504) staff       (20)        0 2022-04-11 22:24:36.319636 kzr_snowflake-0.0.8/docs/
--rw-r--r--   0 mrkfw      (504) staff       (20)      614 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/docs/Makefile
--rw-r--r--   0 mrkfw      (504) staff       (20)       28 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/docs/authors.rst
--rwxr-xr-x   0 mrkfw      (504) staff       (20)     4880 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/docs/conf.py
--rw-r--r--   0 mrkfw      (504) staff       (20)       33 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/docs/contributing.rst
--rw-r--r--   0 mrkfw      (504) staff       (20)       28 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/docs/history.rst
--rw-r--r--   0 mrkfw      (504) staff       (20)      310 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/docs/index.rst
--rw-r--r--   0 mrkfw      (504) staff       (20)     1174 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/docs/installation.rst
--rw-r--r--   0 mrkfw      (504) staff       (20)      775 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/docs/make.bat
--rw-r--r--   0 mrkfw      (504) staff       (20)       27 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/docs/readme.rst
--rw-r--r--   0 mrkfw      (504) staff       (20)       81 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/docs/usage.rst
-drwxr-xr-x   0 mrkfw      (504) staff       (20)        0 2022-04-11 22:24:36.328075 kzr_snowflake-0.0.8/kzr_snowflake/
--rw-r--r--   0 mrkfw      (504) staff       (20)      144 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/kzr_snowflake/__init__.py
--rw-r--r--   0 mrkfw      (504) staff       (20)      316 2022-04-11 22:12:40.000000 kzr_snowflake-0.0.8/kzr_snowflake/cli.py
--rw-r--r--   0 mrkfw      (504) staff       (20)     4343 2022-04-11 22:24:26.000000 kzr_snowflake-0.0.8/kzr_snowflake/kzr_snowflake.py
-drwxr-xr-x   0 mrkfw      (504) staff       (20)        0 2022-04-11 22:24:36.333143 kzr_snowflake-0.0.8/kzr_snowflake.egg-info/
--rw-r--r--   0 mrkfw      (504) staff       (20)     1793 2022-04-11 22:24:34.000000 kzr_snowflake-0.0.8/kzr_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 mrkfw      (504) staff       (20)      639 2022-04-11 22:24:35.000000 kzr_snowflake-0.0.8/kzr_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 mrkfw      (504) staff       (20)        1 2022-04-11 22:24:34.000000 kzr_snowflake-0.0.8/kzr_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 mrkfw      (504) staff       (20)       58 2022-04-11 22:24:34.000000 kzr_snowflake-0.0.8/kzr_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 mrkfw      (504) staff       (20)        1 2022-01-08 00:51:19.000000 kzr_snowflake-0.0.8/kzr_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 mrkfw      (504) staff       (20)      734 2022-04-11 22:24:34.000000 kzr_snowflake-0.0.8/kzr_snowflake.egg-info/requires.txt
--rw-r--r--   0 mrkfw      (504) staff       (20)       14 2022-04-11 22:24:34.000000 kzr_snowflake-0.0.8/kzr_snowflake.egg-info/top_level.txt
--rw-r--r--   0 mrkfw      (504) staff       (20)      385 2022-04-11 22:24:36.370655 kzr_snowflake-0.0.8/setup.cfg
--rw-r--r--   0 mrkfw      (504) staff       (20)     2504 2022-04-11 22:17:57.000000 kzr_snowflake-0.0.8/setup.py
-drwxr-xr-x   0 mrkfw      (504) staff       (20)        0 2022-04-11 22:24:36.364583 kzr_snowflake-0.0.8/tests/
--rw-r--r--   0 mrkfw      (504) staff       (20)       43 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/tests/__init__.py
--rw-r--r--   0 mrkfw      (504) staff       (20)      894 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.8/tests/test_kzr_snowflake.py
+drwxr-xr-x   0 mrkfw      (504) staff       (20)        0 2022-04-11 23:30:15.905725 kzr_snowflake-0.0.9/
+-rw-r--r--   0 mrkfw      (504) staff       (20)      169 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/AUTHORS.rst
+-rw-r--r--   0 mrkfw      (504) staff       (20)     3605 2022-01-08 00:40:04.000000 kzr_snowflake-0.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 mrkfw      (504) staff       (20)       89 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/HISTORY.rst
+-rw-r--r--   0 mrkfw      (504) staff       (20)     1547 2022-01-08 00:40:04.000000 kzr_snowflake-0.0.9/LICENSE
+-rw-r--r--   0 mrkfw      (504) staff       (20)      262 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/MANIFEST.in
+-rw-r--r--   0 mrkfw      (504) staff       (20)     1793 2022-04-11 23:30:15.905959 kzr_snowflake-0.0.9/PKG-INFO
+-rw-r--r--   0 mrkfw      (504) staff       (20)      926 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/README.rst
+drwxr-xr-x   0 mrkfw      (504) staff       (20)        0 2022-04-11 23:30:15.849874 kzr_snowflake-0.0.9/docs/
+-rw-r--r--   0 mrkfw      (504) staff       (20)      614 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/docs/Makefile
+-rw-r--r--   0 mrkfw      (504) staff       (20)       28 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/docs/authors.rst
+-rwxr-xr-x   0 mrkfw      (504) staff       (20)     4880 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/docs/conf.py
+-rw-r--r--   0 mrkfw      (504) staff       (20)       33 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/docs/contributing.rst
+-rw-r--r--   0 mrkfw      (504) staff       (20)       28 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/docs/history.rst
+-rw-r--r--   0 mrkfw      (504) staff       (20)      310 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/docs/index.rst
+-rw-r--r--   0 mrkfw      (504) staff       (20)     1174 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/docs/installation.rst
+-rw-r--r--   0 mrkfw      (504) staff       (20)      775 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/docs/make.bat
+-rw-r--r--   0 mrkfw      (504) staff       (20)       27 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/docs/readme.rst
+-rw-r--r--   0 mrkfw      (504) staff       (20)       81 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/docs/usage.rst
+drwxr-xr-x   0 mrkfw      (504) staff       (20)        0 2022-04-11 23:30:15.886344 kzr_snowflake-0.0.9/kzr_snowflake/
+-rw-r--r--   0 mrkfw      (504) staff       (20)      144 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/kzr_snowflake/__init__.py
+-rw-r--r--   0 mrkfw      (504) staff       (20)      316 2022-04-11 22:12:40.000000 kzr_snowflake-0.0.9/kzr_snowflake/cli.py
+-rw-r--r--   0 mrkfw      (504) staff       (20)     4708 2022-04-11 23:29:58.000000 kzr_snowflake-0.0.9/kzr_snowflake/kzr_snowflake.py
+drwxr-xr-x   0 mrkfw      (504) staff       (20)        0 2022-04-11 23:30:15.891479 kzr_snowflake-0.0.9/kzr_snowflake.egg-info/
+-rw-r--r--   0 mrkfw      (504) staff       (20)     1793 2022-04-11 23:30:14.000000 kzr_snowflake-0.0.9/kzr_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 mrkfw      (504) staff       (20)      639 2022-04-11 23:30:14.000000 kzr_snowflake-0.0.9/kzr_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 mrkfw      (504) staff       (20)        1 2022-04-11 23:30:14.000000 kzr_snowflake-0.0.9/kzr_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 mrkfw      (504) staff       (20)       58 2022-04-11 23:30:14.000000 kzr_snowflake-0.0.9/kzr_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 mrkfw      (504) staff       (20)        1 2022-01-08 00:51:19.000000 kzr_snowflake-0.0.9/kzr_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 mrkfw      (504) staff       (20)      734 2022-04-11 23:30:14.000000 kzr_snowflake-0.0.9/kzr_snowflake.egg-info/requires.txt
+-rw-r--r--   0 mrkfw      (504) staff       (20)       14 2022-04-11 23:30:14.000000 kzr_snowflake-0.0.9/kzr_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 mrkfw      (504) staff       (20)      385 2022-04-11 23:30:15.909213 kzr_snowflake-0.0.9/setup.cfg
+-rw-r--r--   0 mrkfw      (504) staff       (20)     2504 2022-04-11 23:30:09.000000 kzr_snowflake-0.0.9/setup.py
+drwxr-xr-x   0 mrkfw      (504) staff       (20)        0 2022-04-11 23:30:15.904999 kzr_snowflake-0.0.9/tests/
+-rw-r--r--   0 mrkfw      (504) staff       (20)       43 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/tests/__init__.py
+-rw-r--r--   0 mrkfw      (504) staff       (20)      894 2022-01-08 00:40:05.000000 kzr_snowflake-0.0.9/tests/test_kzr_snowflake.py
```

### Comparing `kzr_snowflake-0.0.8/CONTRIBUTING.rst` & `kzr_snowflake-0.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `kzr_snowflake-0.0.8/LICENSE` & `kzr_snowflake-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kzr_snowflake-0.0.8/PKG-INFO` & `kzr_snowflake-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kzr_snowflake
-Version: 0.0.8
+Version: 0.0.9
 Summary: Snowflake helper library
 Home-page: https://github.com/kzraryan-mu/kzr_snowflake
 Author: Md Kamruz Zaman Rana
 Author-email: mrkfw@mail.missouri.edu
 License: GNU General Public License v3
 Keywords: kzr_snowflake
 Platform: UNKNOWN
```

### Comparing `kzr_snowflake-0.0.8/README.rst` & `kzr_snowflake-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `kzr_snowflake-0.0.8/docs/Makefile` & `kzr_snowflake-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kzr_snowflake-0.0.8/docs/conf.py` & `kzr_snowflake-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kzr_snowflake-0.0.8/docs/installation.rst` & `kzr_snowflake-0.0.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `kzr_snowflake-0.0.8/docs/make.bat` & `kzr_snowflake-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kzr_snowflake-0.0.8/kzr_snowflake.egg-info/PKG-INFO` & `kzr_snowflake-0.0.9/kzr_snowflake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kzr-snowflake
-Version: 0.0.8
+Version: 0.0.9
 Summary: Snowflake helper library
 Home-page: https://github.com/kzraryan-mu/kzr_snowflake
 Author: Md Kamruz Zaman Rana
 Author-email: mrkfw@mail.missouri.edu
 License: GNU General Public License v3
 Keywords: kzr_snowflake
 Platform: UNKNOWN
```

### Comparing `kzr_snowflake-0.0.8/kzr_snowflake.egg-info/SOURCES.txt` & `kzr_snowflake-0.0.9/kzr_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kzr_snowflake-0.0.8/kzr_snowflake.egg-info/requires.txt` & `kzr_snowflake-0.0.9/kzr_snowflake.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kzr_snowflake-0.0.8/setup.py` & `kzr_snowflake-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,10 +82,10 @@
     include_package_data=True,
     keywords='kzr_snowflake',
     name='kzr_snowflake',
     packages=find_packages(include=['kzr_snowflake', 'kzr_snowflake.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/kzraryan-mu/kzr_snowflake',
-    version='0.0.8',
+    version='0.0.9',
     zip_safe=False,
 )
```

### Comparing `kzr_snowflake-0.0.8/tests/test_kzr_snowflake.py` & `kzr_snowflake-0.0.9/tests/test_kzr_snowflake.py`

 * *Files identical despite different names*

