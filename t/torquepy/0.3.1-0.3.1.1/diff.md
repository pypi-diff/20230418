# Comparing `tmp/torquepy-0.3.1.tar.gz` & `tmp/torquepy-0.3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torquepy-0.3.1.tar", last modified: Tue Apr 18 11:57:33 2023, max compression
+gzip compressed data, was "torquepy-0.3.1.1.tar", last modified: Tue Apr 18 12:21:01 2023, max compression
```

## Comparing `torquepy-0.3.1.tar` & `torquepy-0.3.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxr-x   0 semenpc   (1000) semenpc   (1000)        0 2023-04-18 11:57:33.383991 torquepy-0.3.1/
--rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      207 2023-04-18 11:57:33.383991 torquepy-0.3.1/PKG-INFO
--rw-rw-r--   0 semenpc   (1000) semenpc   (1000)       38 2023-04-18 11:57:33.383991 torquepy-0.3.1/setup.cfg
--rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      225 2023-04-18 11:57:30.000000 torquepy-0.3.1/setup.py
-drwxrwxr-x   0 semenpc   (1000) semenpc   (1000)        0 2023-04-18 11:57:33.383991 torquepy-0.3.1/torquepy/
--rw-rw-r--   0 semenpc   (1000) semenpc   (1000)     3449 2023-04-18 11:22:45.000000 torquepy-0.3.1/torquepy/torquepy.py
-drwxrwxr-x   0 semenpc   (1000) semenpc   (1000)        0 2023-04-18 11:57:33.383991 torquepy-0.3.1/torquepy.egg-info/
--rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      207 2023-04-18 11:57:33.000000 torquepy-0.3.1/torquepy.egg-info/PKG-INFO
--rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      157 2023-04-18 11:57:33.000000 torquepy-0.3.1/torquepy.egg-info/SOURCES.txt
--rw-rw-r--   0 semenpc   (1000) semenpc   (1000)        1 2023-04-18 11:57:33.000000 torquepy-0.3.1/torquepy.egg-info/dependency_links.txt
--rw-rw-r--   0 semenpc   (1000) semenpc   (1000)        9 2023-04-18 11:57:33.000000 torquepy-0.3.1/torquepy.egg-info/top_level.txt
+drwxrwxr-x   0 semenpc   (1000) semenpc   (1000)        0 2023-04-18 12:21:01.935986 torquepy-0.3.1.1/
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      209 2023-04-18 12:21:01.935986 torquepy-0.3.1.1/PKG-INFO
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)       38 2023-04-18 12:21:01.935986 torquepy-0.3.1.1/setup.cfg
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      231 2023-04-18 12:20:55.000000 torquepy-0.3.1.1/setup.py
+drwxrwxr-x   0 semenpc   (1000) semenpc   (1000)        0 2023-04-18 12:21:01.935986 torquepy-0.3.1.1/torquepy/
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)       36 2023-04-18 12:20:30.000000 torquepy-0.3.1.1/torquepy/__init__.py
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)     3449 2023-04-18 12:01:54.000000 torquepy-0.3.1.1/torquepy/torquepy.py
+drwxrwxr-x   0 semenpc   (1000) semenpc   (1000)        0 2023-04-18 12:21:01.935986 torquepy-0.3.1.1/torquepy.egg-info/
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      209 2023-04-18 12:21:01.000000 torquepy-0.3.1.1/torquepy.egg-info/PKG-INFO
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      178 2023-04-18 12:21:01.000000 torquepy-0.3.1.1/torquepy.egg-info/SOURCES.txt
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)        1 2023-04-18 12:21:01.000000 torquepy-0.3.1.1/torquepy.egg-info/dependency_links.txt
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)        9 2023-04-18 12:21:01.000000 torquepy-0.3.1.1/torquepy.egg-info/top_level.txt
```

### Comparing `torquepy-0.3.1/torquepy/torquepy.py` & `torquepy-0.3.1.1/torquepy/torquepy.py`

 * *Files identical despite different names*

