# Comparing `tmp/TMFuncs-0.0.8.tar.gz` & `tmp/TMFuncs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMFuncs-0.0.8.tar", last modified: Thu Jan 12 07:37:52 2023, max compression
+gzip compressed data, was "TMFuncs-0.0.9.tar", last modified: Thu Jan 19 10:33:03 2023, max compression
```

## Comparing `TMFuncs-0.0.8.tar` & `TMFuncs-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-01-12 07:37:51.999725 TMFuncs-0.0.8/
--rw-rw-rw-   0        0        0     1091 2022-12-21 02:20:24.000000 TMFuncs-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      422 2023-01-12 07:37:51.998728 TMFuncs-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-12-21 02:19:03.000000 TMFuncs-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-12 07:37:51.989728 TMFuncs-0.0.8/TMFuncs/
--rw-rw-rw-   0        0        0      121 2022-12-21 03:06:27.000000 TMFuncs-0.0.8/TMFuncs/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-01-12 07:36:46.000000 TMFuncs-0.0.8/TMFuncs/base.py
--rw-rw-rw-   0        0        0      734 2022-12-19 09:44:54.000000 TMFuncs-0.0.8/TMFuncs/batch_read.py
--rw-rw-rw-   0        0        0     4512 2022-12-21 02:30:38.000000 TMFuncs-0.0.8/TMFuncs/op_log.py
-drwxrwxrwx   0        0        0        0 2023-01-12 07:37:51.996726 TMFuncs-0.0.8/TMFuncs.egg-info/
--rw-rw-rw-   0        0        0      422 2023-01-12 07:37:51.000000 TMFuncs-0.0.8/TMFuncs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-01-12 07:37:51.000000 TMFuncs-0.0.8/TMFuncs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-12 07:37:51.000000 TMFuncs-0.0.8/TMFuncs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-01-12 07:37:51.000000 TMFuncs-0.0.8/TMFuncs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-12 07:37:51.999725 TMFuncs-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1635 2022-12-21 04:26:26.000000 TMFuncs-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-19 10:33:03.475104 TMFuncs-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2022-12-21 02:20:24.000000 TMFuncs-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      422 2023-01-19 10:33:03.474102 TMFuncs-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-12-21 02:19:03.000000 TMFuncs-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-01-19 10:33:03.465104 TMFuncs-0.0.9/TMFuncs/
+-rw-rw-rw-   0        0        0      121 2022-12-21 03:06:27.000000 TMFuncs-0.0.9/TMFuncs/__init__.py
+-rw-rw-rw-   0        0        0     1524 2023-01-12 07:36:46.000000 TMFuncs-0.0.9/TMFuncs/base.py
+-rw-rw-rw-   0        0        0      734 2022-12-19 09:44:54.000000 TMFuncs-0.0.9/TMFuncs/batch_read.py
+-rw-rw-rw-   0        0        0     4512 2022-12-21 02:30:38.000000 TMFuncs-0.0.9/TMFuncs/op_log.py
+-rw-rw-rw-   0        0        0     1875 2023-01-19 10:31:17.000000 TMFuncs-0.0.9/TMFuncs/send_email.py
+drwxrwxrwx   0        0        0        0 2023-01-19 10:33:03.472102 TMFuncs-0.0.9/TMFuncs.egg-info/
+-rw-rw-rw-   0        0        0      422 2023-01-19 10:33:03.000000 TMFuncs-0.0.9/TMFuncs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-01-19 10:33:03.000000 TMFuncs-0.0.9/TMFuncs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-19 10:33:03.000000 TMFuncs-0.0.9/TMFuncs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-01-19 10:33:03.000000 TMFuncs-0.0.9/TMFuncs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-01-19 10:33:03.475104 TMFuncs-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1635 2022-12-21 04:26:26.000000 TMFuncs-0.0.9/setup.py
```

### Comparing `TMFuncs-0.0.8/LICENSE` & `TMFuncs-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `TMFuncs-0.0.8/TMFuncs/base.py` & `TMFuncs-0.0.9/TMFuncs/base.py`

 * *Files identical despite different names*

### Comparing `TMFuncs-0.0.8/TMFuncs/batch_read.py` & `TMFuncs-0.0.9/TMFuncs/batch_read.py`

 * *Files identical despite different names*

### Comparing `TMFuncs-0.0.8/TMFuncs/op_log.py` & `TMFuncs-0.0.9/TMFuncs/op_log.py`

 * *Files identical despite different names*

### Comparing `TMFuncs-0.0.8/setup.py` & `TMFuncs-0.0.9/setup.py`

 * *Files identical despite different names*

