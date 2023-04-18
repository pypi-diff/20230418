# Comparing `tmp/jaquar-0.4.tar.gz` & `tmp/jaquar-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jaquar-0.4.tar", last modified: Tue Apr 18 08:22:11 2023, max compression
+gzip compressed data, was "dist\jaquar-0.5.0.tar", last modified: Tue Apr 18 08:26:58 2023, max compression
```

## Comparing `jaquar-0.4.tar` & `jaquar-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 08:22:11.000000 jaquar-0.4/
-drwxrwxrwx   0        0        0        0 2023-04-18 08:22:11.000000 jaquar-0.4/jaquar/
--rw-rw-rw-   0        0        0     3634 2023-04-18 08:21:35.000000 jaquar-0.4/jaquar/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:22:11.000000 jaquar-0.4/jaquar/config/
--rw-rw-rw-   0        0        0      359 2023-04-17 22:48:29.000000 jaquar-0.4/jaquar/config/settings.py
--rw-rw-rw-   0        0        0      275 2023-04-17 23:55:51.000000 jaquar-0.4/jaquar/config/urls.py
--rw-rw-rw-   0        0        0        0 2023-04-17 21:11:17.000000 jaquar-0.4/jaquar/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:22:11.000000 jaquar-0.4/jaquar/db/
-drwxrwxrwx   0        0        0        0 2023-04-18 08:22:11.000000 jaquar-0.4/jaquar/db/migrations/
--rw-rw-rw-   0        0        0        2 2023-04-17 23:14:35.000000 jaquar-0.4/jaquar/db/migrations/migration.py
--rw-rw-rw-   0        0        0        0 2023-04-17 21:35:25.000000 jaquar-0.4/jaquar/db/migrations/__init__.py
--rw-rw-rw-   0        0        0      498 2023-04-17 21:43:43.000000 jaquar-0.4/jaquar/db/schema.py
--rw-rw-rw-   0        0        0        0 2023-04-17 21:35:07.000000 jaquar-0.4/jaquar/db/__init__.py
--rw-rw-rw-   0        0        0     2556 2023-04-18 08:01:12.000000 jaquar-0.4/jaquar/jq.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:22:11.000000 jaquar-0.4/jaquar/models/
--rw-rw-rw-   0        0        0      994 2023-04-18 06:13:22.000000 jaquar-0.4/jaquar/models/models.py
--rw-rw-rw-   0        0        0        0 2023-04-18 06:06:34.000000 jaquar-0.4/jaquar/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:22:11.000000 jaquar-0.4/jaquar/views/
--rw-rw-rw-   0        0        0       37 2023-04-17 22:14:58.000000 jaquar-0.4/jaquar/views/about.py
--rw-rw-rw-   0        0        0       53 2023-04-17 22:14:25.000000 jaquar-0.4/jaquar/views/contact.py
--rw-rw-rw-   0        0        0     1290 2023-04-17 23:55:42.000000 jaquar-0.4/jaquar/views/home.py
--rw-rw-rw-   0        0        0        0 2023-04-17 21:11:21.000000 jaquar-0.4/jaquar/views/__init__.py
--rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.4/jaquar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 08:22:11.000000 jaquar-0.4/jaquar.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-18 08:22:11.000000 jaquar-0.4/jaquar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-04-18 08:22:11.000000 jaquar-0.4/jaquar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      232 2023-04-18 08:22:11.000000 jaquar-0.4/jaquar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-04-18 08:22:11.000000 jaquar-0.4/jaquar.egg-info/requires.txt
--rw-rw-rw-   0        0        0      573 2023-04-18 08:22:11.000000 jaquar-0.4/jaquar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 08:22:11.000000 jaquar-0.4/jaquar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       99 2023-04-18 06:04:11.000000 jaquar-0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      232 2023-04-18 08:22:11.000000 jaquar-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-18 08:22:11.000000 jaquar-0.4/setup.cfg
--rw-rw-rw-   0        0        0      467 2023-04-18 08:22:09.000000 jaquar-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/
+drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/jaquar/
+-rw-rw-rw-   0        0        0     3634 2023-04-18 08:21:35.000000 jaquar-0.5.0/jaquar/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/jaquar/config/
+-rw-rw-rw-   0        0        0      359 2023-04-17 22:48:29.000000 jaquar-0.5.0/jaquar/config/settings.py
+-rw-rw-rw-   0        0        0      275 2023-04-17 23:55:51.000000 jaquar-0.5.0/jaquar/config/urls.py
+-rw-rw-rw-   0        0        0        0 2023-04-17 21:11:17.000000 jaquar-0.5.0/jaquar/config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/jaquar/db/
+drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/jaquar/db/migrations/
+-rw-rw-rw-   0        0        0        2 2023-04-17 23:14:35.000000 jaquar-0.5.0/jaquar/db/migrations/migration.py
+-rw-rw-rw-   0        0        0        0 2023-04-17 21:35:25.000000 jaquar-0.5.0/jaquar/db/migrations/__init__.py
+-rw-rw-rw-   0        0        0      498 2023-04-17 21:43:43.000000 jaquar-0.5.0/jaquar/db/schema.py
+-rw-rw-rw-   0        0        0        0 2023-04-17 21:35:07.000000 jaquar-0.5.0/jaquar/db/__init__.py
+-rw-rw-rw-   0        0        0     2556 2023-04-18 08:01:12.000000 jaquar-0.5.0/jaquar/jq.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/jaquar/models/
+-rw-rw-rw-   0        0        0      994 2023-04-18 06:13:22.000000 jaquar-0.5.0/jaquar/models/models.py
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:06:34.000000 jaquar-0.5.0/jaquar/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/jaquar/views/
+-rw-rw-rw-   0        0        0       37 2023-04-17 22:14:58.000000 jaquar-0.5.0/jaquar/views/about.py
+-rw-rw-rw-   0        0        0       53 2023-04-17 22:14:25.000000 jaquar-0.5.0/jaquar/views/contact.py
+-rw-rw-rw-   0        0        0     1290 2023-04-17 23:55:42.000000 jaquar-0.5.0/jaquar/views/home.py
+-rw-rw-rw-   0        0        0        0 2023-04-17 21:11:21.000000 jaquar-0.5.0/jaquar/views/__init__.py
+-rw-rw-rw-   0        0        0       43 2023-04-18 08:14:51.000000 jaquar-0.5.0/jaquar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:26:58.000000 jaquar-0.5.0/jaquar.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-18 08:26:57.000000 jaquar-0.5.0/jaquar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 08:26:57.000000 jaquar-0.5.0/jaquar.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2023-04-18 08:26:57.000000 jaquar-0.5.0/jaquar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-04-18 08:26:57.000000 jaquar-0.5.0/jaquar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      573 2023-04-18 08:26:57.000000 jaquar-0.5.0/jaquar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 08:26:57.000000 jaquar-0.5.0/jaquar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       99 2023-04-18 06:04:11.000000 jaquar-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      234 2023-04-18 08:26:58.000000 jaquar-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-04-18 08:26:58.000000 jaquar-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      473 2023-04-18 08:26:20.000000 jaquar-0.5.0/setup.py
```

### Comparing `jaquar-0.4/jaquar/cli.py` & `jaquar-0.5.0/jaquar/cli.py`

 * *Files identical despite different names*

### Comparing `jaquar-0.4/jaquar/jq.py` & `jaquar-0.5.0/jaquar/jq.py`

 * *Files identical despite different names*

### Comparing `jaquar-0.4/jaquar/models/models.py` & `jaquar-0.5.0/jaquar/models/models.py`

 * *Files identical despite different names*

### Comparing `jaquar-0.4/jaquar/views/home.py` & `jaquar-0.5.0/jaquar/views/home.py`

 * *Files identical despite different names*

### Comparing `jaquar-0.4/jaquar.egg-info/SOURCES.txt` & `jaquar-0.5.0/jaquar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

