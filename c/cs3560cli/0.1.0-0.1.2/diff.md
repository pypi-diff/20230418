# Comparing `tmp/cs3560cli-0.1.0.tar.gz` & `tmp/cs3560cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs3560cli-0.1.0.tar", last modified: Tue Mar 14 17:05:18 2023, max compression
+gzip compressed data, was "cs3560cli-0.1.2.tar", last modified: Tue Apr 18 16:16:00 2023, max compression
```

## Comparing `cs3560cli-0.1.0.tar` & `cs3560cli-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwx------   0 kiwi      (1000) kiwi      (1000)        0 2023-03-14 17:05:18.237019 cs3560cli-0.1.0/
--rw-------   0 kiwi      (1000) kiwi      (1000)     1066 2023-03-14 16:14:33.000000 cs3560cli-0.1.0/LICENSE
--rw-------   0 kiwi      (1000) kiwi      (1000)       75 2023-03-14 17:05:18.237019 cs3560cli-0.1.0/PKG-INFO
--rw-------   0 kiwi      (1000) kiwi      (1000)      179 2023-03-14 17:04:57.000000 cs3560cli-0.1.0/README.md
-drwx------   0 kiwi      (1000) kiwi      (1000)        0 2023-03-14 17:05:18.233685 cs3560cli-0.1.0/cs3560cli/
--rw-r--r--   0 kiwi      (1000) kiwi      (1000)        0 2023-03-14 16:36:58.000000 cs3560cli-0.1.0/cs3560cli/__init__.py
--rw-r--r--   0 kiwi      (1000) kiwi      (1000)       59 2023-03-14 17:01:12.000000 cs3560cli-0.1.0/cs3560cli/__main__.py
-drwx------   0 kiwi      (1000) kiwi      (1000)        0 2023-03-14 17:05:18.237019 cs3560cli-0.1.0/cs3560cli/functions/
--rw-r--r--   0 kiwi      (1000) kiwi      (1000)     2266 2023-03-14 16:43:12.000000 cs3560cli-0.1.0/cs3560cli/functions/check_username.py
--rw-r--r--   0 kiwi      (1000) kiwi      (1000)     3261 2023-03-14 16:47:08.000000 cs3560cli-0.1.0/cs3560cli/functions/watch_zip.py
--rw-r--r--   0 kiwi      (1000) kiwi      (1000)      243 2023-03-14 17:01:19.000000 cs3560cli-0.1.0/cs3560cli/main.py
-drwx------   0 kiwi      (1000) kiwi      (1000)        0 2023-03-14 17:05:18.233685 cs3560cli-0.1.0/cs3560cli.egg-info/
--rw-------   0 kiwi      (1000) kiwi      (1000)       75 2023-03-14 17:05:18.000000 cs3560cli-0.1.0/cs3560cli.egg-info/PKG-INFO
--rw-------   0 kiwi      (1000) kiwi      (1000)      365 2023-03-14 17:05:18.000000 cs3560cli-0.1.0/cs3560cli.egg-info/SOURCES.txt
--rw-------   0 kiwi      (1000) kiwi      (1000)        1 2023-03-14 17:05:18.000000 cs3560cli-0.1.0/cs3560cli.egg-info/dependency_links.txt
--rw-------   0 kiwi      (1000) kiwi      (1000)       57 2023-03-14 17:05:18.000000 cs3560cli-0.1.0/cs3560cli.egg-info/entry_points.txt
--rw-------   0 kiwi      (1000) kiwi      (1000)       83 2023-03-14 17:05:18.000000 cs3560cli-0.1.0/cs3560cli.egg-info/requires.txt
--rw-------   0 kiwi      (1000) kiwi      (1000)       10 2023-03-14 17:05:18.000000 cs3560cli-0.1.0/cs3560cli.egg-info/top_level.txt
--rw-r--r--   0 kiwi      (1000) kiwi      (1000)      327 2023-03-14 17:02:38.000000 cs3560cli-0.1.0/pyproject.toml
--rw-------   0 kiwi      (1000) kiwi      (1000)       38 2023-03-14 17:05:18.237019 cs3560cli-0.1.0/setup.cfg
+drwx------   0 kiwi      (1000) kiwi      (1000)        0 2023-04-18 16:16:00.502906 cs3560cli-0.1.2/
+-rw-------   0 kiwi      (1000) kiwi      (1000)     1066 2023-04-18 16:14:21.000000 cs3560cli-0.1.2/LICENSE
+-rw-------   0 kiwi      (1000) kiwi      (1000)       75 2023-04-18 16:16:00.502906 cs3560cli-0.1.2/PKG-INFO
+-rw-------   0 kiwi      (1000) kiwi      (1000)      550 2023-04-18 16:14:21.000000 cs3560cli-0.1.2/README.md
+drwx------   0 kiwi      (1000) kiwi      (1000)        0 2023-04-18 16:16:00.502906 cs3560cli-0.1.2/cs3560cli/
+-rw-------   0 kiwi      (1000) kiwi      (1000)        0 2023-04-18 16:14:21.000000 cs3560cli-0.1.2/cs3560cli/__init__.py
+-rw-------   0 kiwi      (1000) kiwi      (1000)       59 2023-04-18 16:14:21.000000 cs3560cli-0.1.2/cs3560cli/__main__.py
+drwx------   0 kiwi      (1000) kiwi      (1000)        0 2023-04-18 16:16:00.502906 cs3560cli-0.1.2/cs3560cli/functions/
+-rw-------   0 kiwi      (1000) kiwi      (1000)     2266 2023-04-18 16:14:21.000000 cs3560cli-0.1.2/cs3560cli/functions/check_username.py
+-rw-------   0 kiwi      (1000) kiwi      (1000)     3636 2023-04-18 16:14:21.000000 cs3560cli-0.1.2/cs3560cli/functions/create_gitignore.py
+-rw-------   0 kiwi      (1000) kiwi      (1000)     2361 2023-04-18 16:14:21.000000 cs3560cli-0.1.2/cs3560cli/functions/highlight.py
+-rw-------   0 kiwi      (1000) kiwi      (1000)     3261 2023-04-18 16:14:21.000000 cs3560cli-0.1.2/cs3560cli/functions/watch_zip.py
+-rw-------   0 kiwi      (1000) kiwi      (1000)      404 2023-04-18 16:14:21.000000 cs3560cli-0.1.2/cs3560cli/main.py
+drwx------   0 kiwi      (1000) kiwi      (1000)        0 2023-04-18 16:16:00.502906 cs3560cli-0.1.2/cs3560cli.egg-info/
+-rw-------   0 kiwi      (1000) kiwi      (1000)       75 2023-04-18 16:16:00.000000 cs3560cli-0.1.2/cs3560cli.egg-info/PKG-INFO
+-rw-------   0 kiwi      (1000) kiwi      (1000)      438 2023-04-18 16:16:00.000000 cs3560cli-0.1.2/cs3560cli.egg-info/SOURCES.txt
+-rw-------   0 kiwi      (1000) kiwi      (1000)        1 2023-04-18 16:16:00.000000 cs3560cli-0.1.2/cs3560cli.egg-info/dependency_links.txt
+-rw-------   0 kiwi      (1000) kiwi      (1000)       49 2023-04-18 16:16:00.000000 cs3560cli-0.1.2/cs3560cli.egg-info/entry_points.txt
+-rw-------   0 kiwi      (1000) kiwi      (1000)      101 2023-04-18 16:16:00.000000 cs3560cli-0.1.2/cs3560cli.egg-info/requires.txt
+-rw-------   0 kiwi      (1000) kiwi      (1000)       10 2023-04-18 16:16:00.000000 cs3560cli-0.1.2/cs3560cli.egg-info/top_level.txt
+-rw-------   0 kiwi      (1000) kiwi      (1000)      352 2023-04-18 16:14:52.000000 cs3560cli-0.1.2/pyproject.toml
+-rw-------   0 kiwi      (1000) kiwi      (1000)       38 2023-04-18 16:16:00.502906 cs3560cli-0.1.2/setup.cfg
```

### Comparing `cs3560cli-0.1.0/LICENSE` & `cs3560cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cs3560cli-0.1.0/cs3560cli/functions/check_username.py` & `cs3560cli-0.1.2/cs3560cli/functions/check_username.py`

 * *Files identical despite different names*

### Comparing `cs3560cli-0.1.0/cs3560cli/functions/watch_zip.py` & `cs3560cli-0.1.2/cs3560cli/functions/watch_zip.py`

 * *Files identical despite different names*

