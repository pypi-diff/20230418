# Comparing `tmp/real48-1.0.tar.gz` & `tmp/real48-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "real48-1.0.tar", last modified: Tue Apr 18 13:53:14 2023, max compression
+gzip compressed data, was "real48-1.2.tar", last modified: Tue Apr 18 14:10:48 2023, max compression
```

## Comparing `real48-1.0.tar` & `real48-1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-18 13:53:14.089336 real48-1.0/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       48 2023-04-18 13:53:14.085336 real48-1.0/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       94 2023-04-18 13:20:06.000000 real48-1.0/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-18 13:53:14.085336 real48-1.0/real48.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       48 2023-04-18 13:53:13.000000 real48-1.0/real48.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      154 2023-04-18 13:53:14.000000 real48-1.0/real48.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-18 13:53:13.000000 real48-1.0/real48.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        7 2023-04-18 13:53:13.000000 real48-1.0/real48.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1477 2023-04-18 13:43:49.000000 real48-1.0/real48tofloat.c
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-18 13:53:14.089336 real48-1.0/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      147 2023-04-18 13:23:53.000000 real48-1.0/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-18 14:10:48.525213 real48-1.2/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      369 2023-04-18 14:10:48.525213 real48-1.2/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      279 2023-04-18 14:06:56.000000 real48-1.2/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-18 14:10:48.525213 real48-1.2/real48.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      369 2023-04-18 14:10:48.000000 real48-1.2/real48.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      154 2023-04-18 14:10:48.000000 real48-1.2/real48.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-18 14:10:48.000000 real48-1.2/real48.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        7 2023-04-18 14:10:48.000000 real48-1.2/real48.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1477 2023-04-18 13:43:49.000000 real48-1.2/real48tofloat.c
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-18 14:10:48.525213 real48-1.2/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      244 2023-04-18 14:10:02.000000 real48-1.2/setup.py
```

### Comparing `real48-1.0/real48tofloat.c` & `real48-1.2/real48tofloat.c`

 * *Files identical despite different names*

