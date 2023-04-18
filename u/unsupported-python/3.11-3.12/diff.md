# Comparing `tmp/unsupported-python-3.11.tar.gz` & `tmp/unsupported-python-3.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unsupported-python-3.11.tar", last modified: Tue Apr 18 12:48:10 2023, max compression
+gzip compressed data, was "unsupported-python-3.12.tar", last modified: Tue Apr 18 12:47:26 2023, max compression
```

## Comparing `unsupported-python-3.11.tar` & `unsupported-python-3.12.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 ntessore   (501) staff       (20)        0 2023-04-18 12:48:10.829652 unsupported-python-3.11/
--rw-r--r--   0 ntessore   (501) staff       (20)       61 2023-04-18 12:48:10.829374 unsupported-python-3.11/PKG-INFO
--rw-r--r--   0 ntessore   (501) staff       (20)       38 2023-04-18 12:48:10.829719 unsupported-python-3.11/setup.cfg
--rw-r--r--   0 ntessore   (501) staff       (20)      427 2023-04-18 12:48:03.000000 unsupported-python-3.11/setup.py
-drwxr-xr-x   0 ntessore   (501) staff       (20)        0 2023-04-18 12:48:10.828990 unsupported-python-3.11/unsupported_python.egg-info/
--rw-r--r--   0 ntessore   (501) staff       (20)       61 2023-04-18 12:48:10.000000 unsupported-python-3.11/unsupported_python.egg-info/PKG-INFO
--rw-r--r--   0 ntessore   (501) staff       (20)      176 2023-04-18 12:48:10.000000 unsupported-python-3.11/unsupported_python.egg-info/SOURCES.txt
--rw-r--r--   0 ntessore   (501) staff       (20)        1 2023-04-18 12:48:10.000000 unsupported-python-3.11/unsupported_python.egg-info/dependency_links.txt
--rw-r--r--   0 ntessore   (501) staff       (20)        1 2023-04-18 12:48:10.000000 unsupported-python-3.11/unsupported_python.egg-info/top_level.txt
+drwxr-xr-x   0 ntessore   (501) staff       (20)        0 2023-04-18 12:47:26.315847 unsupported-python-3.12/
+-rw-r--r--   0 ntessore   (501) staff       (20)       61 2023-04-18 12:47:26.315551 unsupported-python-3.12/PKG-INFO
+-rw-r--r--   0 ntessore   (501) staff       (20)       38 2023-04-18 12:47:26.315915 unsupported-python-3.12/setup.cfg
+-rw-r--r--   0 ntessore   (501) staff       (20)      427 2023-04-18 12:45:45.000000 unsupported-python-3.12/setup.py
+drwxr-xr-x   0 ntessore   (501) staff       (20)        0 2023-04-18 12:47:26.315274 unsupported-python-3.12/unsupported_python.egg-info/
+-rw-r--r--   0 ntessore   (501) staff       (20)       61 2023-04-18 12:47:26.000000 unsupported-python-3.12/unsupported_python.egg-info/PKG-INFO
+-rw-r--r--   0 ntessore   (501) staff       (20)      176 2023-04-18 12:47:26.000000 unsupported-python-3.12/unsupported_python.egg-info/SOURCES.txt
+-rw-r--r--   0 ntessore   (501) staff       (20)        1 2023-04-18 12:47:26.000000 unsupported-python-3.12/unsupported_python.egg-info/dependency_links.txt
+-rw-r--r--   0 ntessore   (501) staff       (20)        1 2023-04-18 12:47:26.000000 unsupported-python-3.12/unsupported_python.egg-info/top_level.txt
```

