# Comparing `tmp/reddit_etl_abd-0.0.4.tar.gz` & `tmp/reddit_etl_abd-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit_etl_abd-0.0.4.tar", last modified: Fri Apr 14 15:58:00 2023, max compression
+gzip compressed data, was "reddit_etl_abd-0.0.5.tar", last modified: Tue Apr 18 07:06:36 2023, max compression
```

## Comparing `reddit_etl_abd-0.0.4.tar` & `reddit_etl_abd-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 15:58:00.847942 reddit_etl_abd-0.0.4/
--rw-rw-rw-   0        0        0     1077 2023-04-14 10:29:02.000000 reddit_etl_abd-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      373 2023-04-14 15:58:00.840376 reddit_etl_abd-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-14 10:28:34.000000 reddit_etl_abd-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 15:58:00.790874 reddit_etl_abd-0.0.4/extract/
--rw-rw-rw-   0        0        0        0 2023-04-14 06:09:48.000000 reddit_etl_abd-0.0.4/extract/__init__.py
--rw-rw-rw-   0        0        0      807 2023-04-14 13:32:22.000000 reddit_etl_abd-0.0.4/extract/data_ingestion.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:58:00.799045 reddit_etl_abd-0.0.4/includes/
--rw-rw-rw-   0        0        0        0 2023-04-14 07:54:10.000000 reddit_etl_abd-0.0.4/includes/__init__.py
--rw-rw-rw-   0        0        0     2350 2023-04-14 13:32:40.000000 reddit_etl_abd-0.0.4/includes/functions.py
--rw-rw-rw-   0        0        0      441 2023-04-14 10:55:13.000000 reddit_etl_abd-0.0.4/includes/vars.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:58:00.799045 reddit_etl_abd-0.0.4/load/
--rw-rw-rw-   0        0        0        0 2023-04-14 12:46:27.000000 reddit_etl_abd-0.0.4/load/__init__.py
--rw-rw-rw-   0        0        0      949 2023-04-14 13:33:43.000000 reddit_etl_abd-0.0.4/load/load_author_flair.py
--rw-rw-rw-   0        0        0      937 2023-04-14 13:34:12.000000 reddit_etl_abd-0.0.4/load/load_awardings.py
--rw-rw-rw-   0        0        0      933 2023-04-14 13:34:35.000000 reddit_etl_abd-0.0.4/load/load_gildings.py
--rw-rw-rw-   0        0        0      929 2023-04-14 13:34:52.000000 reddit_etl_abd-0.0.4/load/load_popular.py
--rw-rw-rw-   0        0        0      465 2023-04-14 15:57:23.000000 reddit_etl_abd-0.0.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-14 15:58:00.831548 reddit_etl_abd-0.0.4/reddit_etl_abd.egg-info/
--rw-rw-rw-   0        0        0      373 2023-04-14 15:58:00.000000 reddit_etl_abd-0.0.4/reddit_etl_abd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-04-14 15:58:00.000000 reddit_etl_abd-0.0.4/reddit_etl_abd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 15:58:00.000000 reddit_etl_abd-0.0.4/reddit_etl_abd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-14 15:58:00.000000 reddit_etl_abd-0.0.4/reddit_etl_abd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 15:58:00.847942 reddit_etl_abd-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 15:58:00.840376 reddit_etl_abd-0.0.4/transform/
--rw-rw-rw-   0        0        0        0 2023-04-14 12:46:37.000000 reddit_etl_abd-0.0.4/transform/__init__.py
--rw-rw-rw-   0        0        0     2403 2023-04-14 13:35:17.000000 reddit_etl_abd-0.0.4/transform/transform_author_flair.py
--rw-rw-rw-   0        0        0     1896 2023-04-14 13:35:38.000000 reddit_etl_abd-0.0.4/transform/transform_awardings.py
--rw-rw-rw-   0        0        0     1546 2023-04-14 13:35:53.000000 reddit_etl_abd-0.0.4/transform/transform_gildings.py
--rw-rw-rw-   0        0        0     1802 2023-04-14 13:36:13.000000 reddit_etl_abd-0.0.4/transform/transform_popular.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:06:36.987714 reddit_etl_abd-0.0.5/
+-rw-rw-rw-   0        0        0     1077 2023-04-14 10:29:02.000000 reddit_etl_abd-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      372 2023-04-18 07:06:36.987714 reddit_etl_abd-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       65 2023-04-14 18:11:43.000000 reddit_etl_abd-0.0.5/README.md
+-rw-rw-rw-   0        0        0      439 2023-04-18 07:05:56.000000 reddit_etl_abd-0.0.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-18 07:06:36.958708 reddit_etl_abd-0.0.5/reddit_etl_abd/
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:58:12.000000 reddit_etl_abd-0.0.5/reddit_etl_abd/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:06:36.976479 reddit_etl_abd-0.0.5/reddit_etl_abd.egg-info/
+-rw-rw-rw-   0        0        0      372 2023-04-18 07:06:36.000000 reddit_etl_abd-0.0.5/reddit_etl_abd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-04-18 07:06:36.000000 reddit_etl_abd-0.0.5/reddit_etl_abd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 07:06:36.000000 reddit_etl_abd-0.0.5/reddit_etl_abd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 07:06:36.000000 reddit_etl_abd-0.0.5/reddit_etl_abd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 07:06:36.987714 reddit_etl_abd-0.0.5/setup.cfg
```

### Comparing `reddit_etl_abd-0.0.4/LICENSE` & `reddit_etl_abd-0.0.5/LICENSE`

 * *Files identical despite different names*

