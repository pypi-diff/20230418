# Comparing `tmp/positional_defaults-2023.4.17.tar.gz` & `tmp/positional_defaults-2023.4.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "positional_defaults-2023.4.17.tar", last modified: Mon Apr 17 09:31:25 2023, max compression
+gzip compressed data, was "positional_defaults-2023.4.18.tar", last modified: Tue Apr 18 10:14:31 2023, max compression
```

## Comparing `positional_defaults-2023.4.17.tar` & `positional_defaults-2023.4.18.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ntessore   (501) staff       (20)        0 2023-04-17 09:31:25.141966 positional_defaults-2023.4.17/
--rw-r--r--   0 ntessore   (501) staff       (20)     1072 2023-04-15 03:02:05.000000 positional_defaults-2023.4.17/LICENSE.txt
--rw-r--r--   0 ntessore   (501) staff       (20)     3607 2023-04-17 09:31:25.141720 positional_defaults-2023.4.17/PKG-INFO
--rw-r--r--   0 ntessore   (501) staff       (20)     1844 2023-04-17 08:54:08.000000 positional_defaults-2023.4.17/README.md
--rw-r--r--   0 ntessore   (501) staff       (20)     1002 2023-04-17 08:00:48.000000 positional_defaults-2023.4.17/_positional_defaults.py
-drwxr-xr-x   0 ntessore   (501) staff       (20)        0 2023-04-17 09:31:25.141418 positional_defaults-2023.4.17/positional_defaults.egg-info/
--rw-r--r--   0 ntessore   (501) staff       (20)     3607 2023-04-17 09:31:25.000000 positional_defaults-2023.4.17/positional_defaults.egg-info/PKG-INFO
--rw-r--r--   0 ntessore   (501) staff       (20)      264 2023-04-17 09:31:25.000000 positional_defaults-2023.4.17/positional_defaults.egg-info/SOURCES.txt
--rw-r--r--   0 ntessore   (501) staff       (20)        1 2023-04-17 09:31:25.000000 positional_defaults-2023.4.17/positional_defaults.egg-info/dependency_links.txt
--rw-r--r--   0 ntessore   (501) staff       (20)       41 2023-04-17 09:31:25.000000 positional_defaults-2023.4.17/positional_defaults.egg-info/top_level.txt
--rw-r--r--   0 ntessore   (501) staff       (20)     2247 2023-04-17 08:54:08.000000 positional_defaults-2023.4.17/positional_defaults.py
--rw-r--r--   0 ntessore   (501) staff       (20)      788 2023-04-17 09:12:19.000000 positional_defaults-2023.4.17/pyproject.toml
--rw-r--r--   0 ntessore   (501) staff       (20)       38 2023-04-17 09:31:25.142061 positional_defaults-2023.4.17/setup.cfg
--rw-r--r--   0 ntessore   (501) staff       (20)      123 2023-04-17 09:12:11.000000 positional_defaults-2023.4.17/setup.py
+drwxr-xr-x   0 ntessore   (501) staff       (20)        0 2023-04-18 10:14:31.153699 positional_defaults-2023.4.18/
+-rw-r--r--   0 ntessore   (501) staff       (20)     1072 2023-04-15 03:02:05.000000 positional_defaults-2023.4.18/LICENSE.txt
+-rw-r--r--   0 ntessore   (501) staff       (20)     2418 2023-04-18 10:14:31.153296 positional_defaults-2023.4.18/PKG-INFO
+-rw-r--r--   0 ntessore   (501) staff       (20)     1844 2023-04-17 09:34:00.000000 positional_defaults-2023.4.18/README.md
+-rw-r--r--   0 ntessore   (501) staff       (20)      820 2023-04-18 09:58:09.000000 positional_defaults-2023.4.18/_positional_defaults.py
+drwxr-xr-x   0 ntessore   (501) staff       (20)        0 2023-04-18 10:14:31.152612 positional_defaults-2023.4.18/positional_defaults.egg-info/
+-rw-r--r--   0 ntessore   (501) staff       (20)     2418 2023-04-18 10:14:31.000000 positional_defaults-2023.4.18/positional_defaults.egg-info/PKG-INFO
+-rw-r--r--   0 ntessore   (501) staff       (20)      264 2023-04-18 10:14:31.000000 positional_defaults-2023.4.18/positional_defaults.egg-info/SOURCES.txt
+-rw-r--r--   0 ntessore   (501) staff       (20)        1 2023-04-18 10:14:31.000000 positional_defaults-2023.4.18/positional_defaults.egg-info/dependency_links.txt
+-rw-r--r--   0 ntessore   (501) staff       (20)       41 2023-04-18 10:14:31.000000 positional_defaults-2023.4.18/positional_defaults.egg-info/top_level.txt
+-rw-r--r--   0 ntessore   (501) staff       (20)     2823 2023-04-18 10:08:28.000000 positional_defaults-2023.4.18/positional_defaults.py
+-rw-r--r--   0 ntessore   (501) staff       (20)      823 2023-04-18 10:14:02.000000 positional_defaults-2023.4.18/pyproject.toml
+-rw-r--r--   0 ntessore   (501) staff       (20)       38 2023-04-18 10:14:31.153801 positional_defaults-2023.4.18/setup.cfg
+-rw-r--r--   0 ntessore   (501) staff       (20)      692 2023-04-18 09:33:36.000000 positional_defaults-2023.4.18/setup.py
```

### Comparing `positional_defaults-2023.4.17/LICENSE.txt` & `positional_defaults-2023.4.18/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `positional_defaults-2023.4.17/README.md` & `positional_defaults-2023.4.18/README.md`

 * *Files identical despite different names*

### Comparing `positional_defaults-2023.4.17/pyproject.toml` & `positional_defaults-2023.4.18/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 name = "positional_defaults"
 authors = [
     {name = "Nicolas Tessore", email = "n.tessore@ucl.ac.uk"},
     {name = "Nathaniel Starkman", email = "n.starkman@mail.utoronto.ca"},
 ]
 description = "Set defaults for any positional-only parameter"
 readme = "README.md"
-license = {file = "LICENSE.txt"}
+license = {text = "MIT"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
 ]
 requires-python = ">=3.8"
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/ntessore/positional_defaults"
 Issues = "https://github.com/ntessore/positional_defaults/issues"
```

