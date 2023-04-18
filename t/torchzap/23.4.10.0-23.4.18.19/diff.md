# Comparing `tmp/torchzap-23.4.10.0.tar.gz` & `tmp/torchzap-23.4.18.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchzap-23.4.10.0.tar", last modified: Mon Apr 10 00:21:46 2023, max compression
+gzip compressed data, was "dist/torchzap-23.4.18.19.tar", last modified: Tue Apr 18 11:46:24 2023, max compression
```

## Comparing `torchzap-23.4.10.0.tar` & `torchzap-23.4.18.19.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:21:46.882202 torchzap-23.4.10.0/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-10 00:21:46.882202 torchzap-23.4.10.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 00:21:29.000000 torchzap-23.4.10.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 00:21:46.882202 torchzap-23.4.10.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-10 00:21:29.000000 torchzap-23.4.10.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:21:46.882202 torchzap-23.4.10.0/torchzap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 00:21:29.000000 torchzap-23.4.10.0/torchzap/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-04-10 00:21:29.000000 torchzap-23.4.10.0/torchzap/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-10 00:21:29.000000 torchzap-23.4.10.0/torchzap/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:21:46.882202 torchzap-23.4.10.0/torchzap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-10 00:21:46.000000 torchzap-23.4.10.0/torchzap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-10 00:21:46.000000 torchzap-23.4.10.0/torchzap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 00:21:46.000000 torchzap-23.4.10.0/torchzap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-10 00:21:46.000000 torchzap-23.4.10.0/torchzap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 00:21:46.000000 torchzap-23.4.10.0/torchzap.egg-info/top_level.txt
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-04-18 11:46:24.487797 torchzap-23.4.18.19/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      359 2023-04-18 11:46:24.487797 torchzap-23.4.18.19/PKG-INFO
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        5 2023-03-31 07:38:53.000000 torchzap-23.4.18.19/README.md
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       38 2023-04-18 11:46:24.487797 torchzap-23.4.18.19/setup.cfg
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      745 2023-04-10 00:14:59.000000 torchzap-23.4.18.19/setup.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-04-18 11:46:24.487797 torchzap-23.4.18.19/torchzap/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       83 2023-04-11 04:06:45.000000 torchzap-23.4.18.19/torchzap/__init__.py
+-rwxr-xr-x   0 gaoang    (1001) gaoang    (1001)      688 2023-04-03 03:12:05.000000 torchzap-23.4.18.19/torchzap/preprocessing.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     6222 2023-03-31 07:40:01.000000 torchzap-23.4.18.19/torchzap/trainer.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-04-18 11:46:24.487797 torchzap-23.4.18.19/torchzap.egg-info/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      359 2023-04-18 11:46:24.000000 torchzap-23.4.18.19/torchzap.egg-info/PKG-INFO
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      244 2023-04-18 11:46:24.000000 torchzap-23.4.18.19/torchzap.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        1 2023-04-18 11:46:24.000000 torchzap-23.4.18.19/torchzap.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       61 2023-04-18 11:46:24.000000 torchzap-23.4.18.19/torchzap.egg-info/requires.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        9 2023-04-18 11:46:24.000000 torchzap-23.4.18.19/torchzap.egg-info/top_level.txt
```

### Comparing `torchzap-23.4.10.0/setup.py` & `torchzap-23.4.18.19/setup.py`

 * *Files identical despite different names*

### Comparing `torchzap-23.4.10.0/torchzap/preprocessing.py` & `torchzap-23.4.18.19/torchzap/preprocessing.py`

 * *Files identical despite different names*

### Comparing `torchzap-23.4.10.0/torchzap/trainer.py` & `torchzap-23.4.18.19/torchzap/trainer.py`

 * *Files identical despite different names*

