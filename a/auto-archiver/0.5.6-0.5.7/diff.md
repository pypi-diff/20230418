# Comparing `tmp/auto_archiver-0.5.6.tar.gz` & `tmp/auto_archiver-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_archiver-0.5.6.tar", last modified: Tue Apr 18 17:51:08 2023, max compression
+gzip compressed data, was "auto_archiver-0.5.7.tar", last modified: Tue Apr 18 18:30:57 2023, max compression
```

## Comparing `auto_archiver-0.5.6.tar` & `auto_archiver-0.5.7.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.377878 auto_archiver-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-18 17:51:08.377878 auto_archiver-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-18 17:51:08.377878 auto_archiver-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.365878 auto_archiver-0.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.369878 auto_archiver-0.5.6/src/auto_archiver/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.369878 auto_archiver-0.5.6/src/auto_archiver/archivers/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/instagram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/instagram_tbot_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/telegram_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/telethon_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/tiktok_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/twitter_api_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/twitter_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/vk_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/archivers/youtubedl_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/auto_auto_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.373878 auto_archiver-0.5.6/src/auto_archiver/core/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/core/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/core/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.373878 auto_archiver-0.5.6/src/auto_archiver/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/databases/console_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/databases/csv_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/databases/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/databases/gsheet_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.373878 auto_archiver-0.5.6/src/auto_archiver/enrichers/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/hash_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/screenshot_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/thumbnail_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/wacz_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/wayback_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/enrichers/whisper_enricher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.373878 auto_archiver-0.5.6/src/auto_archiver/feeders/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/feeders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/feeders/cli_feeder.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/feeders/feeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/feeders/gsheet_feeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.373878 auto_archiver-0.5.6/src/auto_archiver/formatters/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/formatters/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/formatters/html_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/formatters/mute_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.373878 auto_archiver-0.5.6/src/auto_archiver/formatters/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/formatters/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/formatters/templates/html_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/formatters/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.373878 auto_archiver-0.5.6/src/auto_archiver/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/storages/gd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/storages/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/storages/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/storages/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.377878 auto_archiver-0.5.6/src/auto_archiver/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/utils/gsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/utils/gworksheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/utils/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/utils/webdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-18 17:49:56.000000 auto_archiver-0.5.6/src/auto_archiver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:51:08.369878 auto_archiver-0.5.6/src/auto_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-18 17:51:08.000000 auto_archiver-0.5.6/src/auto_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-18 17:51:08.000000 auto_archiver-0.5.6/src/auto_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:51:08.000000 auto_archiver-0.5.6/src/auto_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 17:51:08.000000 auto_archiver-0.5.6/src/auto_archiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:51:08.000000 auto_archiver-0.5.6/src/auto_archiver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-18 17:51:08.000000 auto_archiver-0.5.6/src/auto_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 17:51:08.000000 auto_archiver-0.5.6/src/auto_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.414122 auto_archiver-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-18 18:30:57.414122 auto_archiver-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-18 18:30:57.414122 auto_archiver-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.402122 auto_archiver-0.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.406122 auto_archiver-0.5.7/src/auto_archiver/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.406122 auto_archiver-0.5.7/src/auto_archiver/archivers/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/instagram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/instagram_tbot_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/telegram_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/telethon_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/tiktok_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/twitter_api_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/twitter_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/vk_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/archivers/youtubedl_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/auto_auto_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.410122 auto_archiver-0.5.7/src/auto_archiver/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/core/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/core/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.410122 auto_archiver-0.5.7/src/auto_archiver/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/databases/console_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/databases/csv_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/databases/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/databases/gsheet_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.410122 auto_archiver-0.5.7/src/auto_archiver/enrichers/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/hash_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/screenshot_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/thumbnail_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/wacz_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/wayback_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/enrichers/whisper_enricher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.410122 auto_archiver-0.5.7/src/auto_archiver/feeders/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/feeders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/feeders/cli_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/feeders/feeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/feeders/gsheet_feeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.410122 auto_archiver-0.5.7/src/auto_archiver/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/formatters/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/formatters/html_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/formatters/mute_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.410122 auto_archiver-0.5.7/src/auto_archiver/formatters/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/formatters/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/formatters/templates/html_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/formatters/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.414122 auto_archiver-0.5.7/src/auto_archiver/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/storages/gd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/storages/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/storages/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/storages/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.414122 auto_archiver-0.5.7/src/auto_archiver/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/utils/gsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/utils/gworksheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/utils/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/utils/webdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-18 18:29:35.000000 auto_archiver-0.5.7/src/auto_archiver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:30:57.406122 auto_archiver-0.5.7/src/auto_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-18 18:30:57.000000 auto_archiver-0.5.7/src/auto_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-18 18:30:57.000000 auto_archiver-0.5.7/src/auto_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:30:57.000000 auto_archiver-0.5.7/src/auto_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 18:30:57.000000 auto_archiver-0.5.7/src/auto_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:30:57.000000 auto_archiver-0.5.7/src/auto_archiver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-18 18:30:57.000000 auto_archiver-0.5.7/src/auto_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 18:30:57.000000 auto_archiver-0.5.7/src/auto_archiver.egg-info/top_level.txt
```

### Comparing `auto_archiver-0.5.6/LICENSE` & `auto_archiver-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/PKG-INFO` & `auto_archiver-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_archiver
-Version: 0.5.6
+Version: 0.5.7
 Summary: Easily archive online media content
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
 Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
 Project-URL: Bellingcat, https://www.bellingcat.com
```

### Comparing `auto_archiver-0.5.6/README.md` & `auto_archiver-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/setup.cfg` & `auto_archiver-0.5.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/archivers/archiver.py` & `auto_archiver-0.5.7/src/auto_archiver/archivers/archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/archivers/instagram_archiver.py` & `auto_archiver-0.5.7/src/auto_archiver/archivers/instagram_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/archivers/instagram_tbot_archiver.py` & `auto_archiver-0.5.7/src/auto_archiver/archivers/instagram_tbot_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/archivers/telegram_archiver.py` & `auto_archiver-0.5.7/src/auto_archiver/archivers/telegram_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/archivers/telethon_archiver.py` & `auto_archiver-0.5.7/src/auto_archiver/archivers/telethon_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/archivers/tiktok_archiver.py` & `auto_archiver-0.5.7/src/auto_archiver/archivers/tiktok_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/archivers/twitter_api_archiver.py` & `auto_archiver-0.5.7/src/auto_archiver/archivers/twitter_api_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/archivers/twitter_archiver.py` & `auto_archiver-0.5.7/src/auto_archiver/archivers/twitter_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/archivers/vk_archiver.py` & `auto_archiver-0.5.7/src/auto_archiver/archivers/vk_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/archivers/youtubedl_archiver.py` & `auto_archiver-0.5.7/src/auto_archiver/archivers/youtubedl_archiver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/auto_auto_archive.py` & `auto_archiver-0.5.7/src/auto_archiver/auto_auto_archive.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/core/config.py` & `auto_archiver-0.5.7/src/auto_archiver/core/config.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/core/context.py` & `auto_archiver-0.5.7/src/auto_archiver/core/context.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/core/media.py` & `auto_archiver-0.5.7/src/auto_archiver/core/media.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/core/metadata.py` & `auto_archiver-0.5.7/src/auto_archiver/core/metadata.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/core/orchestrator.py` & `auto_archiver-0.5.7/src/auto_archiver/core/orchestrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         # 5 - store media
         # looks for Media in result.media and also result.media[x].properties (as list or dict values)
         result.store()
 
         # 6 - format and store formatted if needed
         # enrichers typically need access to already stored URLs etc
         if (final_media := self.formatter.format(result)):
-            final_media.store()
+            final_media.store(url=url)
             result.set_final_media(final_media)
 
         if result.is_empty():
             result.status = "nothing archived"
 
         # signal completion to databases (DBs, Google Sheets, CSV, ...)
         for d in self.databases: d.done(result)
```

### Comparing `auto_archiver-0.5.6/src/auto_archiver/core/step.py` & `auto_archiver-0.5.7/src/auto_archiver/core/step.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/databases/console_db.py` & `auto_archiver-0.5.7/src/auto_archiver/databases/console_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/databases/csv_db.py` & `auto_archiver-0.5.7/src/auto_archiver/databases/csv_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/databases/database.py` & `auto_archiver-0.5.7/src/auto_archiver/databases/database.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/databases/gsheet_db.py` & `auto_archiver-0.5.7/src/auto_archiver/databases/gsheet_db.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/enrichers/enricher.py` & `auto_archiver-0.5.7/src/auto_archiver/enrichers/enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/enrichers/hash_enricher.py` & `auto_archiver-0.5.7/src/auto_archiver/enrichers/hash_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/enrichers/screenshot_enricher.py` & `auto_archiver-0.5.7/src/auto_archiver/enrichers/screenshot_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/enrichers/thumbnail_enricher.py` & `auto_archiver-0.5.7/src/auto_archiver/enrichers/thumbnail_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/enrichers/wacz_enricher.py` & `auto_archiver-0.5.7/src/auto_archiver/enrichers/wacz_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/enrichers/wayback_enricher.py` & `auto_archiver-0.5.7/src/auto_archiver/enrichers/wayback_enricher.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/enrichers/whisper_enricher.py` & `auto_archiver-0.5.7/src/auto_archiver/enrichers/whisper_enricher.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
         url = to_enrich.get_url()
         logger.debug(f"WHISPER[{self.action}]: iterating media items for {url=}.")
 
         job_results = {}
         for i, m in enumerate(to_enrich.media):
             if m.is_video() or m.is_audio():
-                m.store()
+                m.store(url=url)
                 try:
                     job_id = self.submit_job(m)
                     job_results[job_id] = False
                     logger.debug(f"JOB SUBMITTED: {job_id=} for {m.key=}")
                     to_enrich.media[i].set("whisper_model", {"job_id": job_id})
                 except Exception as e:
                     logger.error(f"Failed to submit whisper job for {m.filename=} with error {e}\n{traceback.format_exc()}")
@@ -54,15 +54,15 @@
         job_results = self.check_jobs(job_results)
 
         for i, m in enumerate(to_enrich.media):
             if m.is_video() or m.is_audio():
                 job_id = to_enrich.media[i].get("whisper_model")["job_id"]
                 to_enrich.media[i].set("whisper_model", {
                     "job_id": job_id,
-                    self.action: job_results[job_id]
+                    **job_results[job_id]
                 })
 
     def submit_job(self, media: Media):
         s3 = self._get_s3_storage()
         s3_url = s3.get_cdn_url(media)
         assert s3_url in media.urls, f"Could not find S3 url ({s3_url}) in list of stored media urls "
         payload = {
@@ -96,26 +96,24 @@
         logger.debug(f"Checked job {job_id=} with status='{j['status']}'")
         if j['status'] == "processing": return False
         elif j['status'] == "error": return f"Error: {j['meta']['error']}"
         elif j['status'] == "success":
             r_res = requests.get(f'{self.api_endpoint}/jobs/{job_id}/artifacts', headers={'Authorization': f'Bearer {self.api_key}'})
             assert r_res.status_code == 200, f"Job artifacts did not respond with 200, instead with: {r_res.status_code}"
             logger.success(r_res.json())
-            result = []
-            for artifact in r_res.json():
+            result = {}
+            for art_id, artifact in enumerate(r_res.json()):
                 subtitle = []
                 full_text = []
                 for i, d in enumerate(artifact.get("data")):
                     subtitle.append(f"{i+1}\n{d.get('start')} --> {d.get('end')}\n{d.get('text').strip()}")
                     full_text.append(d.get('text').strip())
                 if not len(subtitle): continue
-                result.append({
-                    "subtitle": "\n".join(subtitle),
-                    "full_text": "\n".join(full_text),
-                })
+                result[f"artifact_{art_id}_subtitle"] = "\n".join(subtitle)
+                result[f"artifact_{art_id}_text"] = "\n".join(full_text)
             return result
         return False
 
     def _get_s3_storage(self) -> S3Storage:
         try:
             return next(s for s in ArchivingContext.get("storages") if s.__class__ == S3Storage)
         except:
```

### Comparing `auto_archiver-0.5.6/src/auto_archiver/feeders/cli_feeder.py` & `auto_archiver-0.5.7/src/auto_archiver/feeders/cli_feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/feeders/feeder.py` & `auto_archiver-0.5.7/src/auto_archiver/feeders/feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/feeders/gsheet_feeder.py` & `auto_archiver-0.5.7/src/auto_archiver/feeders/gsheet_feeder.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/formatters/formatter.py` & `auto_archiver-0.5.7/src/auto_archiver/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/formatters/html_formatter.py` & `auto_archiver-0.5.7/src/auto_archiver/formatters/html_formatter.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/formatters/templates/html_template.html` & `auto_archiver-0.5.7/src/auto_archiver/formatters/templates/html_template.html`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
         table.content td:nth-child(2),
         .center {
             text-align: center;
         }
 
         .copy:hover {
-            font-weight: 600;
+            background: aliceblue;
             cursor: copy;
         }
 
         #notification {
             position: fixed;
             right: 20px;
             top: 20px;
```

### Comparing `auto_archiver-0.5.6/src/auto_archiver/formatters/templates/macros.html` & `auto_archiver-0.5.7/src/auto_archiver/formatters/templates/macros.html`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/storages/gd.py` & `auto_archiver-0.5.7/src/auto_archiver/storages/gd.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/storages/local.py` & `auto_archiver-0.5.7/src/auto_archiver/storages/local.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/storages/s3.py` & `auto_archiver-0.5.7/src/auto_archiver/storages/s3.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/storages/storage.py` & `auto_archiver-0.5.7/src/auto_archiver/storages/storage.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/utils/gsheet.py` & `auto_archiver-0.5.7/src/auto_archiver/utils/gsheet.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/utils/gworksheet.py` & `auto_archiver-0.5.7/src/auto_archiver/utils/gworksheet.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/utils/misc.py` & `auto_archiver-0.5.7/src/auto_archiver/utils/misc.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/utils/url.py` & `auto_archiver-0.5.7/src/auto_archiver/utils/url.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver/utils/webdriver.py` & `auto_archiver-0.5.7/src/auto_archiver/utils/webdriver.py`

 * *Files identical despite different names*

### Comparing `auto_archiver-0.5.6/src/auto_archiver.egg-info/PKG-INFO` & `auto_archiver-0.5.7/src/auto_archiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-archiver
-Version: 0.5.6
+Version: 0.5.7
 Summary: Easily archive online media content
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Project-URL: Source Code, https://github.com/bellingcat/auto-archiver
 Project-URL: Bug Tracker, https://github.com/bellingcat/auto-archiver/issues
 Project-URL: Bellingcat, https://www.bellingcat.com
```

### Comparing `auto_archiver-0.5.6/src/auto_archiver.egg-info/SOURCES.txt` & `auto_archiver-0.5.7/src/auto_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

