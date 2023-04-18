# Comparing `tmp/student-repos-handler-1.3.0.tar.gz` & `tmp/student-repos-handler-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "student-repos-handler-1.3.0.tar", last modified: Mon Apr 10 22:44:08 2023, max compression
+gzip compressed data, was "student-repos-handler-2.0.0.tar", last modified: Tue Apr 18 00:10:21 2023, max compression
```

## Comparing `student-repos-handler-1.3.0.tar` & `student-repos-handler-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 fisa      (1000) fisa      (1000)        0 2023-04-10 22:44:08.086051 student-repos-handler-1.3.0/
--rw-rw-r--   0 fisa      (1000) fisa      (1000)     1009 2023-04-10 22:44:08.086051 student-repos-handler-1.3.0/PKG-INFO
--rw-r--r--   0 fisa      (1000) fisa      (1000)      256 2020-09-12 01:06:10.000000 student-repos-handler-1.3.0/README.md
--rwxr-xr-x   0 fisa      (1000) fisa      (1000)    12435 2023-04-10 22:42:35.000000 student-repos-handler-1.3.0/repos.py
--rw-rw-r--   0 fisa      (1000) fisa      (1000)       38 2023-04-10 22:44:08.086051 student-repos-handler-1.3.0/setup.cfg
--rw-rw-r--   0 fisa      (1000) fisa      (1000)      910 2023-04-10 22:43:48.000000 student-repos-handler-1.3.0/setup.py
-drwxrwxr-x   0 fisa      (1000) fisa      (1000)        0 2023-04-10 22:44:08.086051 student-repos-handler-1.3.0/student_repos_handler.egg-info/
--rw-rw-r--   0 fisa      (1000) fisa      (1000)     1009 2023-04-10 22:44:07.000000 student-repos-handler-1.3.0/student_repos_handler.egg-info/PKG-INFO
--rw-rw-r--   0 fisa      (1000) fisa      (1000)      299 2023-04-10 22:44:07.000000 student-repos-handler-1.3.0/student_repos_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 fisa      (1000) fisa      (1000)        1 2023-04-10 22:44:07.000000 student-repos-handler-1.3.0/student_repos_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 fisa      (1000) fisa      (1000)       38 2023-04-10 22:44:07.000000 student-repos-handler-1.3.0/student_repos_handler.egg-info/entry_points.txt
--rw-rw-r--   0 fisa      (1000) fisa      (1000)       19 2023-04-10 22:44:07.000000 student-repos-handler-1.3.0/student_repos_handler.egg-info/requires.txt
--rw-rw-r--   0 fisa      (1000) fisa      (1000)        6 2023-04-10 22:44:07.000000 student-repos-handler-1.3.0/student_repos_handler.egg-info/top_level.txt
+drwxrwxr-x   0 fisa      (1000) fisa      (1000)        0 2023-04-18 00:10:21.395319 student-repos-handler-2.0.0/
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)     1009 2023-04-18 00:10:21.395319 student-repos-handler-2.0.0/PKG-INFO
+-rw-r--r--   0 fisa      (1000) fisa      (1000)      256 2020-09-12 01:06:10.000000 student-repos-handler-2.0.0/README.md
+-rwxr-xr-x   0 fisa      (1000) fisa      (1000)    17815 2023-04-18 00:07:07.000000 student-repos-handler-2.0.0/repos.py
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)       38 2023-04-18 00:10:21.395319 student-repos-handler-2.0.0/setup.cfg
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)      910 2023-04-18 00:09:34.000000 student-repos-handler-2.0.0/setup.py
+drwxrwxr-x   0 fisa      (1000) fisa      (1000)        0 2023-04-18 00:10:21.395319 student-repos-handler-2.0.0/student_repos_handler.egg-info/
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)     1009 2023-04-18 00:10:21.000000 student-repos-handler-2.0.0/student_repos_handler.egg-info/PKG-INFO
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)      299 2023-04-18 00:10:21.000000 student-repos-handler-2.0.0/student_repos_handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)        1 2023-04-18 00:10:21.000000 student-repos-handler-2.0.0/student_repos_handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)       38 2023-04-18 00:10:21.000000 student-repos-handler-2.0.0/student_repos_handler.egg-info/entry_points.txt
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)       19 2023-04-18 00:10:21.000000 student-repos-handler-2.0.0/student_repos_handler.egg-info/requires.txt
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)        6 2023-04-18 00:10:21.000000 student-repos-handler-2.0.0/student_repos_handler.egg-info/top_level.txt
```

### Comparing `student-repos-handler-1.3.0/PKG-INFO` & `student-repos-handler-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: student-repos-handler
-Version: 1.3.0
+Version: 2.0.0
 Summary: Simple tool to handle multiple repos at once, oriented to the grading of assignments in UCSE DAR
 Home-page: https://github.com/fisadev/student-repos-handler
 Author: Juan Pedro Fisanotti
 Author-email: fisadev@gmail.com
 License: LICENSE.txt
 Description: # Student-repos-handler
```

### Comparing `student-repos-handler-1.3.0/setup.py` & `student-repos-handler-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(
     name='student-repos-handler',
-    version='1.3.0',
+    version='2.0.0',
     description='Simple tool to handle multiple repos at once, oriented to the grading of assignments in UCSE DAR',
     long_description=open('README.md').read(),
     author='Juan Pedro Fisanotti',
     author_email='fisadev@gmail.com',
     url='https://github.com/fisadev/student-repos-handler',
     license='LICENSE.txt',
     python_requires='>=3.4',
```

### Comparing `student-repos-handler-1.3.0/student_repos_handler.egg-info/PKG-INFO` & `student-repos-handler-2.0.0/student_repos_handler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: student-repos-handler
-Version: 1.3.0
+Version: 2.0.0
 Summary: Simple tool to handle multiple repos at once, oriented to the grading of assignments in UCSE DAR
 Home-page: https://github.com/fisadev/student-repos-handler
 Author: Juan Pedro Fisanotti
 Author-email: fisadev@gmail.com
 License: LICENSE.txt
 Description: # Student-repos-handler
```

