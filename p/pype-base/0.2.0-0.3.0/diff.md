# Comparing `tmp/pype-base-0.2.0.tar.gz` & `tmp/pype-base-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pype-base-0.2.0.tar", last modified: Fri Jan 20 12:14:33 2023, max compression
+gzip compressed data, was "pype-base-0.3.0.tar", last modified: Tue Apr 18 07:35:36 2023, max compression
```

## Comparing `pype-base-0.2.0.tar` & `pype-base-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:14:33.642339 pype-base-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-20 12:14:33.642339 pype-base-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 12:14:33.642339 pype-base-0.2.0/pype_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-20 12:14:33.000000 pype-base-0.2.0/pype_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-01-20 12:14:33.000000 pype-base-0.2.0/pype_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 12:14:33.000000 pype-base-0.2.0/pype_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-01-20 12:14:33.000000 pype-base-0.2.0/pype_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 12:14:33.000000 pype-base-0.2.0/pype_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 12:14:33.642339 pype-base-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-01-20 12:11:52.000000 pype-base-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:35:36.086322 pype-base-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-18 07:35:36.086322 pype-base-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:35:36.086322 pype-base-0.3.0/pype_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-18 07:35:36.000000 pype-base-0.3.0/pype_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-18 07:35:36.000000 pype-base-0.3.0/pype_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:35:36.000000 pype-base-0.3.0/pype_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-18 07:35:36.000000 pype-base-0.3.0/pype_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:35:36.000000 pype-base-0.3.0/pype_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:35:36.086322 pype-base-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-18 07:32:59.000000 pype-base-0.3.0/setup.py
```

