# Comparing `tmp/pythoncoloringslibV2-1.0.0.tar.gz` & `tmp/pythoncoloringslibV2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncoloringslibV2-1.0.0.tar", last modified: Mon Apr 17 17:19:11 2023, max compression
+gzip compressed data, was "pythoncoloringslibV2-2.0.0.tar", last modified: Tue Apr 18 18:58:46 2023, max compression
```

## Comparing `pythoncoloringslibV2-1.0.0.tar` & `pythoncoloringslibV2-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 17:19:11.529605 pythoncoloringslibV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      328 2023-04-17 17:19:11.529605 pythoncoloringslibV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 17:19:11.529605 pythoncoloringslibV2-1.0.0/pythoncoloringslibV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-17 17:19:11.000000 pythoncoloringslibV2-1.0.0/pythoncoloringslibV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 17:19:11.529605 pythoncoloringslibV2-1.0.0/pythoncoloringslibV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      328 2023-04-17 17:19:11.000000 pythoncoloringslibV2-1.0.0/pythoncoloringslibV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2023-04-17 17:19:11.000000 pythoncoloringslibV2-1.0.0/pythoncoloringslibV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 17:19:11.000000 pythoncoloringslibV2-1.0.0/pythoncoloringslibV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-17 17:19:11.000000 pythoncoloringslibV2-1.0.0/pythoncoloringslibV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 17:19:11.529605 pythoncoloringslibV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      541 2023-04-17 17:19:10.000000 pythoncoloringslibV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 18:58:46.307633 pythoncoloringslibV2-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      407 2023-04-18 18:58:46.307633 pythoncoloringslibV2-2.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 18:58:46.307633 pythoncoloringslibV2-2.0.0/pythoncoloringslibV2/
+-rw-r--r--   0 root         (0) root         (0)    70957 2023-04-18 18:58:45.000000 pythoncoloringslibV2-2.0.0/pythoncoloringslibV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 18:58:46.307633 pythoncoloringslibV2-2.0.0/pythoncoloringslibV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      407 2023-04-18 18:58:46.000000 pythoncoloringslibV2-2.0.0/pythoncoloringslibV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-04-18 18:58:46.000000 pythoncoloringslibV2-2.0.0/pythoncoloringslibV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 18:58:46.000000 pythoncoloringslibV2-2.0.0/pythoncoloringslibV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-18 18:58:46.000000 pythoncoloringslibV2-2.0.0/pythoncoloringslibV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 18:58:46.307633 pythoncoloringslibV2-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      620 2023-04-18 18:58:45.000000 pythoncoloringslibV2-2.0.0/setup.py
```

