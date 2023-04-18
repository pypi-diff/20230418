# Comparing `tmp/auto_archiver-0.5.5.tar.gz` & `tmp/auto_archiver-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_archiver-0.5.5.tar", last modified: Thu Mar 23 18:52:36 2023, max compression
+gzip compressed data, was "auto_archiver-0.5.6.tar", last modified: Tue Apr 18 17:51:08 2023, max compression
```

## Comparing `auto_archiver-0.5.5.tar` & `auto_archiver-0.5.6.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:52:36.658608 auto_archiver-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-03-23 18:52:36.658608 auto_archiver-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-23 18:52:36.658608 auto_archiver-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:52:36.650608 auto_archiver-0.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:52:36.650608 auto_archiver-0.5.5/src/auto_archiver/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:52:36.654608 auto_archiver-0.5.5/src/auto_archiver/archivers/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/archivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/archivers/archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/archivers/instagram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/archivers/instagram_tbot_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/archivers/telegram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/archivers/telethon_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/archivers/tiktok_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/archivers/twitter_api_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/archivers/twitter_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/archivers/vk_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/archivers/youtubedl_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/auto_auto_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:52:36.654608 auto_archiver-0.5.5/src/auto_archiver/core/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/core/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/core/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:52:36.654608 auto_archiver-0.5.5/src/auto_archiver/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/databases/console_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/databases/csv_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/databases/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/databases/gsheet_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:52:36.654608 auto_archiver-0.5.5/src/auto_archiver/enrichers/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/enrichers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/enrichers/enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/enrichers/hash_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/enrichers/screenshot_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/enrichers/thumbnail_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/enrichers/wacz_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/enrichers/wayback_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/enrichers/whisper_enricher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:52:36.654608 auto_archiver-0.5.5/src/auto_archiver/feeders/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/feeders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/feeders/cli_feeder.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/feeders/feeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/feeders/gsheet_feeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:52:36.658608 auto_archiver-0.5.5/src/auto_archiver/formatters/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/formatters/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/formatters/html_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/formatters/mute_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:52:36.658608 auto_archiver-0.5.5/src/auto_archiver/formatters/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/formatters/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/formatters/templates/html_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/formatters/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:52:36.658608 auto_archiver-0.5.5/src/auto_archiver/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/storages/gd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/storages/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/storages/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/storages/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:52:36.658608 auto_archiver-0.5.5/src/auto_archiver/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/utils/gsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/utils/gworksheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/utils/webdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-23 18:51:26.000000 auto_archiver-0.5.5/src/auto_archiver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 18:52:36.650608 auto_archiver-0.5.5/src/auto_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-03-23 18:52:36.000000 auto_archiver-0.5.5/src/auto_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-03-23 18:52:36.000000 auto_archiver-0.5.5/src/auto_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 18:52:36.000000 auto_archiver-0.5.5/src/auto_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-23 18:52:36.000000 auto_archiver-0.5.5/src/auto_archiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 18:52:36.000000 auto_archiver-0.5.5/src/auto_archiver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-23 18:52:36.000000 auto_archiver-0.5.5/src/auto_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-23 18:52:36.000000 auto_archiver-0.5.5/src/auto_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.377878 auto_archiver-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-18 17:51:08.377878 auto_archiver-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-18 17:51:08.377878 auto_archiver-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.365878 auto_archiver-0.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.369878 auto_archiver-0.5.6/src/auto_archiver/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.369878 auto_archiver-0.5.6/src/auto_archiver/archivers/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/instagram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/instagram_tbot_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/telegram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/telethon_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/tiktok_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/twitter_api_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/twitter_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/vk_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/youtubedl_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/auto_auto_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.373878 auto_archiver-0.5.6/src/auto_archiver/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/core/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/core/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.373878 auto_archiver-0.5.6/src/auto_archiver/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/databases/console_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/databases/csv_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/databases/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/databases/gsheet_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.373878 auto_archiver-0.5.6/src/auto_archiver/enrichers/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/hash_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/screenshot_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/thumbnail_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/wacz_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/wayback_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/whisper_enricher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.373878 auto_archiver-0.5.6/src/auto_archiver/feeders/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/feeders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/feeders/cli_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/feeders/feeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/feeders/gsheet_feeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.373878 auto_archiver-0.5.6/src/auto_archiver/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/formatters/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/formatters/html_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/formatters/mute_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.373878 auto_archiver-0.5.6/src/auto_archiver/formatters/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/formatters/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/formatters/templates/html_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/formatters/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.373878 auto_archiver-0.5.6/src/auto_archiver/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/storages/gd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/storages/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/storages/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/storages/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.377878 auto_archiver-0.5.6/src/auto_archiver/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/utils/gsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/utils/gworksheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/utils/webdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.369878 auto_archiver-0.5.6/src/auto_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-18 17:51:08.000000 auto_archiver-0.5.6/src/auto_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-18 17:51:08.000000 auto_archiver-0.5.6/src/auto_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:51:08.000000 auto_archiver-0.5.6/src/auto_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 17:51:08.000000 auto_archiver-0.5.6/src/auto_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:51:08.000000 auto_archiver-0.5.6/src/auto_archiver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-18 17:51:08.000000 auto_archiver-0.5.6/src/auto_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 17:51:08.000000 auto_archiver-0.5.6/src/auto_archiver.egg-info/top_level.txt
```

### Comparing `auto_archiver-0.5.5/LICENSE` & `auto_archiver-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/PKG-INFO` & `auto_archiver-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_archiver
-Version: 0.5.5
+Version: 0.5.6
 Summary: Easily archive online media content
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
 Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
 Project-URL: Bellingcat, https://www.bellingcat.com
```

### Comparing `auto_archiver-0.5.5/README.md` & `auto_archiver-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/setup.cfg` & `auto_archiver-0.5.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/archivers/archiver.py` & `auto_archiver-0.5.6/src/auto_archiver/archivers/archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/archivers/instagram_archiver.py` & `auto_archiver-0.5.6/src/auto_archiver/archivers/instagram_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/archivers/instagram_tbot_archiver.py` & `auto_archiver-0.5.6/src/auto_archiver/archivers/instagram_tbot_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/archivers/telegram_archiver.py` & `auto_archiver-0.5.6/src/auto_archiver/archivers/telegram_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/archivers/telethon_archiver.py` & `auto_archiver-0.5.6/src/auto_archiver/archivers/telethon_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/archivers/tiktok_archiver.py` & `auto_archiver-0.5.6/src/auto_archiver/archivers/tiktok_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/archivers/twitter_api_archiver.py` & `auto_archiver-0.5.6/src/auto_archiver/archivers/twitter_api_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/archivers/twitter_archiver.py` & `auto_archiver-0.5.6/src/auto_archiver/archivers/twitter_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/archivers/vk_archiver.py` & `auto_archiver-0.5.6/src/auto_archiver/archivers/vk_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/archivers/youtubedl_archiver.py` & `auto_archiver-0.5.6/src/auto_archiver/archivers/youtubedl_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/auto_auto_archive.py` & `auto_archiver-0.5.6/src/auto_archiver/auto_auto_archive.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/core/config.py` & `auto_archiver-0.5.6/src/auto_archiver/core/config.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/core/context.py` & `auto_archiver-0.5.6/src/auto_archiver/core/context.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/core/media.py` & `auto_archiver-0.5.6/src/auto_archiver/core/media.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 @dataclass
 class Media:
     filename: str
     key: str = None
     urls: List[str] = field(default_factory=list)
     properties: dict = field(default_factory=dict)
     _mimetype: str = None  # eg: image/jpeg
-    _stored: bool = field(default=False, repr=False, metadata=config(exclude=True))
+    _stored: bool = field(default=False, repr=False, metadata=config(exclude=lambda _: True)) # always exclude
 
     def store(self: Media, override_storages: List = None, url: str = "url-not-available"):
         # stores the media into the provided/available storages [Storage]
         # repeats the process for its properties, in case they have inner media themselves
         # for now it only goes down 1 level but it's easy to make it recursive if needed
         storages = override_storages or ArchivingContext.get("storages")
         if not len(storages):
```

### Comparing `auto_archiver-0.5.5/src/auto_archiver/core/metadata.py` & `auto_archiver-0.5.6/src/auto_archiver/core/metadata.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/core/orchestrator.py` & `auto_archiver-0.5.6/src/auto_archiver/core/orchestrator.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/core/step.py` & `auto_archiver-0.5.6/src/auto_archiver/core/step.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/databases/console_db.py` & `auto_archiver-0.5.6/src/auto_archiver/databases/console_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/databases/csv_db.py` & `auto_archiver-0.5.6/src/auto_archiver/databases/csv_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/databases/database.py` & `auto_archiver-0.5.6/src/auto_archiver/databases/database.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/databases/gsheet_db.py` & `auto_archiver-0.5.6/src/auto_archiver/databases/gsheet_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/enrichers/enricher.py` & `auto_archiver-0.5.6/src/auto_archiver/enrichers/enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/enrichers/hash_enricher.py` & `auto_archiver-0.5.6/src/auto_archiver/enrichers/hash_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/enrichers/screenshot_enricher.py` & `auto_archiver-0.5.6/src/auto_archiver/enrichers/screenshot_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/enrichers/thumbnail_enricher.py` & `auto_archiver-0.5.6/src/auto_archiver/enrichers/thumbnail_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/enrichers/wacz_enricher.py` & `auto_archiver-0.5.6/src/auto_archiver/enrichers/wacz_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/enrichers/wayback_enricher.py` & `auto_archiver-0.5.6/src/auto_archiver/enrichers/wayback_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/enrichers/whisper_enricher.py` & `auto_archiver-0.5.6/src/auto_archiver/enrichers/whisper_enricher.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,15 +96,27 @@
         logger.debug(f"Checked job {job_id=} with status='{j['status']}'")
         if j['status'] == "processing": return False
         elif j['status'] == "error": return f"Error: {j['meta']['error']}"
         elif j['status'] == "success":
             r_res = requests.get(f'{self.api_endpoint}/jobs/{job_id}/artifacts', headers={'Authorization': f'Bearer {self.api_key}'})
             assert r_res.status_code == 200, f"Job artifacts did not respond with 200, instead with: {r_res.status_code}"
             logger.success(r_res.json())
-            return [artifact.get("data").get("text", "") for artifact in r_res.json()]
+            result = []
+            for artifact in r_res.json():
+                subtitle = []
+                full_text = []
+                for i, d in enumerate(artifact.get("data")):
+                    subtitle.append(f"{i+1}\n{d.get('start')} --> {d.get('end')}\n{d.get('text').strip()}")
+                    full_text.append(d.get('text').strip())
+                if not len(subtitle): continue
+                result.append({
+                    "subtitle": "\n".join(subtitle),
+                    "full_text": "\n".join(full_text),
+                })
+            return result
         return False
 
     def _get_s3_storage(self) -> S3Storage:
         try:
             return next(s for s in ArchivingContext.get("storages") if s.__class__ == S3Storage)
         except:
             logger.warning("No S3Storage instance found in storages")
```

### Comparing `auto_archiver-0.5.5/src/auto_archiver/feeders/cli_feeder.py` & `auto_archiver-0.5.6/src/auto_archiver/feeders/cli_feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/feeders/feeder.py` & `auto_archiver-0.5.6/src/auto_archiver/feeders/feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/feeders/gsheet_feeder.py` & `auto_archiver-0.5.6/src/auto_archiver/feeders/gsheet_feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/formatters/formatter.py` & `auto_archiver-0.5.6/src/auto_archiver/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/formatters/html_formatter.py` & `auto_archiver-0.5.6/src/auto_archiver/formatters/html_formatter.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/formatters/templates/html_template.html` & `auto_archiver-0.5.6/src/auto_archiver/formatters/templates/html_template.html`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/formatters/templates/macros.html` & `auto_archiver-0.5.6/src/auto_archiver/formatters/templates/macros.html`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/storages/gd.py` & `auto_archiver-0.5.6/src/auto_archiver/storages/gd.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/storages/local.py` & `auto_archiver-0.5.6/src/auto_archiver/storages/local.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/storages/s3.py` & `auto_archiver-0.5.6/src/auto_archiver/storages/s3.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/storages/storage.py` & `auto_archiver-0.5.6/src/auto_archiver/storages/storage.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/utils/gsheet.py` & `auto_archiver-0.5.6/src/auto_archiver/utils/gsheet.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/utils/gworksheet.py` & `auto_archiver-0.5.6/src/auto_archiver/utils/gworksheet.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/utils/misc.py` & `auto_archiver-0.5.6/src/auto_archiver/utils/misc.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/utils/url.py` & `auto_archiver-0.5.6/src/auto_archiver/utils/url.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver/utils/webdriver.py` & `auto_archiver-0.5.6/src/auto_archiver/utils/webdriver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.5/src/auto_archiver.egg-info/PKG-INFO` & `auto_archiver-0.5.6/src/auto_archiver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-archiver
-Version: 0.5.5
+Version: 0.5.6
 Summary: Easily archive online media content
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
 Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
 Project-URL: Bellingcat, https://www.bellingcat.com
```

### Comparing `auto_archiver-0.5.5/src/auto_archiver.egg-info/SOURCES.txt` & `auto_archiver-0.5.6/src/auto_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

