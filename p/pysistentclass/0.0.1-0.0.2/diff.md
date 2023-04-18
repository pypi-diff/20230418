# Comparing `tmp/pysistentclass-0.0.1.tar.gz` & `tmp/pysistentclass-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysistentclass-0.0.1.tar", last modified: Tue Apr 18 15:31:42 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pysistentclass-0.0.1.tar` & `pysistentclass-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,6 @@
-drwxr-xr-x   0 marc      (1000) marc      (1000)        0 2023-04-18 15:31:42.470773 pysistentclass-0.0.1/
--rw-r--r--   0 marc      (1000) marc      (1000)    35148 2023-04-18 15:31:09.000000 pysistentclass-0.0.1/LICENSE
--rw-r--r--   0 marc      (1000) marc      (1000)      621 2023-04-18 15:31:42.470773 pysistentclass-0.0.1/PKG-INFO
--rw-r--r--   0 marc      (1000) marc      (1000)       58 2023-04-18 15:30:14.000000 pysistentclass-0.0.1/README.md
--rw-r--r--   0 marc      (1000) marc      (1000)      682 2023-04-18 15:31:01.000000 pysistentclass-0.0.1/pyproject.toml
--rw-r--r--   0 marc      (1000) marc      (1000)       38 2023-04-18 15:31:42.470773 pysistentclass-0.0.1/setup.cfg
-drwxr-xr-x   0 marc      (1000) marc      (1000)        0 2023-04-18 15:31:42.467439 pysistentclass-0.0.1/src/
-drwxr-xr-x   0 marc      (1000) marc      (1000)        0 2023-04-18 15:31:42.470773 pysistentclass-0.0.1/src/pysistentclass/
--rw-r--r--   0 marc      (1000) marc      (1000)     6487 2023-04-18 15:29:55.000000 pysistentclass-0.0.1/src/pysistentclass/__init__.py
-drwxr-xr-x   0 marc      (1000) marc      (1000)        0 2023-04-18 15:31:42.470773 pysistentclass-0.0.1/src/pysistentclass.egg-info/
--rw-r--r--   0 marc      (1000) marc      (1000)      621 2023-04-18 15:31:42.000000 pysistentclass-0.0.1/src/pysistentclass.egg-info/PKG-INFO
--rw-r--r--   0 marc      (1000) marc      (1000)      272 2023-04-18 15:31:42.000000 pysistentclass-0.0.1/src/pysistentclass.egg-info/SOURCES.txt
--rw-r--r--   0 marc      (1000) marc      (1000)        1 2023-04-18 15:31:42.000000 pysistentclass-0.0.1/src/pysistentclass.egg-info/dependency_links.txt
--rw-r--r--   0 marc      (1000) marc      (1000)       21 2023-04-18 15:31:42.000000 pysistentclass-0.0.1/src/pysistentclass.egg-info/requires.txt
--rw-r--r--   0 marc      (1000) marc      (1000)       15 2023-04-18 15:31:42.000000 pysistentclass-0.0.1/src/pysistentclass.egg-info/top_level.txt
+-rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 pysistentclass-0.0.2/src/pysistentclass/__init__.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pysistentclass-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pysistentclass-0.0.2/LICENSE
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pysistentclass-0.0.2/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pysistentclass-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 pysistentclass-0.0.2/PKG-INFO
```

### Comparing `pysistentclass-0.0.1/LICENSE` & `pysistentclass-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysistentclass-0.0.1/pyproject.toml` & `pysistentclass-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "pysistentclass"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "manjaroman2", email = "manjaroman2@protonmail.com" }]
 description = "A small settings module for python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

