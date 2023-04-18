# Comparing `tmp/jcmutils-1.2.0.tar.gz` & `tmp/jcmutils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.2.0.tar", last modified: Sat Apr 15 13:23:04 2023, max compression
+gzip compressed data, was "jcmutils-1.3.0.tar", last modified: Tue Apr 18 07:50:41 2023, max compression
```

## Comparing `jcmutils-1.2.0.tar` & `jcmutils-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-15 13:23:04.124179 jcmutils-1.2.0/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.2.0/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-15 13:23:04.124179 jcmutils-1.2.0/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.2.0/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-15 13:23:04.124179 jcmutils-1.2.0/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      130 2023-04-15 12:55:54.000000 jcmutils-1.2.0/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.2.0/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.2.0/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     9093 2023-04-15 13:13:52.000000 jcmutils-1.2.0/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-15 13:23:04.124179 jcmutils-1.2.0/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-15 13:23:04.000000 jcmutils-1.2.0/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      268 2023-04-15 13:23:04.000000 jcmutils-1.2.0/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-04-15 13:23:04.000000 jcmutils-1.2.0/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       17 2023-04-15 13:23:04.000000 jcmutils-1.2.0/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-04-15 13:23:04.000000 jcmutils-1.2.0/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-04-15 13:23:04.124179 jcmutils-1.2.0/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      514 2023-04-15 13:15:27.000000 jcmutils-1.2.0/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-18 07:50:41.581172 jcmutils-1.3.0/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.3.0/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-18 07:50:41.581172 jcmutils-1.3.0/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.3.0/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-18 07:50:41.581172 jcmutils-1.3.0/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.3.0/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2677 2023-04-18 07:46:32.000000 jcmutils-1.3.0/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.3.0/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.3.0/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8004 2023-04-18 07:27:53.000000 jcmutils-1.3.0/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-18 07:50:41.581172 jcmutils-1.3.0/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-18 07:50:41.000000 jcmutils-1.3.0/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-04-18 07:50:41.000000 jcmutils-1.3.0/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-04-18 07:50:41.000000 jcmutils-1.3.0/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       24 2023-04-18 07:50:41.000000 jcmutils-1.3.0/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-04-18 07:50:41.000000 jcmutils-1.3.0/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-04-18 07:50:41.581172 jcmutils-1.3.0/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      523 2023-04-18 07:47:07.000000 jcmutils-1.3.0/setup.py
```

### Comparing `jcmutils-1.2.0/LICENSE` & `jcmutils-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.2.0/README.md` & `jcmutils-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.2.0/jcmutils/gen_sources.py` & `jcmutils-1.3.0/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.2.0/jcmutils/logger.py` & `jcmutils-1.3.0/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.2.0/setup.py` & `jcmutils-1.3.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.2.0'
+VERSION = '1.3.0'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
     description=DESCRIPTION,
     packages=find_packages(),
-    install_requires=["numpy","matplotlib"],
+    install_requires=["numpy","matplotlib","opencv"],
     keywords=["jcmsuite","utils"],
     classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     ]
 )
```

