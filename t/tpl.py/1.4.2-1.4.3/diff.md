# Comparing `tmp/tpl.py-1.4.2.tar.gz` & `tmp/tpl.py-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpl.py-1.4.2.tar", last modified: Tue Apr 18 18:21:09 2023, max compression
+gzip compressed data, was "tpl.py-1.4.3.tar", last modified: Tue Apr 18 18:31:21 2023, max compression
```

## Comparing `tpl.py-1.4.2.tar` & `tpl.py-1.4.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:21:09.216499 tpl.py-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 18:20:59.000000 tpl.py-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-18 18:20:59.000000 tpl.py-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 18:21:09.216499 tpl.py-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-04-18 18:20:59.000000 tpl.py-1.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 18:20:59.000000 tpl.py-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 18:21:09.216499 tpl.py-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-18 18:20:59.000000 tpl.py-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:21:09.216499 tpl.py-1.4.2/template_py/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-18 18:20:59.000000 tpl.py-1.4.2/template_py/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8027 2023-04-18 18:20:59.000000 tpl.py-1.4.2/template_py/template_py.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:21:09.216499 tpl.py-1.4.2/tpl.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 18:21:09.000000 tpl.py-1.4.2/tpl.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-18 18:21:09.000000 tpl.py-1.4.2/tpl.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:21:09.000000 tpl.py-1.4.2/tpl.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-18 18:21:09.000000 tpl.py-1.4.2/tpl.py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 18:21:09.000000 tpl.py-1.4.2/tpl.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 18:21:09.000000 tpl.py-1.4.2/tpl.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:31:21.090939 tpl.py-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 18:31:11.000000 tpl.py-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-18 18:31:11.000000 tpl.py-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 18:31:21.090939 tpl.py-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-04-18 18:31:11.000000 tpl.py-1.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 18:31:11.000000 tpl.py-1.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 18:31:21.090939 tpl.py-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-18 18:31:11.000000 tpl.py-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:31:21.090939 tpl.py-1.4.3/template_py/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-18 18:31:11.000000 tpl.py-1.4.3/template_py/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8027 2023-04-18 18:31:11.000000 tpl.py-1.4.3/template_py/template_py.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:31:21.090939 tpl.py-1.4.3/tpl.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 18:31:21.000000 tpl.py-1.4.3/tpl.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-18 18:31:21.000000 tpl.py-1.4.3/tpl.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:31:21.000000 tpl.py-1.4.3/tpl.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-18 18:31:21.000000 tpl.py-1.4.3/tpl.py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 18:31:21.000000 tpl.py-1.4.3/tpl.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 18:31:21.000000 tpl.py-1.4.3/tpl.py.egg-info/top_level.txt
```

### Comparing `tpl.py-1.4.2/LICENSE` & `tpl.py-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tpl.py-1.4.2/README.md` & `tpl.py-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `tpl.py-1.4.2/template_py/template_py.py` & `tpl.py-1.4.3/template_py/template_py.py`

 * *Files identical despite different names*

