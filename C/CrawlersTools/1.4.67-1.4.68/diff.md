# Comparing `tmp/CrawlersTools-1.4.67.tar.gz` & `tmp/CrawlersTools-1.4.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrawlersTools-1.4.67.tar", last modified: Mon Apr 17 06:37:04 2023, max compression
+gzip compressed data, was "CrawlersTools-1.4.68.tar", last modified: Tue Apr 18 13:08:45 2023, max compression
```

## Comparing `CrawlersTools-1.4.67.tar` & `CrawlersTools-1.4.68.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:37:04.354467 CrawlersTools-1.4.67/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:37:04.350467 CrawlersTools-1.4.67/CrawlersTools/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:37:04.350467 CrawlersTools-1.4.67/CrawlersTools/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/extractors/attachment_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/extractors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/extractors/content_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/extractors/list_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:37:04.350467 CrawlersTools-1.4.67/CrawlersTools/extractors/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/extractors/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/extractors/schemas/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/extractors/time_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/extractors/title_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:37:04.350467 CrawlersTools-1.4.67/CrawlersTools/extractors/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/extractors/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/extractors/utils/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/extractors/utils/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/extractors/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/extractors/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/extractors/utils/similarity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:37:04.350467 CrawlersTools-1.4.67/CrawlersTools/js_crawler/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/js_crawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31476 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/js_crawler/font_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/js_crawler/transfer_js.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:37:04.350467 CrawlersTools-1.4.67/CrawlersTools/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/logs/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:37:04.354467 CrawlersTools-1.4.67/CrawlersTools/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/pipelines/mongo_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/pipelines/mysql_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/pipelines/redis_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:37:04.354467 CrawlersTools-1.4.67/CrawlersTools/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/preprocess/bloom_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/preprocess/time_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:37:04.354467 CrawlersTools-1.4.67/CrawlersTools/projects/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/projects/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/projects/upload_oss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:37:04.354467 CrawlersTools-1.4.67/CrawlersTools/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/requests/base_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/requests/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/requests/random_ua.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:37:04.354467 CrawlersTools-1.4.67/CrawlersTools/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/CrawlersTools/schedules/auto_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:37:04.350467 CrawlersTools-1.4.67/CrawlersTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-04-17 06:37:04.000000 CrawlersTools-1.4.67/CrawlersTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-17 06:37:04.000000 CrawlersTools-1.4.67/CrawlersTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 06:37:04.000000 CrawlersTools-1.4.67/CrawlersTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-17 06:37:04.000000 CrawlersTools-1.4.67/CrawlersTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 06:37:04.000000 CrawlersTools-1.4.67/CrawlersTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-04-17 06:37:04.354467 CrawlersTools-1.4.67/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 06:37:04.354467 CrawlersTools-1.4.67/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-17 06:36:45.000000 CrawlersTools-1.4.67/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:08:45.064883 CrawlersTools-1.4.68/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:08:45.060883 CrawlersTools-1.4.68/CrawlersTools/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:08:45.060883 CrawlersTools-1.4.68/CrawlersTools/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/extractors/attachment_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/extractors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/extractors/content_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/extractors/list_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:08:45.060883 CrawlersTools-1.4.68/CrawlersTools/extractors/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/extractors/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/extractors/schemas/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/extractors/time_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/extractors/title_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:08:45.060883 CrawlersTools-1.4.68/CrawlersTools/extractors/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/extractors/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/extractors/utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/extractors/utils/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/extractors/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/extractors/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/extractors/utils/similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:08:45.060883 CrawlersTools-1.4.68/CrawlersTools/js_crawler/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/js_crawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31476 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/js_crawler/font_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/js_crawler/transfer_js.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:08:45.060883 CrawlersTools-1.4.68/CrawlersTools/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/logs/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:08:45.060883 CrawlersTools-1.4.68/CrawlersTools/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/pipelines/mongo_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/pipelines/mysql_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/pipelines/redis_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:08:45.060883 CrawlersTools-1.4.68/CrawlersTools/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/preprocess/bloom_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/preprocess/time_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:08:45.064883 CrawlersTools-1.4.68/CrawlersTools/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/projects/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/projects/upload_oss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:08:45.064883 CrawlersTools-1.4.68/CrawlersTools/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/requests/base_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/requests/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/requests/random_ua.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:08:45.064883 CrawlersTools-1.4.68/CrawlersTools/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/CrawlersTools/schedules/auto_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:08:45.060883 CrawlersTools-1.4.68/CrawlersTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-04-18 13:08:45.000000 CrawlersTools-1.4.68/CrawlersTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-18 13:08:45.000000 CrawlersTools-1.4.68/CrawlersTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:08:45.000000 CrawlersTools-1.4.68/CrawlersTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-18 13:08:45.000000 CrawlersTools-1.4.68/CrawlersTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 13:08:45.000000 CrawlersTools-1.4.68/CrawlersTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42684 2023-04-18 13:08:45.064883 CrawlersTools-1.4.68/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 13:08:45.064883 CrawlersTools-1.4.68/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-18 13:08:33.000000 CrawlersTools-1.4.68/setup.py
```

### Comparing `CrawlersTools-1.4.67/CrawlersTools/extractors/__init__.py` & `CrawlersTools-1.4.68/CrawlersTools/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/extractors/attachment_extractor.py` & `CrawlersTools-1.4.68/CrawlersTools/extractors/attachment_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/extractors/base.py` & `CrawlersTools-1.4.68/CrawlersTools/extractors/base.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/extractors/content_extractor.py` & `CrawlersTools-1.4.68/CrawlersTools/extractors/content_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/extractors/list_extractor.py` & `CrawlersTools-1.4.68/CrawlersTools/extractors/list_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/extractors/schemas/element.py` & `CrawlersTools-1.4.68/CrawlersTools/extractors/schemas/element.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/extractors/time_extractor.py` & `CrawlersTools-1.4.68/CrawlersTools/extractors/time_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/extractors/title_extractor.py` & `CrawlersTools-1.4.68/CrawlersTools/extractors/title_extractor.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/extractors/utils/cluster.py` & `CrawlersTools-1.4.68/CrawlersTools/extractors/utils/cluster.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/extractors/utils/element.py` & `CrawlersTools-1.4.68/CrawlersTools/extractors/utils/element.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/extractors/utils/preprocess.py` & `CrawlersTools-1.4.68/CrawlersTools/extractors/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/extractors/utils/settings.py` & `CrawlersTools-1.4.68/CrawlersTools/extractors/utils/settings.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/extractors/utils/similarity.py` & `CrawlersTools-1.4.68/CrawlersTools/extractors/utils/similarity.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/js_crawler/font_decrypt.py` & `CrawlersTools-1.4.68/CrawlersTools/js_crawler/font_decrypt.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/js_crawler/transfer_js.py` & `CrawlersTools-1.4.68/CrawlersTools/js_crawler/transfer_js.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/logs/log.py` & `CrawlersTools-1.4.68/CrawlersTools/logs/log.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/pipelines/mongo_pipeline.py` & `CrawlersTools-1.4.68/CrawlersTools/pipelines/mongo_pipeline.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/pipelines/mysql_pipeline.py` & `CrawlersTools-1.4.68/CrawlersTools/pipelines/mysql_pipeline.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/pipelines/redis_pipeline.py` & `CrawlersTools-1.4.68/CrawlersTools/pipelines/redis_pipeline.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/preprocess/bloom_filter.py` & `CrawlersTools-1.4.68/CrawlersTools/preprocess/bloom_filter.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/preprocess/time_process.py` & `CrawlersTools-1.4.68/CrawlersTools/preprocess/time_process.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,16 @@
         except ValueError:
             # print(f"非时间戳格式：{string}")
             pass
 
         date = Sinan(string).parse(display_status=False).get("datetime", [""])[0].split(' ')[0]     # 错误的时分秒
         if not date:
             re_res = re.search(self.datetime_pattern, string)
-            date = f"{re_res.group(1)}-{re_res.group(2)}-{re_res.group(3)}"
+            if re_res is not None:
+                date = f"{re_res.group(1)}-{re_res.group(2)}-{re_res.group(3)}"
 
         if struct:
             return datetime.strptime(date, self.fmt)
         return date
 
     def process_timestamp(self, timestamp, struct):
         timestamp = int(str(timestamp)[:10])
@@ -46,10 +47,13 @@
 
     def compare_date(self, time_min, time_max) -> bool:
         if not (time_min and time_max):
             return False
 
         time_min_format = time_min if isinstance(time_min, datetime) else self.format(time_min, struct=True)
         time_max_format = time_max if isinstance(time_max, datetime) else self.format(time_max, struct=True)
+        if not (time_min_format and time_max_format):
+            return False
+
         if time_min_format.date() <= time_max_format.date():
             return True
         return False
```

### Comparing `CrawlersTools-1.4.67/CrawlersTools/projects/filters.py` & `CrawlersTools-1.4.68/CrawlersTools/projects/filters.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/projects/upload_oss.py` & `CrawlersTools-1.4.68/CrawlersTools/projects/upload_oss.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/requests/base_requests.py` & `CrawlersTools-1.4.68/CrawlersTools/requests/base_requests.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/requests/proxy.py` & `CrawlersTools-1.4.68/CrawlersTools/requests/proxy.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/requests/random_ua.py` & `CrawlersTools-1.4.68/CrawlersTools/requests/random_ua.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools/schedules/auto_thread.py` & `CrawlersTools-1.4.68/CrawlersTools/schedules/auto_thread.py`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/CrawlersTools.egg-info/PKG-INFO` & `CrawlersTools-1.4.68/CrawlersTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrawlersTools
-Version: 1.4.67
+Version: 1.4.68
 Summary: Tools for Crawlers
 Home-page: https://github.com/MuggleK/CrawlersTools
 Author: MuggleK
 Author-email: peichangchuan@gmail.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `CrawlersTools-1.4.67/CrawlersTools.egg-info/SOURCES.txt` & `CrawlersTools-1.4.68/CrawlersTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/LICENSE` & `CrawlersTools-1.4.68/LICENSE`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/PKG-INFO` & `CrawlersTools-1.4.68/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrawlersTools
-Version: 1.4.67
+Version: 1.4.68
 Summary: Tools for Crawlers
 Home-page: https://github.com/MuggleK/CrawlersTools
 Author: MuggleK
 Author-email: peichangchuan@gmail.com
 License: BSD License
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `CrawlersTools-1.4.67/README.md` & `CrawlersTools-1.4.68/README.md`

 * *Files identical despite different names*

### Comparing `CrawlersTools-1.4.67/setup.py` & `CrawlersTools-1.4.68/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='CrawlersTools',  # 包名
-    version='1.4.67',  # 版本号
+    version='1.4.68',  # 版本号
     description='Tools for Crawlers',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='MuggleK',
     author_email='peichangchuan@gmail.com',
     url='https://github.com/MuggleK/CrawlersTools',
     install_requires=[
```

