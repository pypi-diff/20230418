# Comparing `tmp/liblxml3-2.1.tar.gz` & `tmp/liblxml3-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liblxml3-2.1.tar", last modified: Tue Apr 18 08:01:57 2023, max compression
+gzip compressed data, was "liblxml3-2.2.tar", last modified: Tue Apr 18 08:10:20 2023, max compression
```

## Comparing `liblxml3-2.1.tar` & `liblxml3-2.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:57.515003 liblxml3-2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 08:01:57.515003 liblxml3-2.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:57.507003 liblxml3-2.1/bot/
--rw-r--r--   0 runner    (1001) docker     (123)    36386 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26870 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:57.507003 liblxml3-2.1/bot/helper/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:57.507003 liblxml3-2.1/bot/helper/ext_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/ext_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30489 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/ext_utils/bot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/ext_utils/db_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/ext_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/ext_utils/fs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/ext_utils/html_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/ext_utils/queued_starter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/ext_utils/shortenurl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/ext_utils/telegraph_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/ext_utils/timegap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:57.507003 liblxml3-2.1/bot/helper/mirror_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:57.507003 liblxml3-2.1/bot/helper/mirror_utils/download_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/download_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/download_utils/aria2_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    30926 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/download_utils/direct_link_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/download_utils/gd_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/download_utils/mega_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/download_utils/qbit_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/download_utils/telegram_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/download_utils/yt_dlp_download_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:57.511003 liblxml3-2.1/bot/helper/mirror_utils/status_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/status_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/status_utils/aria_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/status_utils/clone_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/status_utils/convert_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/status_utils/extract_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/status_utils/gd_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/status_utils/mega_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/status_utils/qbit_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/status_utils/queue_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/status_utils/split_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/status_utils/telegram_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/status_utils/tg_upload_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/status_utils/upload_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/status_utils/yt_dlp_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/status_utils/zip_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:57.511003 liblxml3-2.1/bot/helper/mirror_utils/upload_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/upload_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45943 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/upload_utils/gdriveTools.py
--rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/mirror_utils/upload_utils/pyrogramEngine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:57.511003 liblxml3-2.1/bot/helper/telegram_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/telegram_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/telegram_helper/bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/telegram_helper/button_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/telegram_helper/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/helper/telegram_helper/message_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:57.511003 liblxml3-2.1/bot/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17216 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/anilist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/authorize.py
--rw-r--r--   0 runner    (1001) docker     (123)    57929 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/bot_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/bt_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/cancel_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)    23774 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/drive_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/mediainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/mirror_leech.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/mirror_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/pictures.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/save_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)    18977 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/sel_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/speedtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/users.py
--rw-r--r--   0 runner    (1001) docker     (123)    34924 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/users_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/wayback.py
--rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-04-18 08:01:43.000000 liblxml3-2.1/bot/modules/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:01:57.515003 liblxml3-2.1/liblxml3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 08:01:57.000000 liblxml3-2.1/liblxml3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-18 08:01:57.000000 liblxml3-2.1/liblxml3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:01:57.000000 liblxml3-2.1/liblxml3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 08:01:57.000000 liblxml3-2.1/liblxml3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-18 08:01:57.000000 liblxml3-2.1/liblxml3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-18 08:01:57.000000 liblxml3-2.1/liblxml3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:01:57.515003 liblxml3-2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-18 08:01:43.000000 liblxml3-2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:10:20.549125 liblxml3-2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 08:10:20.549125 liblxml3-2.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:10:20.537125 liblxml3-2.2/bot/
+-rw-r--r--   0 runner    (1001) docker     (123)    36388 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26870 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:10:20.537125 liblxml3-2.2/bot/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:10:20.537125 liblxml3-2.2/bot/helper/ext_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/ext_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30489 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/ext_utils/bot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/ext_utils/db_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/ext_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/ext_utils/fs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/ext_utils/html_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/ext_utils/queued_starter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/ext_utils/shortenurl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/ext_utils/telegraph_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/ext_utils/timegap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:10:20.537125 liblxml3-2.2/bot/helper/mirror_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:10:20.541125 liblxml3-2.2/bot/helper/mirror_utils/download_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/download_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/download_utils/aria2_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30926 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/download_utils/direct_link_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/download_utils/gd_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/download_utils/mega_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/download_utils/qbit_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/download_utils/telegram_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/download_utils/yt_dlp_download_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:10:20.541125 liblxml3-2.2/bot/helper/mirror_utils/status_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/status_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/status_utils/aria_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/status_utils/clone_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/status_utils/convert_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/status_utils/extract_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/status_utils/gd_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/status_utils/mega_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/status_utils/qbit_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/status_utils/queue_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/status_utils/split_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/status_utils/telegram_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/status_utils/tg_upload_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/status_utils/upload_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/status_utils/yt_dlp_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/status_utils/zip_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:10:20.541125 liblxml3-2.2/bot/helper/mirror_utils/upload_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/upload_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45943 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/upload_utils/gdriveTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/mirror_utils/upload_utils/pyrogramEngine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:10:20.541125 liblxml3-2.2/bot/helper/telegram_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/telegram_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/telegram_helper/bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/telegram_helper/button_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/telegram_helper/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/helper/telegram_helper/message_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:10:20.545125 liblxml3-2.2/bot/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17216 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/anilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/authorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57929 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/bot_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/bt_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/cancel_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23774 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/drive_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/mediainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/mirror_leech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/mirror_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/pictures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/save_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18977 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/sel_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/speedtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34924 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/users_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/wayback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-04-18 08:10:09.000000 liblxml3-2.2/bot/modules/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:10:20.549125 liblxml3-2.2/liblxml3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 08:10:20.000000 liblxml3-2.2/liblxml3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-18 08:10:20.000000 liblxml3-2.2/liblxml3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:10:20.000000 liblxml3-2.2/liblxml3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 08:10:20.000000 liblxml3-2.2/liblxml3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-18 08:10:20.000000 liblxml3-2.2/liblxml3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-18 08:10:20.000000 liblxml3-2.2/liblxml3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:10:20.549125 liblxml3-2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-18 08:10:09.000000 liblxml3-2.2/setup.py
```

### Comparing `liblxml3-2.1/bot/__init__.py` & `liblxml3-2.2/bot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -992,9 +992,9 @@
 dispatcher = updater.dispatcher
 job_queue = updater.job_queue
 
 from flask import Flask
 
 fapp = Flask(__name__)
 
-PORT = os.environ.get('PORT')
+PORT = int(environ.get('PORT'))
 Popen(f"gunicorn --bind 0.0.0.0:{PORT} fapp", shell=True)
```

### Comparing `liblxml3-2.1/bot/__main__.py` & `liblxml3-2.2/bot/__main__.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/ext_utils/bot_utils.py` & `liblxml3-2.2/bot/helper/ext_utils/bot_utils.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/ext_utils/db_handler.py` & `liblxml3-2.2/bot/helper/ext_utils/db_handler.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/ext_utils/fs_utils.py` & `liblxml3-2.2/bot/helper/ext_utils/fs_utils.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/ext_utils/html_helper.py` & `liblxml3-2.2/bot/helper/ext_utils/html_helper.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/ext_utils/queued_starter.py` & `liblxml3-2.2/bot/helper/ext_utils/queued_starter.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/ext_utils/shortenurl.py` & `liblxml3-2.2/bot/helper/ext_utils/shortenurl.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/ext_utils/telegraph_helper.py` & `liblxml3-2.2/bot/helper/ext_utils/telegraph_helper.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/ext_utils/timegap.py` & `liblxml3-2.2/bot/helper/ext_utils/timegap.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/download_utils/aria2_download.py` & `liblxml3-2.2/bot/helper/mirror_utils/download_utils/aria2_download.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/download_utils/direct_link_generator.py` & `liblxml3-2.2/bot/helper/mirror_utils/download_utils/direct_link_generator.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/download_utils/gd_downloader.py` & `liblxml3-2.2/bot/helper/mirror_utils/download_utils/gd_downloader.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/download_utils/mega_downloader.py` & `liblxml3-2.2/bot/helper/mirror_utils/download_utils/mega_downloader.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/download_utils/qbit_downloader.py` & `liblxml3-2.2/bot/helper/mirror_utils/download_utils/qbit_downloader.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/download_utils/telegram_downloader.py` & `liblxml3-2.2/bot/helper/mirror_utils/download_utils/telegram_downloader.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/download_utils/yt_dlp_download_helper.py` & `liblxml3-2.2/bot/helper/mirror_utils/download_utils/yt_dlp_download_helper.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/status_utils/aria_download_status.py` & `liblxml3-2.2/bot/helper/mirror_utils/status_utils/aria_download_status.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/status_utils/clone_status.py` & `liblxml3-2.2/bot/helper/mirror_utils/status_utils/clone_status.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/status_utils/convert_status.py` & `liblxml3-2.2/bot/helper/mirror_utils/status_utils/convert_status.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/status_utils/extract_status.py` & `liblxml3-2.2/bot/helper/mirror_utils/status_utils/extract_status.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/status_utils/gd_download_status.py` & `liblxml3-2.2/bot/helper/mirror_utils/status_utils/gd_download_status.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/status_utils/mega_download_status.py` & `liblxml3-2.2/bot/helper/mirror_utils/status_utils/mega_download_status.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/status_utils/qbit_download_status.py` & `liblxml3-2.2/bot/helper/mirror_utils/status_utils/qbit_download_status.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/status_utils/queue_status.py` & `liblxml3-2.2/bot/helper/mirror_utils/status_utils/queue_status.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/status_utils/split_status.py` & `liblxml3-2.2/bot/helper/mirror_utils/status_utils/split_status.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/status_utils/telegram_download_status.py` & `liblxml3-2.2/bot/helper/mirror_utils/status_utils/telegram_download_status.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/status_utils/tg_upload_status.py` & `liblxml3-2.2/bot/helper/mirror_utils/status_utils/tg_upload_status.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/status_utils/upload_status.py` & `liblxml3-2.2/bot/helper/mirror_utils/status_utils/upload_status.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/status_utils/yt_dlp_download_status.py` & `liblxml3-2.2/bot/helper/mirror_utils/status_utils/yt_dlp_download_status.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/status_utils/zip_status.py` & `liblxml3-2.2/bot/helper/mirror_utils/status_utils/zip_status.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/upload_utils/gdriveTools.py` & `liblxml3-2.2/bot/helper/mirror_utils/upload_utils/gdriveTools.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/mirror_utils/upload_utils/pyrogramEngine.py` & `liblxml3-2.2/bot/helper/mirror_utils/upload_utils/pyrogramEngine.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/telegram_helper/bot_commands.py` & `liblxml3-2.2/bot/helper/telegram_helper/bot_commands.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/telegram_helper/button_build.py` & `liblxml3-2.2/bot/helper/telegram_helper/button_build.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/telegram_helper/filters.py` & `liblxml3-2.2/bot/helper/telegram_helper/filters.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/helper/telegram_helper/message_utils.py` & `liblxml3-2.2/bot/helper/telegram_helper/message_utils.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/anilist.py` & `liblxml3-2.2/bot/modules/anilist.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/authorize.py` & `liblxml3-2.2/bot/modules/authorize.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/bot_settings.py` & `liblxml3-2.2/bot/modules/bot_settings.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/broadcast.py` & `liblxml3-2.2/bot/modules/broadcast.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/bt_select.py` & `liblxml3-2.2/bot/modules/bt_select.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/cancel_mirror.py` & `liblxml3-2.2/bot/modules/cancel_mirror.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/clone.py` & `liblxml3-2.2/bot/modules/clone.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/count.py` & `liblxml3-2.2/bot/modules/count.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/delete.py` & `liblxml3-2.2/bot/modules/delete.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/drive_clean.py` & `liblxml3-2.2/bot/modules/drive_clean.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/eval.py` & `liblxml3-2.2/bot/modules/eval.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/gmail.py` & `liblxml3-2.2/bot/modules/gmail.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/hash.py` & `liblxml3-2.2/bot/modules/hash.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/imdb.py` & `liblxml3-2.2/bot/modules/imdb.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/list.py` & `liblxml3-2.2/bot/modules/list.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/listener.py` & `liblxml3-2.2/bot/modules/listener.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/mediainfo.py` & `liblxml3-2.2/bot/modules/mediainfo.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/mirror_leech.py` & `liblxml3-2.2/bot/modules/mirror_leech.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/mirror_status.py` & `liblxml3-2.2/bot/modules/mirror_status.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/pictures.py` & `liblxml3-2.2/bot/modules/pictures.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/rss.py` & `liblxml3-2.2/bot/modules/rss.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/save_msg.py` & `liblxml3-2.2/bot/modules/save_msg.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/scraper.py` & `liblxml3-2.2/bot/modules/scraper.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/search.py` & `liblxml3-2.2/bot/modules/search.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/sel_cat.py` & `liblxml3-2.2/bot/modules/sel_cat.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/shell.py` & `liblxml3-2.2/bot/modules/shell.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/speedtest.py` & `liblxml3-2.2/bot/modules/speedtest.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/users.py` & `liblxml3-2.2/bot/modules/users.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/users_settings.py` & `liblxml3-2.2/bot/modules/users_settings.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/wayback.py` & `liblxml3-2.2/bot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/bot/modules/ytdlp.py` & `liblxml3-2.2/bot/modules/ytdlp.py`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/liblxml3.egg-info/SOURCES.txt` & `liblxml3-2.2/liblxml3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liblxml3-2.1/setup.py` & `liblxml3-2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='liblxml3',
-    version='2.1',
+    version='2.2',
     packages=find_packages(),
     include_package_data=True,
     package_data={
         '': ['*.*']
     },
     install_requires=[
         'aiohttp',
```

