# Comparing `tmp/torquepy-0.3.tar.gz` & `tmp/torquepy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torquepy-0.3.tar", last modified: Tue Apr 18 11:47:49 2023, max compression
+gzip compressed data, was "torquepy-0.3.1.tar", last modified: Tue Apr 18 11:57:33 2023, max compression
```

## Comparing `torquepy-0.3.tar` & `torquepy-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
-drwxrwxr-x   0 semenpc   (1000) semenpc   (1000)        0 2023-04-18 11:47:49.423993 torquepy-0.3/
--rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      205 2023-04-18 11:47:49.423993 torquepy-0.3/PKG-INFO
--rw-rw-r--   0 semenpc   (1000) semenpc   (1000)       38 2023-04-18 11:47:49.423993 torquepy-0.3/setup.cfg
--rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      226 2023-04-18 11:47:46.000000 torquepy-0.3/setup.py
-drwxrwxr-x   0 semenpc   (1000) semenpc   (1000)        0 2023-04-18 11:47:49.423993 torquepy-0.3/torquepy.egg-info/
--rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      205 2023-04-18 11:47:49.000000 torquepy-0.3/torquepy.egg-info/PKG-INFO
--rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      136 2023-04-18 11:47:49.000000 torquepy-0.3/torquepy.egg-info/SOURCES.txt
--rw-rw-r--   0 semenpc   (1000) semenpc   (1000)        1 2023-04-18 11:47:49.000000 torquepy-0.3/torquepy.egg-info/dependency_links.txt
--rw-rw-r--   0 semenpc   (1000) semenpc   (1000)        1 2023-04-18 11:47:49.000000 torquepy-0.3/torquepy.egg-info/top_level.txt
+drwxrwxr-x   0 semenpc   (1000) semenpc   (1000)        0 2023-04-18 11:57:33.383991 torquepy-0.3.1/
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      207 2023-04-18 11:57:33.383991 torquepy-0.3.1/PKG-INFO
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)       38 2023-04-18 11:57:33.383991 torquepy-0.3.1/setup.cfg
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      225 2023-04-18 11:57:30.000000 torquepy-0.3.1/setup.py
+drwxrwxr-x   0 semenpc   (1000) semenpc   (1000)        0 2023-04-18 11:57:33.383991 torquepy-0.3.1/torquepy/
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)     3449 2023-04-18 11:22:45.000000 torquepy-0.3.1/torquepy/torquepy.py
+drwxrwxr-x   0 semenpc   (1000) semenpc   (1000)        0 2023-04-18 11:57:33.383991 torquepy-0.3.1/torquepy.egg-info/
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      207 2023-04-18 11:57:33.000000 torquepy-0.3.1/torquepy.egg-info/PKG-INFO
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)      157 2023-04-18 11:57:33.000000 torquepy-0.3.1/torquepy.egg-info/SOURCES.txt
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)        1 2023-04-18 11:57:33.000000 torquepy-0.3.1/torquepy.egg-info/dependency_links.txt
+-rw-rw-r--   0 semenpc   (1000) semenpc   (1000)        9 2023-04-18 11:57:33.000000 torquepy-0.3.1/torquepy.egg-info/top_level.txt
```

