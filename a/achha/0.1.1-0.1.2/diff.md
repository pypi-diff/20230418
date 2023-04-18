# Comparing `tmp/achha-0.1.1.tar.gz` & `tmp/achha-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "achha-0.1.1.tar", last modified: Tue Apr 18 06:16:29 2023, max compression
+gzip compressed data, was "achha-0.1.2.tar", last modified: Tue Apr 18 06:20:45 2023, max compression
```

## Comparing `achha-0.1.1.tar` & `achha-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-04-18 06:16:29.626760 achha-0.1.1/
--rw-rw-r--   0 amit      (1000) amit      (1000)      154 2023-04-18 06:16:29.626760 achha-0.1.1/PKG-INFO
-drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-04-18 06:16:29.622760 achha-0.1.1/Plugin1/
--rw-rw-r--   0 amit      (1000) amit      (1000)        0 2023-04-18 05:15:52.000000 achha-0.1.1/Plugin1/__init__.py
--rw-rw-r--   0 amit      (1000) amit      (1000)        0 2023-04-18 05:15:58.000000 achha-0.1.1/Plugin1/main.py
-drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-04-18 06:16:29.626760 achha-0.1.1/achha.egg-info/
--rw-rw-r--   0 amit      (1000) amit      (1000)      154 2023-04-18 06:16:29.000000 achha-0.1.1/achha.egg-info/PKG-INFO
--rw-rw-r--   0 amit      (1000) amit      (1000)      192 2023-04-18 06:16:29.000000 achha-0.1.1/achha.egg-info/SOURCES.txt
--rw-rw-r--   0 amit      (1000) amit      (1000)        1 2023-04-18 06:16:29.000000 achha-0.1.1/achha.egg-info/dependency_links.txt
--rw-rw-r--   0 amit      (1000) amit      (1000)       55 2023-04-18 06:16:29.000000 achha-0.1.1/achha.egg-info/entry_points.txt
--rw-rw-r--   0 amit      (1000) amit      (1000)        8 2023-04-18 06:16:29.000000 achha-0.1.1/achha.egg-info/top_level.txt
--rw-rw-r--   0 amit      (1000) amit      (1000)       38 2023-04-18 06:16:29.626760 achha-0.1.1/setup.cfg
--rw-rw-r--   0 amit      (1000) amit      (1000)      380 2023-04-18 06:16:26.000000 achha-0.1.1/setup.py
+drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-04-18 06:20:45.286767 achha-0.1.2/
+-rw-rw-r--   0 amit      (1000) amit      (1000)      154 2023-04-18 06:20:45.286767 achha-0.1.2/PKG-INFO
+drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-04-18 06:20:45.282767 achha-0.1.2/Plugin1/
+-rw-rw-r--   0 amit      (1000) amit      (1000)       29 2023-04-18 06:19:57.000000 achha-0.1.2/Plugin1/__init__.py
+-rw-rw-r--   0 amit      (1000) amit      (1000)        0 2023-04-18 05:15:58.000000 achha-0.1.2/Plugin1/main.py
+drwxrwxr-x   0 amit      (1000) amit      (1000)        0 2023-04-18 06:20:45.286767 achha-0.1.2/achha.egg-info/
+-rw-rw-r--   0 amit      (1000) amit      (1000)      154 2023-04-18 06:20:45.000000 achha-0.1.2/achha.egg-info/PKG-INFO
+-rw-rw-r--   0 amit      (1000) amit      (1000)      192 2023-04-18 06:20:45.000000 achha-0.1.2/achha.egg-info/SOURCES.txt
+-rw-rw-r--   0 amit      (1000) amit      (1000)        1 2023-04-18 06:20:45.000000 achha-0.1.2/achha.egg-info/dependency_links.txt
+-rw-rw-r--   0 amit      (1000) amit      (1000)       55 2023-04-18 06:20:45.000000 achha-0.1.2/achha.egg-info/entry_points.txt
+-rw-rw-r--   0 amit      (1000) amit      (1000)        8 2023-04-18 06:20:45.000000 achha-0.1.2/achha.egg-info/top_level.txt
+-rw-rw-r--   0 amit      (1000) amit      (1000)       38 2023-04-18 06:20:45.286767 achha-0.1.2/setup.cfg
+-rw-rw-r--   0 amit      (1000) amit      (1000)      380 2023-04-18 06:20:36.000000 achha-0.1.2/setup.py
```

