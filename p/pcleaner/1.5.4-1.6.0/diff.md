# Comparing `tmp/pcleaner-1.5.4.tar.gz` & `tmp/pcleaner-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcleaner-1.5.4.tar", last modified: Mon Apr 17 19:15:57 2023, max compression
+gzip compressed data, was "pcleaner-1.6.0.tar", last modified: Tue Apr 18 20:41:45 2023, max compression
```

## Comparing `pcleaner-1.5.4.tar` & `pcleaner-1.6.0.tar`

### file list

```diff
@@ -1,67 +1,71 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.554623 pcleaner-1.5.4/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.5.4/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-17 19:15:57.554623 pcleaner-1.5.4/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11039 2023-04-12 00:54:25.000000 pcleaner-1.5.4/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.547957 pcleaner-1.5.4/pcleaner/
--rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2023-04-17 18:13:47.000000 pcleaner-1.5.4/pcleaner/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    17232 2023-04-17 18:10:07.000000 pcleaner-1.5.4/pcleaner/analytics.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8765 2023-04-14 12:31:00.000000 pcleaner-1.5.4/pcleaner/cleaner.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5841 2023-04-14 16:52:21.000000 pcleaner-1.5.4/pcleaner/cli_utils.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.551290 pcleaner-1.5.4/pcleaner/comic_text_detector/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/basemodel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/inference.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.551290 pcleaner-1.5.4/pcleaner/comic_text_detector/models/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/models/__init__.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.551290 pcleaner-1.5.4/pcleaner/comic_text_detector/models/yolov5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/models/yolov5/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/models/yolov5/common.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/models/yolov5/yolo.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.551290 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/db_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/export.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/general.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/imgproc_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/io_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/loss.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/textblock.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/textmask.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/weight_init.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.5.4/pcleaner/comic_text_detector/utils/yolov5_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35861 2023-04-13 14:02:44.000000 pcleaner-1.5.4/pcleaner/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6056 2023-04-17 18:08:37.000000 pcleaner-1.5.4/pcleaner/ctd_interface.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.5.4/pcleaner/denoiser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.554623 pcleaner-1.5.4/pcleaner/gui/
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.554623 pcleaner-1.5.4/pcleaner/gui/CustomQ/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3206 2022-08-27 14:37:25.000000 pcleaner-1.5.4/pcleaner/gui/CustomQ/CTableWidget.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-1.5.4/pcleaner/gui/CustomQ/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-1.5.4/pcleaner/gui/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    21094 2023-04-17 02:04:01.000000 pcleaner-1.5.4/pcleaner/gui/file_table.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1904 2023-04-17 01:26:57.000000 pcleaner-1.5.4/pcleaner/gui/launcher.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    34194 2023-04-17 02:09:36.000000 pcleaner-1.5.4/pcleaner/gui/mainwindow_driver.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.554623 pcleaner-1.5.4/pcleaner/gui/rc_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-1.5.4/pcleaner/gui/rc_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    81975 2023-04-17 01:43:12.000000 pcleaner-1.5.4/pcleaner/gui/rc_generated_files/icons_rc.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.554623 pcleaner-1.5.4/pcleaner/gui/ui_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 00:09:43.000000 pcleaner-1.5.4/pcleaner/gui/ui_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6310 2023-04-17 00:10:07.000000 pcleaner-1.5.4/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    29139 2023-04-17 02:04:43.000000 pcleaner-1.5.4/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3233 2023-04-17 16:45:08.000000 pcleaner-1.5.4/pcleaner/gui/worker_thread.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1321 2023-04-17 02:10:39.000000 pcleaner-1.5.4/pcleaner/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    23338 2023-04-13 18:46:48.000000 pcleaner-1.5.4/pcleaner/image_ops.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    26041 2023-04-17 18:36:40.000000 pcleaner-1.5.4/pcleaner/main.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4845 2023-04-14 12:51:27.000000 pcleaner-1.5.4/pcleaner/model_downloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8183 2023-04-13 18:07:02.000000 pcleaner-1.5.4/pcleaner/pre_processor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7546 2023-01-23 03:12:00.000000 pcleaner-1.5.4/pcleaner/profile_cli.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13299 2023-04-13 19:11:27.000000 pcleaner-1.5.4/pcleaner/structures.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-17 19:15:57.551290 pcleaner-1.5.4/pcleaner.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-17 19:15:57.000000 pcleaner-1.5.4/pcleaner.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1855 2023-04-17 19:15:57.000000 pcleaner-1.5.4/pcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-17 19:15:57.000000 pcleaner-1.5.4/pcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-04-17 19:15:57.000000 pcleaner-1.5.4/pcleaner.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      188 2023-04-17 19:15:57.000000 pcleaner-1.5.4/pcleaner.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-04-17 19:15:57.000000 pcleaner-1.5.4/pcleaner.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.5.4/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1058 2023-04-17 19:15:57.554623 pcleaner-1.5.4/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.5.4/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.614643 pcleaner-1.6.0/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.6.0/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-18 20:41:45.614643 pcleaner-1.6.0/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11039 2023-04-12 00:54:25.000000 pcleaner-1.6.0/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.607976 pcleaner-1.6.0/pcleaner/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2023-04-18 20:40:27.000000 pcleaner-1.6.0/pcleaner/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    17227 2023-04-18 15:30:05.000000 pcleaner-1.6.0/pcleaner/analytics.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5841 2023-04-14 16:52:21.000000 pcleaner-1.6.0/pcleaner/cli_utils.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.611310 pcleaner-1.6.0/pcleaner/comic_text_detector/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/basemodel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/inference.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.611310 pcleaner-1.6.0/pcleaner/comic_text_detector/models/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/models/__init__.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.611310 pcleaner-1.6.0/pcleaner/comic_text_detector/models/yolov5/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/models/yolov5/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/models/yolov5/common.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/models/yolov5/yolo.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.614643 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/db_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/export.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/general.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/imgproc_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/io_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/loss.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/textblock.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/textmask.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/weight_init.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/yolov5_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    36360 2023-04-18 15:36:00.000000 pcleaner-1.6.0/pcleaner/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6056 2023-04-17 18:08:37.000000 pcleaner-1.6.0/pcleaner/ctd_interface.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.614643 pcleaner-1.6.0/pcleaner/data/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-1.6.0/pcleaner/data/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.6.0/pcleaner/denoiser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.614643 pcleaner-1.6.0/pcleaner/gui/
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.614643 pcleaner-1.6.0/pcleaner/gui/CustomQ/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1076 2023-04-18 01:52:48.000000 pcleaner-1.6.0/pcleaner/gui/CustomQ/CComboBox.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3206 2022-08-27 14:37:25.000000 pcleaner-1.6.0/pcleaner/gui/CustomQ/CTableWidget.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-1.6.0/pcleaner/gui/CustomQ/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-1.6.0/pcleaner/gui/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    21094 2023-04-17 02:04:01.000000 pcleaner-1.6.0/pcleaner/gui/file_table.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1904 2023-04-17 01:26:57.000000 pcleaner-1.6.0/pcleaner/gui/launcher.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35231 2023-04-18 16:17:08.000000 pcleaner-1.6.0/pcleaner/gui/mainwindow_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2938 2023-04-18 16:38:05.000000 pcleaner-1.6.0/pcleaner/gui/profile_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.614643 pcleaner-1.6.0/pcleaner/gui/rc_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-1.6.0/pcleaner/gui/rc_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    80116 2023-04-18 01:36:08.000000 pcleaner-1.6.0/pcleaner/gui/rc_generated_files/icons_rc.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.614643 pcleaner-1.6.0/pcleaner/gui/ui_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 00:09:43.000000 pcleaner-1.6.0/pcleaner/gui/ui_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6310 2023-04-17 00:10:07.000000 pcleaner-1.6.0/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    29181 2023-04-18 18:34:09.000000 pcleaner-1.6.0/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3233 2023-04-17 16:45:08.000000 pcleaner-1.6.0/pcleaner/gui/worker_thread.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1321 2023-04-17 02:10:39.000000 pcleaner-1.6.0/pcleaner/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    23327 2023-04-18 15:30:05.000000 pcleaner-1.6.0/pcleaner/image_ops.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    26399 2023-04-18 20:02:05.000000 pcleaner-1.6.0/pcleaner/main.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8762 2023-04-18 15:30:06.000000 pcleaner-1.6.0/pcleaner/masker.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4845 2023-04-14 12:51:27.000000 pcleaner-1.6.0/pcleaner/model_downloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8778 2023-04-18 20:36:25.000000 pcleaner-1.6.0/pcleaner/pre_processor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7546 2023-01-23 03:12:00.000000 pcleaner-1.6.0/pcleaner/profile_cli.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14109 2023-04-18 20:03:45.000000 pcleaner-1.6.0/pcleaner/structures.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.611310 pcleaner-1.6.0/pcleaner.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-18 20:41:45.000000 pcleaner-1.6.0/pcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1945 2023-04-18 20:41:45.000000 pcleaner-1.6.0/pcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-18 20:41:45.000000 pcleaner-1.6.0/pcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-04-18 20:41:45.000000 pcleaner-1.6.0/pcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      188 2023-04-18 20:41:45.000000 pcleaner-1.6.0/pcleaner.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-04-18 20:41:45.000000 pcleaner-1.6.0/pcleaner.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.6.0/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1058 2023-04-18 20:41:45.614643 pcleaner-1.6.0/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.6.0/setup.py
```

### Comparing `pcleaner-1.5.4/LICENSE` & `pcleaner-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/PKG-INFO` & `pcleaner-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.5.4
+Version: 1.6.0
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pcleaner-1.5.4/README.md` & `pcleaner-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/analytics.py` & `pcleaner-1.6.0/pcleaner/analytics.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,17 +117,17 @@
             f"{lower_bar}{clr.Fore.RED}{upper_bar} {upper}{clr.Style.RESET_ALL} / {lower}"
         )
 
     # Show legend.
     print(f"\n█ Small boxes | {clr.Fore.RED}█ Removed boxes{clr.Style.RESET_ALL}")
 
 
-def draw_cleaner_histogram(data: dict[str, tuple[int, int]]) -> None:
+def draw_masker_histogram(data: dict[str, tuple[int, int]]) -> None:
     """
-    Draw a histogram of the cleaner results.
+    Draw a histogram of the masker results.
 
     :param data: A dict of the mask name, (perfect uses, all uses).
     """
 
     width = terminal_width()
     # Find the maximum value in the data. (at least 1 to avoid division by zero)
     max_value = max(list(map(lambda x: x[1], data.values())))
@@ -189,17 +189,17 @@
         )
         for i in range(min_value, max_value // partition_size)
     ]
 
     return partition
 
 
-def show_cleaner_analytics(analytics: list[tuple[Path, bool, int, float]]):
+def show_masker_analytics(analytics: list[tuple[Path, bool, int, float]]):
     """
-    Present the analytics gathered from the cleaning process.
+    Present the analytics gathered from the masking process.
 
     The analytics for each page in the list consist of the following tuple:
     list[original_image_path, mask_found, mask_index, border_deviation]
 
     :param analytics: The analytics gathered from each page.
     """
 
@@ -245,15 +245,15 @@
         for index, perfect_total in enumerate(
             zip(perfect_mask_usages_by_index, mask_usages_by_index)
         )
         if index < len(mask_usages_by_index) - 1
     }
     mask_usages_dict["Box mask"] = perfect_mask_usages_by_index[-1], mask_usages_by_index[-1]
 
-    draw_cleaner_histogram(mask_usages_dict)
+    draw_masker_histogram(mask_usages_dict)
 
     # Find out what pages had how many failures.
     # Structure: {page_path: {"succeeded": 0, "failed": 0}}
     pages_with_success_and_fails_dict: defaultdict[Path, defaultdict[str, int]] = defaultdict(
         lambda: defaultdict(int)
     )
     for analytics in analytics:
```

### Comparing `pcleaner-1.5.4/pcleaner/cleaner.py` & `pcleaner-1.6.0/pcleaner/masker.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 from PIL import Image
 from logzero import logger, loglevel, DEBUG, INFO
 
 import pcleaner.image_ops as ops
 import pcleaner.structures as st
 
 
-def clean_page(c_data: st.CleanerData) -> list[tuple[Path, bool, int, float]]:
+def clean_page(m_data: st.MaskerData) -> list[tuple[Path, bool, int, float]]:
     """
     Do all the shit and return analytics for mask fitting.
 
-    :param c_data: All the data needed for the cleaning process.
+    :param m_data: All the data needed for the cleaning process.
     :return: Analytics, consisting of the json file path, and a list of whether the mask was generated, the index of
         the best mask, and the border uniformity of the best mask for each box.
     """
 
-    page_data = st.PageData.from_json(c_data.json_path.read_text())
+    page_data = st.PageData.from_json(m_data.json_path.read_text())
 
     # Make a shorter alias.
-    g_conf = c_data.general_config
-    c_conf = c_data.cleaner_config
+    g_conf = m_data.general_config
+    m_conf = m_data.masker_config
 
     original_path = Path(page_data.original_path)
     original_img_path_as_png = original_path.with_suffix(
         ".png"
     )  # Make sure all derived file names are .png.
     # Clobber protection prefixes have the form "[A-Z]{4}-\d+_file name", ex. JMCF-0_0023.json
-    clobber_protection_prefix = c_data.json_path.stem.split("_")[0]
+    clobber_protection_prefix = m_data.json_path.stem.split("_")[0]
     cache_out_path = (
-        c_data.cache_dir / f"{clobber_protection_prefix}_{original_img_path_as_png.name}"
+        m_data.cache_dir / f"{clobber_protection_prefix}_{original_img_path_as_png.name}"
     )
 
     def save_mask(img, name_suffix):
-        if c_data.show_masks:
+        if m_data.show_masks:
             img.save(cache_out_path.with_stem(cache_out_path.stem + name_suffix))
 
     # Load the base image.
     base_image = Image.open(page_data.image_path)
 
     # Make a box mask. These will serve as basic masks as opposed to the AI generated precise ones.
     box_mask = page_data.make_box_mask(base_image.size, st.BoxType.EXTENDED_BOX)
@@ -58,17 +58,17 @@
     mask_fitments: list[st.MaskFittingResults] = [
         ops.pick_best_mask(
             base=base_image,
             precise_mask=cut_mask,
             box_mask=box_mask,
             masking_box=masking_box,
             reference_box=reference_box,
-            cleaner_conf=c_conf,
+            masker_conf=m_conf,
             scale=page_data.scale,
-            save_masks=c_data.show_masks,
+            save_masks=m_data.show_masks,
             analytics_page_path=Path(original_img_path_as_png),
         )
         for masking_box, reference_box in zip(
             page_data.merged_extended_boxes, page_data.reference_boxes
         )
     ]
     # Take out all entries that are None, since these masks were false positives.
@@ -78,59 +78,59 @@
     analytics: list[tuple[Path, bool, int, float]] = [m.analytics for m in mask_fitments]
 
     # Remove entries if they failed.
     best_masks = [m for m in mask_fitments if not m.failed]
 
     combined_mask = ops.combine_best_masks(base_image.size, best_masks)
 
-    if c_data.show_masks:
+    if m_data.show_masks:
         # Save the masks in the debug folder.
         ops.visualize_mask_fitments(
             base_image, mask_fitments, cache_out_path.with_stem(cache_out_path.stem + "_masks")
         )
 
         # Output the result with the debug filter.
-        combined_mask_debug = ops.apply_debug_filter_to_mask(combined_mask, c_conf.debug_mask_color)
+        combined_mask_debug = ops.apply_debug_filter_to_mask(combined_mask, m_conf.debug_mask_color)
         base_image_copy = base_image.copy()
         base_image_copy.paste(combined_mask_debug, (0, 0), combined_mask_debug)
         save_mask(base_image_copy, "_with_masks")
 
     # Save the combined mask for denoising.
     combined_mask_path = cache_out_path.with_stem(cache_out_path.stem + "_combined_mask")
     combined_mask.save(combined_mask_path)
     save_denoising_data(
         Path(page_data.original_path),
         original_img_path_as_png,
         combined_mask_path,
         Path(page_data.image_path),
         cache_out_path,
         page_data.scale,
-        c_conf.mask_max_standard_deviation,
+        m_conf.mask_max_standard_deviation,
         mask_fitments,
     )
 
     # Settle on the final output path for the cleaned image.
     # Check if outputting directly.
-    if c_data.output_dir is not None:
+    if m_data.output_dir is not None:
         # If the scale isn't 1, then we need to reload the original image and scale the mask to fit.
         if page_data.scale != 1:
             cleaned_image = Image.open(page_data.original_path)
             combined_mask = combined_mask.resize(cleaned_image.size, Image.NEAREST)
         else:
             cleaned_image = base_image.copy()
 
         cleaned_image.paste(combined_mask, (0, 0), combined_mask)
 
-        if c_data.output_dir.is_absolute():
-            final_out_path = c_data.output_dir / original_img_path_as_png.name
+        if m_data.output_dir.is_absolute():
+            final_out_path = m_data.output_dir / original_img_path_as_png.name
         else:
             # Take the original image path, and place the image in a subdirectory.
             # This is for when multiple directories were passed in.
             final_out_path = (
-                original_img_path_as_png.parent / c_data.output_dir / original_img_path_as_png.name
+                original_img_path_as_png.parent / m_data.output_dir / original_img_path_as_png.name
             )
 
         final_out_path.parent.mkdir(parents=True, exist_ok=True)
         final_cleaned_out_path = final_out_path.with_name(final_out_path.stem + "_clean.png")
         final_mask_out_path = final_out_path.with_name(final_out_path.stem + "_mask.png")
 
         # Check what the preferred output format is.
@@ -145,25 +145,25 @@
         if g_conf.preferred_mask_file_type is None:
             # Use png by default.
             final_mask_out_path = final_mask_out_path.with_suffix(".png")
         else:
             final_mask_out_path = final_mask_out_path.with_suffix(g_conf.preferred_mask_file_type)
 
         # The arg parser should ensure that both can't be true at once, not like that'd be an issue, just plain silly.
-        if not c_data.save_only_mask and not c_data.save_only_text:
+        if not m_data.save_only_mask and not m_data.save_only_text:
             # Save the final image.
             logger.debug(f"Saving final image to {final_cleaned_out_path}")
             ops.save_optimized(cleaned_image, final_cleaned_out_path, original_path)
 
-        if not c_data.save_only_cleaned and not c_data.save_only_text:
+        if not m_data.save_only_cleaned and not m_data.save_only_text:
             # Save the final image.
             logger.debug(f"Saving final mask to {final_mask_out_path}")
             ops.save_optimized(combined_mask, final_mask_out_path)
 
-        if c_data.extract_text:
+        if m_data.extract_text:
             # Extract the text layer from the image.
             logger.debug(f"Extracting text from {final_cleaned_out_path}")
             text_img = ops.extract_text(base_image, combined_mask)
             text_out_path = final_out_path.with_name(final_out_path.stem + "_text.png")
             if g_conf.preferred_mask_file_type is None:
                 # Use png by default.
                 text_out_path = text_out_path.with_suffix(".png")
```

### Comparing `pcleaner-1.5.4/pcleaner/cli_utils.py` & `pcleaner-1.6.0/pcleaner/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/comic_text_detector/basemodel.py` & `pcleaner-1.6.0/pcleaner/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/comic_text_detector/inference.py` & `pcleaner-1.6.0/pcleaner/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/comic_text_detector/models/yolov5/common.py` & `pcleaner-1.6.0/pcleaner/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/comic_text_detector/models/yolov5/yolo.py` & `pcleaner-1.6.0/pcleaner/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/db_utils.py` & `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/export.py` & `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/general.py` & `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/imgproc_utils.py` & `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/io_utils.py` & `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/loss.py` & `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/textblock.py` & `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/textmask.py` & `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/weight_init.py` & `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/comic_text_detector/utils/yolov5_utils.py` & `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/config.py` & `pcleaner-1.6.0/pcleaner/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         try_to_load(self, config_updater, section, int, "box_right_padding_initial")
         try_to_load(self, config_updater, section, int, "box_padding_extended")
         try_to_load(self, config_updater, section, int, "box_right_padding_extended")
         try_to_load(self, config_updater, section, int, "box_reference_padding")
 
 
 @dataclass
-class CleanerConfig:
+class MaskerConfig:
     mask_growth_step_pixels: int = 2
     mask_growth_steps: int = 11
     off_white_max_threshold: int = 240
     mask_improvement_threshold: float = 0.1
     mask_selection_fast: bool = False
     mask_max_standard_deviation: float = 15
     debug_mask_color: tuple[int, int, int, int] = (108, 30, 240, 127)
@@ -227,15 +227,15 @@
         """
         Write the config to the config updater object.
 
         :param config_updater: An existing config updater object.
         :param add_after_section: The section to add the new section after.
         """
         config_str = f"""\
-        [Cleaner]
+        [Masker]
         
         
         # Number of pixels to grow the mask by each step.
         # This bulks up the outline of the mask, so smaller values will be more accurate but slower.
         mask_growth_step_pixels = {self.mask_growth_step_pixels}
         
         # Number of steps to grow the mask by.
@@ -267,60 +267,62 @@
         # which isn't a good mask, as it will require inpainting anyway.
         mask_max_standard_deviation = {self.mask_max_standard_deviation}
         
         # Color to use for the debug mask. This is a tuple of RGBA values.
         debug_mask_color = {','.join(map(str, self.debug_mask_color))}
         
         """
-        cleaner_conf = cu.ConfigUpdater()
-        cleaner_conf.read_string(multi_left_strip(config_str))
-        cleaner_section = cleaner_conf["Cleaner"]
-        config_updater[add_after_section].add_after.space(2).section(cleaner_section.detach())
+        masker_conf = cu.ConfigUpdater()
+        masker_conf.read_string(multi_left_strip(config_str))
+        masker_section = masker_conf["Masker"]
+        config_updater[add_after_section].add_after.space(2).section(masker_section.detach())
 
     def import_from_conf(self, config_updater: cu.ConfigUpdater) -> None:
         """
         Read the config from the config updater object.
 
         :param config_updater: An existing config updater object.
         """
-        section = "Cleaner"
+        section = "Masker"
         if not config_updater.has_section(section):
             logger.info(f"No {section} section found in the profile, using defaults.")
             return
 
         try_to_load(self, config_updater, section, int, "mask_growth_step_pixels")
         try_to_load(self, config_updater, section, int, "mask_growth_steps")
         try_to_load(self, config_updater, section, int, "off_white_max_threshold")
         try_to_load(self, config_updater, section, float, "mask_improvement_threshold")
         try_to_load(self, config_updater, section, bool, "mask_selection_fast")
         try_to_load(self, config_updater, section, float, "mask_max_standard_deviation")
         try:
             color_tuple: tuple[int, ...] = tuple(
-                int(x) for x in config_updater["Cleaner"]["debug_mask_color"].value.split(",")
+                int(x) for x in config_updater["Masker"]["debug_mask_color"].value.split(",")
             )
             if len(color_tuple) != 4:
                 raise ValueError(
                     f"Invalid color tuple length. Expected 4: 'Red, Green, Blue, Alpha' got {len(color_tuple)}"
                 )
             color_tuple: tuple[int, int, int, int]
             self.debug_mask_color = color_tuple
         except (cu.NoOptionError, ValueError):
             pass
 
 
 @dataclass
 class DenoiserConfig:
+    denoising_enabled: bool = True
     noise_min_standard_deviation: float = 0.25
     noise_outline_size: int = 5
     noise_fade_radius: int = 1
     colored_images: bool = False
     filter_strength: int = 10
     color_filter_strength: int = 10
     template_window_size: int = 7
     search_window_size: int = 21
+    # TODO respect denoising enabled
 
     def export_to_conf(self, config_updater: cu.ConfigUpdater, add_after_section: str) -> None:
         """
         Write the config to the config updater object.
 
         :param config_updater: An existing config updater object.
         :param add_after_section: The section to add the new section after.
@@ -333,14 +335,19 @@
         
         # This means that the color of pixels around the edge of a mask isn't uniform,
         # which is quantified as a standard deviation. The denoiser can target masks with
         # a minimum standard deviation and denoise the area right around the mask.
         # This preserves details in the rest of the image, but removes artifacts right around where
         # the text used to be.
         
+        # Since this is an optional step and may even be superfluous for high-resolution images that 
+        # don't suffer from jpeg-artifacts, it can be disabled here.
+        # Set to False to disable denoising.
+        denoising_enabled = {self.denoising_enabled}
+        
         # The minimum standard deviation of colors around the edge of a given mask
         # to perform denoising on the region around the mask.
         noise_min_standard_deviation = {self.noise_min_standard_deviation}
         
         # The thickness of an outline to denoise around a mask.
         noise_outline_size = {self.noise_outline_size}
         
@@ -396,34 +403,40 @@
     """
     A profile is a collection of settings that can be saved and loaded from disk.
     """
 
     general: GeneralConfig = GeneralConfig()
     text_detector: TextDetectorConfig = TextDetectorConfig()
     pre_processor: PreProcessorConfig = PreProcessorConfig()
-    cleaner: CleanerConfig = CleanerConfig()
+    masker: MaskerConfig = MaskerConfig()
     denoiser: DenoiserConfig = DenoiserConfig()
 
+    def bundle_config(self) -> cu.ConfigUpdater:
+        """
+        Bundle the config into a ConfigUpdater object.
+        """
+        config_updater = cu.ConfigUpdater()
+        self.general.export_to_conf(config_updater)
+        self.text_detector.export_to_conf(config_updater, "General")
+        self.pre_processor.export_to_conf(config_updater, "TextDetector")
+        self.masker.export_to_conf(config_updater, "PreProcessor")
+        self.denoiser.export_to_conf(config_updater, "Masker")
+        return config_updater
+
     def write(self, path: Path) -> bool:
         """
         Write the profile to a file.
 
         :param path: The path to write the profile to.
         :return: True if the profile was written successfully, False otherwise.
         """
         logger.debug("Writing profile to disk...")
-        config_updater = cu.ConfigUpdater()
-        self.general.export_to_conf(config_updater)
-        self.text_detector.export_to_conf(config_updater, "General")
-        self.pre_processor.export_to_conf(config_updater, "TextDetector")
-        self.cleaner.export_to_conf(config_updater, "PreProcessor")
-        self.denoiser.export_to_conf(config_updater, "Cleaner")
         try:
             with open(path, "w") as file:
-                config_updater.write(file)
+                self.bundle_config().write(file)
             return True
         except Exception as e:
             logger.error(f"Failed to write profile to {path}:\n{e}")
             return False
 
     @classmethod
     def load(cls, path: Path) -> "Profile":
@@ -434,15 +447,15 @@
         config = cu.ConfigUpdater()
         try:
             config.read(path)
             profile = cls()
             profile.general.import_from_conf(config)
             profile.text_detector.import_from_conf(config)
             profile.pre_processor.import_from_conf(config)
-            profile.cleaner.import_from_conf(config)
+            profile.masker.import_from_conf(config)
             profile.denoiser.import_from_conf(config)
         except Exception as e:
             logger.error(f"Failed to load profile from {path}:\n{e}")
             profile = cls()
             print("Failed to load profile, using default profile.")
         return profile
```

### Comparing `pcleaner-1.5.4/pcleaner/ctd_interface.py` & `pcleaner-1.6.0/pcleaner/ctd_interface.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/denoiser.py` & `pcleaner-1.6.0/pcleaner/denoiser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/gui/CustomQ/CTableWidget.py` & `pcleaner-1.6.0/pcleaner/gui/CustomQ/CTableWidget.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/gui/file_table.py` & `pcleaner-1.6.0/pcleaner/gui/file_table.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/gui/launcher.py` & `pcleaner-1.6.0/pcleaner/gui/launcher.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/gui/mainwindow_driver.py` & `pcleaner-1.6.0/pcleaner/gui/mainwindow_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,39 +6,43 @@
 import PySide6.QtGui as Qg
 import PySide6.QtWidgets as Qw
 from PySide6.QtCore import Signal
 from logzero import logger
 
 import pcleaner.cli_utils as cu
 import pcleaner.helpers as hp
+import pcleaner.config as cfg
+import pcleaner.gui.profile_parser as pp
 from pcleaner.gui.ui_generated_files.ui_Mainwindow import Ui_MainWindow
 from pcleaner.gui.file_table import Column
 from pcleaner import __display_name__, __version__
 
 
 # noinspection PyUnresolvedReferences
 class MainWindow(Qw.QMainWindow, Ui_MainWindow):
 
-    # config: cfg.Config = None
+    config: cfg.Config = None
     # glossary: st.Glossary = None
     processing: bool = False
 
     # text_params_changed = Signal(st.Glossary)
     # text_output_changed = Signal()
     # abort_translation_worker = Signal()
 
     label_stats: Qw.QLabel
 
-    def __init__(self, mock: bool = False):
+    def __init__(self):
         Qw.QMainWindow.__init__(self)
         self.setupUi(self)
         self.setWindowTitle(f"{__display_name__} {__version__}")
         self.setWindowIcon(Qg.QIcon(":/logo-tiny.png"))
         self.processing = False
 
+        self.config = cfg.load_config()
+
         self.initialize_ui()
         #
         # self.threadpool = Qc.QThreadPool.globalInstance()
         # logger.info(f"Multithreading with maximum {self.threadpool.maxThreadCount()} threads")
         #
         # self.config = cfg.Config.load()
         # # Set debug flag.
@@ -53,14 +57,15 @@
 
     def initialize_ui(self):
         self.hide_progress()
         self.start_button_enabled(False)
         self.show_button_start()
         self.update_input_buttons()
         self.set_up_statusbar()
+        self.initialize_profiles()
 
         # Allow the table to accept file drops and hide the ID column.
         self.file_table.setAcceptDrops(True)
         self.file_table.setColumnHidden(Column.ID, True)
         self.file_table.setColumnWidth(Column.FILENAME, 200)
         self.file_table.setColumnWidth(Column.STATUS, 200)
 
@@ -350,14 +355,41 @@
     def update_file_table_params(self):
         """
         Update the file table with the current parameters.
         """
         self.text_params_changed.emit(self.glossary)
 
     """
+    Profiles
+    """
+
+    def initialize_profiles(self):
+        """
+        Load the available profiles and display the default profile.
+        """
+        all_profiles: list[tuple[str, Path | None]] = [(cfg.RESERVED_PROFILE_NAMES[0], None)]
+        for profile_name, profile_path in self.config.saved_profiles.items():
+            all_profiles.append((profile_name, profile_path))
+
+        self.comboBox_current_profile.clear()
+        for profile_name, profile_path in all_profiles:
+            self.comboBox_current_profile.addTextItemLinkedData(profile_name, profile_path)
+
+        self.load_current_profile()
+
+    def load_current_profile(self):
+        """
+        Load the current profile.
+        """
+        logger.debug("Loading current profile.")
+        self.config.load_profile(self.comboBox_current_profile.currentText())
+
+        pp.parse_profile_structure(self.config.current_profile)
+
+    """
     Glossary
     """
 
     def load_glossary(self):
         """
         Open a glossary file and parse it.
         Afterwards, notify any files to apply it.
```

### Comparing `pcleaner-1.5.4/pcleaner/gui/rc_generated_files/icons_rc.py` & `pcleaner-1.6.0/pcleaner/gui/rc_generated_files/icons_rc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1392,55 +1392,14 @@
  L 6.7265625 11.\
 419922 L 14 4.22\
 07031 L 13.27343\
 8 3.5 z \x22\x0a     c\
 lass=\x22ColorSchem\
 e-Text\x22\x0a     />\x0a\
 </svg>\x0a\
-\x00\x00\x02b\
-<\
-svg width=\x2216\x22 x\
-mlns=\x22http://www\
-.w3.org/2000/svg\
-\x22 height=\x2216\x22 vi\
-ewBox=\x220 0 16 16\
-\x22>\x0a <path color-\
-interpolation-fi\
-lters=\x22linearRGB\
-\x22 color=\x22#000000\
-\x22 image-renderin\
-g=\x22auto\x22 color-r\
-endering=\x22auto\x22 \
-d=\x22m2.064 2v12h1\
-2v-12h-11zm1 1h1\
-.912c.057.16.087\
-.33.088.5 0 .828\
--.672 1.5-1.5 1.\
-5-.17-.001-.34-.\
-03-.5-.088zm2.94\
-7 0h7.05v10h-10v\
--.783l1.326-1.29\
-9 1.408-1.404.56\
-4.418 1.102 1.06\
-8 2.6-2.398 4 3.\
-891-1-2.492-3-3-\
-2.6 2.6-1.6-1.6-\
-2.801 2.801v-4.8\
-54c.164.034.332.\
-052.5.053 1.381 \
-0 2.5-1.119 2.5-\
-2.5-.001-.168-.0\
-18-.336-.053-.5\x22\
- color-interpola\
-tion=\x22sRGB\x22 text\
--rendering=\x22auto\
-\x22 fill=\x22#4bc94b\x22\
- shape-rendering\
-=\x22auto\x22/>\x0a</svg>\
-\x0a\
 \x00\x00\x02^\
 <\
 svg width=\x2216\x22 x\
 mlns=\x22http://www\
 .w3.org/2000/svg\
 \x22 height=\x2216\x22 vi\
 ewBox=\x220 0 16 16\
@@ -2715,55 +2674,14 @@
  L 6.7265625 11.\
 419922 L 14 4.22\
 07031 L 13.27343\
 8 3.5 z \x22\x0a     c\
 lass=\x22ColorSchem\
 e-Text\x22\x0a     />\x0a\
 </svg>\x0a\
-\x00\x00\x02b\
-<\
-svg width=\x2216\x22 x\
-mlns=\x22http://www\
-.w3.org/2000/svg\
-\x22 height=\x2216\x22 vi\
-ewBox=\x220 0 16 16\
-\x22>\x0a <path color-\
-interpolation-fi\
-lters=\x22linearRGB\
-\x22 color=\x22#000000\
-\x22 image-renderin\
-g=\x22auto\x22 color-r\
-endering=\x22auto\x22 \
-d=\x22m2.064 2v12h1\
-2v-12h-11zm1 1h1\
-.912c.057.16.087\
-.33.088.5 0 .828\
--.672 1.5-1.5 1.\
-5-.17-.001-.34-.\
-03-.5-.088zm2.94\
-7 0h7.05v10h-10v\
--.783l1.326-1.29\
-9 1.408-1.404.56\
-4.418 1.102 1.06\
-8 2.6-2.398 4 3.\
-891-1-2.492-3-3-\
-2.6 2.6-1.6-1.6-\
-2.801 2.801v-4.8\
-54c.164.034.332.\
-052.5.053 1.381 \
-0 2.5-1.119 2.5-\
-2.5-.001-.168-.0\
-18-.336-.053-.5\x22\
- color-interpola\
-tion=\x22sRGB\x22 text\
--rendering=\x22auto\
-\x22 fill=\x22#4bc94b\x22\
- shape-rendering\
-=\x22auto\x22/>\x0a</svg>\
-\x0a\
 \x00\x00\x02^\
 <\
 svg width=\x2216\x22 x\
 mlns=\x22http://www\
 .w3.org/2000/svg\
 \x22 height=\x2216\x22 vi\
 ewBox=\x220 0 16 16\
@@ -3069,19 +2987,14 @@
 \x00i\x00a\x00l\x00o\x00g\x00-\x00c\x00a\x00n\x00c\x00e\x00l\x00.\x00s\x00v\x00g\
 \
 \x00\x13\
 \x04h\xff\xc7\
 \x00d\
 \x00i\x00a\x00l\x00o\x00g\x00-\x00o\x00k\x00-\x00a\x00p\x00p\x00l\x00y\x00.\x00s\
 \x00v\x00g\
-\x00\x12\
-\x0f\x13\xd8G\
-\x00i\
-\x00m\x00a\x00g\x00e\x00-\x00j\x00p\x00e\x00g\x002\x000\x000\x000\x00.\x00s\x00v\
-\x00g\
 \x00\x0e\
 \x092O\x87\
 \x00i\
 \x00m\x00a\x00g\x00e\x00-\x00t\x00i\x00f\x00f\x00.\x00s\x00v\x00g\
 \x00\x13\
 \x0eR1\xe7\
 \x00i\
@@ -3100,85 +3013,83 @@
 \x00i\
 \x00m\x00a\x00g\x00e\x00-\x00p\x00n\x00g\x00.\x00s\x00v\x00g\
 "
 
 qt_resource_struct = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x03\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00:\x00\x02\x00\x00\x00\x03\x00\x00\x00!\
+\x00\x00\x00:\x00\x02\x00\x00\x00\x03\x00\x00\x00 \
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x1a\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
 \x00\x00\x01\x87\x8c\xdf\x0e\xff\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x03\x00\x00\x00\x04\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00h\x00\x02\x00\x00\x00\x01\x00\x00\x00\x1a\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x80\x00\x02\x00\x00\x00\x01\x00\x00\x00\x07\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00L\x00\x01\x00\x00\x00\x01\x00\x00bk\
+\x00\x00\x00L\x00\x01\x00\x00\x00\x01\x00\x00`\x05\
 \x00\x00\x01\x82\xfe\x95\xbc\x1d\
 \x00\x00\x00\x94\x00\x02\x00\x00\x00\x12\x00\x00\x00\x08\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x01\x80\x00\x00\x00\x00\x00\x01\x00\x00\x86\xe7\
+\x00\x00\x01\x80\x00\x00\x00\x00\x00\x01\x00\x00\x84\x81\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02&\x00\x00\x00\x00\x00\x01\x00\x00\x92\xb0\
+\x00\x00\x02&\x00\x00\x00\x00\x00\x01\x00\x00\x90J\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x03\x18\x00\x00\x00\x00\x00\x01\x00\x00\x9eS\
+\x00\x00\x03\x18\x00\x00\x00\x00\x00\x01\x00\x00\x9b\xed\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x03@\x00\x00\x00\x00\x00\x01\x00\x00\xa1U\
+\x00\x00\x03@\x00\x00\x00\x00\x00\x01\x00\x00\x9e\xef\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x00\xc4\x00\x00\x00\x00\x00\x01\x00\x00tQ\
+\x00\x00\x00\xc4\x00\x00\x00\x00\x00\x01\x00\x00q\xeb\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01Z\x00\x00\x00\x00\x00\x01\x00\x00\x80z\
+\x00\x00\x01Z\x00\x00\x00\x00\x00\x01\x00\x00~\x14\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\xf6\x00\x00\x00\x00\x00\x01\x00\x00\x9c~\
+\x00\x00\x02\xf6\x00\x00\x00\x00\x00\x01\x00\x00\x9a\x18\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\x14\x00\x00\x00\x00\x00\x01\x00\x00z:\
+\x00\x00\x01\x14\x00\x00\x00\x00\x00\x01\x00\x00w\xd4\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x014\x00\x00\x00\x00\x00\x01\x00\x00~\x1b\
+\x00\x00\x014\x00\x00\x00\x00\x00\x01\x00\x00{\xb5\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x00\x9e\x00\x00\x00\x00\x00\x01\x00\x00p\xdc\
+\x00\x00\x00\x9e\x00\x00\x00\x00\x00\x01\x00\x00nv\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\xb6\x00\x00\x00\x00\x00\x01\x00\x00\x97\xeb\
+\x00\x00\x02\xb6\x00\x00\x00\x00\x00\x01\x00\x00\x95\x85\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x8b\xcb\
+\x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x89e\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\xd4\x00\x00\x00\x00\x00\x01\x00\x00\x99\xd9\
+\x00\x00\x02\xd4\x00\x00\x00\x00\x00\x01\x00\x00\x97s\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\xc8\x00\x00\x00\x00\x00\x01\x00\x00\x8dp\
+\x00\x00\x01\xc8\x00\x00\x00\x00\x00\x01\x00\x00\x8b\x0a\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02N\x00\x00\x00\x00\x00\x01\x00\x00\x94\xc2\
+\x00\x00\x02N\x00\x00\x00\x00\x00\x01\x00\x00\x92\x5c\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x00\xf2\x00\x00\x00\x00\x00\x01\x00\x00xG\
+\x00\x00\x00\xf2\x00\x00\x00\x00\x00\x01\x00\x00u\xe1\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\x80\x00\x00\x00\x00\x00\x01\x00\x00\x96\xd4\
+\x00\x00\x02\x80\x00\x00\x00\x00\x00\x01\x00\x00\x94n\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\xfe\x00\x00\x00\x00\x00\x01\x00\x00\x8f\xcf\
+\x00\x00\x01\xfe\x00\x00\x00\x00\x00\x01\x00\x00\x8di\
 \x00\x00\x01\x83\x9f\xda\x12\xf9\
-\x00\x00\x00\x94\x00\x02\x00\x00\x00\x06\x00\x00\x00\x1b\
+\x00\x00\x00\x94\x00\x02\x00\x00\x00\x05\x00\x00\x00\x1b\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x04\x04\x00\x00\x00\x00\x00\x01\x00\x00\xac\xdd\
-\x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x04&\x00\x00\x00\x00\x00\x01\x00\x00\xafC\
+\x00\x00\x03\xda\x00\x00\x00\x00\x00\x01\x00\x00\xa8\x11\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\xe4\x00\x00\x00\x00\x00\x01\x00\x00\xaa{\
+\x00\x00\x03\xfc\x00\x00\x00\x00\x00\x01\x00\x00\xaaw\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\x96\x00\x00\x00\x00\x00\x01\x00\x00\xa5\xb7\
+\x00\x00\x03\xba\x00\x00\x00\x00\x00\x01\x00\x00\xa5\xaf\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\xb8\x00\x00\x00\x00\x00\x01\x00\x00\xa8\x19\
+\x00\x00\x03l\x00\x00\x00\x00\x00\x01\x00\x00\xa0\xeb\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03l\x00\x00\x00\x00\x00\x01\x00\x00\xa3Q\
+\x00\x00\x03\x8e\x00\x00\x00\x00\x00\x01\x00\x00\xa3M\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x00h\x00\x02\x00\x00\x00\x01\x00\x00\x007\
+\x00\x00\x00h\x00\x02\x00\x00\x00\x01\x00\x00\x006\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x80\x00\x02\x00\x00\x00\x01\x00\x00\x00$\
+\x00\x00\x00\x80\x00\x02\x00\x00\x00\x01\x00\x00\x00#\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00L\x00\x01\x00\x00\x00\x01\x00\x00\x14h\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x00\x94\x00\x02\x00\x00\x00\x12\x00\x00\x00%\
+\x00\x00\x00\x94\x00\x02\x00\x00\x00\x12\x00\x00\x00$\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x01\x80\x00\x00\x00\x00\x00\x01\x00\x007\xa9\
 \x00\x00\x01\x81\xc0B\xdb\x80\
 \x00\x00\x02&\x00\x00\x00\x00\x00\x01\x00\x00Cr\
 \x00\x00\x01\x81\xc0B\xdb\x80\
 \x00\x00\x03\x18\x00\x00\x00\x00\x00\x01\x00\x00O\x15\
 \x00\x00\x01\x81\xc0B\xdb\x80\
@@ -3208,28 +3119,26 @@
 \x00\x00\x01\x81\xc0B\xdb\x80\
 \x00\x00\x00\xf2\x00\x00\x00\x00\x00\x01\x00\x00)\x09\
 \x00\x00\x01\x81\xc0B\xdb\x80\
 \x00\x00\x02\x80\x00\x00\x00\x00\x00\x01\x00\x00G\x96\
 \x00\x00\x01\x81\xc0B\xdb\x80\
 \x00\x00\x01\xfe\x00\x00\x00\x00\x00\x01\x00\x00@\x91\
 \x00\x00\x01\x83\x9f\xda\x12\xf9\
-\x00\x00\x00\x94\x00\x02\x00\x00\x00\x06\x00\x00\x008\
+\x00\x00\x00\x94\x00\x02\x00\x00\x00\x05\x00\x00\x007\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x04\x04\x00\x00\x00\x00\x00\x01\x00\x00]\x9f\
-\x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x04&\x00\x00\x00\x00\x00\x01\x00\x00`\x05\
+\x00\x00\x03\xda\x00\x00\x00\x00\x00\x01\x00\x00[9\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\xe4\x00\x00\x00\x00\x00\x01\x00\x00[=\
+\x00\x00\x03\xfc\x00\x00\x00\x00\x00\x01\x00\x00]\x9f\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\x96\x00\x00\x00\x00\x00\x01\x00\x00Vy\
-\x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\xb8\x00\x00\x00\x00\x00\x01\x00\x00X\xdb\
+\x00\x00\x03\xba\x00\x00\x00\x00\x00\x01\x00\x00X\xd7\
 \x00\x00\x01\x86\xac\x9ffH\
 \x00\x00\x03l\x00\x00\x00\x00\x00\x01\x00\x00T\x13\
 \x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x03\x8e\x00\x00\x00\x00\x00\x01\x00\x00Vu\
+\x00\x00\x01\x86\xac\x9ffH\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `pcleaner-1.5.4/pcleaner/gui/ui_generated_files/ui_ImageDetails.py` & `pcleaner-1.6.0/pcleaner/gui/ui_generated_files/ui_ImageDetails.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/gui/ui_generated_files/ui_Mainwindow.py` & `pcleaner-1.6.0/pcleaner/gui/ui_generated_files/ui_Mainwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,23 @@
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
 from PySide6.QtGui import (QAction, QBrush, QColor, QConicalGradient,
     QCursor, QFont, QFontDatabase, QGradient,
     QIcon, QImage, QKeySequence, QLinearGradient,
     QPainter, QPalette, QPixmap, QRadialGradient,
     QTransform)
-from PySide6.QtWidgets import (QAbstractItemView, QApplication, QCheckBox, QComboBox,
-    QFormLayout, QFrame, QGroupBox, QHBoxLayout,
-    QHeaderView, QLabel, QLineEdit, QMainWindow,
-    QMenu, QMenuBar, QProgressBar, QPushButton,
-    QRadioButton, QSizePolicy, QSpacerItem, QSplitter,
-    QStatusBar, QTabWidget, QTableWidgetItem, QTextEdit,
-    QToolBox, QVBoxLayout, QWidget)
+from PySide6.QtWidgets import (QAbstractItemView, QApplication, QCheckBox, QFormLayout,
+    QFrame, QGroupBox, QHBoxLayout, QHeaderView,
+    QLabel, QLineEdit, QMainWindow, QMenu,
+    QMenuBar, QProgressBar, QPushButton, QRadioButton,
+    QSizePolicy, QSpacerItem, QSplitter, QStatusBar,
+    QTabWidget, QTableWidgetItem, QTextEdit, QToolBox,
+    QVBoxLayout, QWidget)
 
+from pcleaner.gui.CustomQ.CComboBox import CComboBox
 from pcleaner.gui.file_table import FileTable
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         if not MainWindow.objectName():
             MainWindow.setObjectName(u"MainWindow")
         MainWindow.resize(1701, 720)
@@ -80,15 +81,15 @@
         self.splitter.setHandleWidth(10)
         self.groupBox = QGroupBox(self.splitter)
         self.groupBox.setObjectName(u"groupBox")
         self.verticalLayout_2 = QVBoxLayout(self.groupBox)
         self.verticalLayout_2.setObjectName(u"verticalLayout_2")
         self.horizontalLayout_2 = QHBoxLayout()
         self.horizontalLayout_2.setObjectName(u"horizontalLayout_2")
-        self.comboBox_current_profile = QComboBox(self.groupBox)
+        self.comboBox_current_profile = CComboBox(self.groupBox)
         self.comboBox_current_profile.addItem("")
         self.comboBox_current_profile.setObjectName(u"comboBox_current_profile")
         sizePolicy = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.comboBox_current_profile.sizePolicy().hasHeightForWidth())
         self.comboBox_current_profile.setSizePolicy(sizePolicy)
@@ -185,15 +186,15 @@
         self.verticalLayout_3.addWidget(self.file_table)
 
         self.tabWidget_files.addTab(self.tabWidget_table_page, "")
         self.splitter.addWidget(self.tabWidget_files)
         self.frame_3 = QFrame(self.splitter)
         self.frame_3.setObjectName(u"frame_3")
         self.frame_3.setFrameShape(QFrame.StyledPanel)
-        self.frame_3.setFrameShadow(QFrame.Sunken)
+        self.frame_3.setFrameShadow(QFrame.Raised)
         self.verticalLayout_4 = QVBoxLayout(self.frame_3)
         self.verticalLayout_4.setObjectName(u"verticalLayout_4")
         self.horizontalLayout_3 = QHBoxLayout()
         self.horizontalLayout_3.setObjectName(u"horizontalLayout_3")
         self.groupBox_4 = QGroupBox(self.frame_3)
         self.groupBox_4.setObjectName(u"groupBox_4")
         self.verticalLayout_9 = QVBoxLayout(self.groupBox_4)
```

### Comparing `pcleaner-1.5.4/pcleaner/gui/worker_thread.py` & `pcleaner-1.6.0/pcleaner/gui/worker_thread.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/helpers.py` & `pcleaner-1.6.0/pcleaner/helpers.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/image_ops.py` & `pcleaner-1.6.0/pcleaner/image_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,15 @@
 
 def pick_best_mask(
     base: Image,
     precise_mask: Image,
     box_mask: Image,
     masking_box: tuple[int, int, int, int],
     reference_box: tuple[int, int, int, int],
-    cleaner_conf: cfg.CleanerConfig,
+    masker_conf: cfg.MaskerConfig,
     scale: float,
     save_masks: bool,
     analytics_page_path: Path,
 ) -> None | st.MaskFittingResults:
     """
     Generate various sizes of the precise mask and pick the best one from
     among them, and the box mask.
@@ -289,15 +289,15 @@
 
 
     :param base: The base image.
     :param precise_mask: The precise mask.
     :param box_mask: The box mask.
     :param masking_box: The box to cut the mask out of.
     :param reference_box: The box to cut the base image out of.
-    :param cleaner_conf: The cleaner config.
+    :param masker_conf: The masker config.
     :param scale: The scale of the original image to the base image.
     :param save_masks: Whether to save the masks.
     :param analytics_page_path: The path to the original image for the analytics.
     :return: The best mask and what color to make it and the box (along with analytics). If no best
         mask was found, return None for the mask and color.
     """
     # Calculate offset coords between the reference box and the mask box.
@@ -319,64 +319,64 @@
 
     box_mask = cut_out_mask(box_mask, masking_box, base.size, x_offset, y_offset)
 
     # Generate masks of various sizes for the precise mask, then add the box mask to the list.
     # The generated masks are in ascending size order.
     mask_gen = make_mask_steps_convolution(
         precise_mask,
-        hp.scale_length_rounded(cleaner_conf.mask_growth_step_pixels, scale),
-        cleaner_conf.mask_growth_steps,
+        hp.scale_length_rounded(masker_conf.mask_growth_step_pixels, scale),
+        masker_conf.mask_growth_steps,
     )
 
     # When using the fast mask selection, make a new generator with the box mask as the first mask,
     # followed by the generated masks.
     def generator_with_first(generator, first):
         yield first
         yield from generator
 
     def generator_with_last(generator, last):
         yield from generator
         yield last
 
-    if cleaner_conf.mask_selection_fast:
+    if masker_conf.mask_selection_fast:
         mask_stream = generator_with_first(mask_gen, box_mask)
     else:
         mask_stream = generator_with_last(mask_gen, box_mask)
 
     # Calculate the border uniformity of each mask.
     # Border deviations: (std deviation, median color)
     border_deviations: list[tuple[Image, int]] = []
     masks = []
     for mask in mask_stream:
         try:
             masks.append(mask)
             current_deviation = border_std_deviation(
-                base, mask, cleaner_conf.off_white_max_threshold
+                base, mask, masker_conf.off_white_max_threshold
             )
             border_deviations.append(current_deviation)
             # Break on the first perfect mask if using the fast mask selection.
-            if cleaner_conf.mask_selection_fast and current_deviation[0] == 0:
+            if masker_conf.mask_selection_fast and current_deviation[0] == 0:
                 break
         except BlankMaskError:
             return None
     # Find the best mask.
     best_mask = None
     lowest_border_deviation = None
     lowest_deviation_color = None
     for i, border_deviation in enumerate(border_deviations):
         mask_deviation, mask_color = border_deviation
         if i == 0 or mask_deviation <= (
-            lowest_border_deviation * (1 - cleaner_conf.mask_improvement_threshold)
+            lowest_border_deviation * (1 - masker_conf.mask_improvement_threshold)
         ):
             lowest_border_deviation = mask_deviation
             lowest_deviation_color = mask_color
             best_mask = masks[i]
 
     # If the std deviation is too high, return None.
-    if lowest_border_deviation > cleaner_conf.mask_max_standard_deviation:
+    if lowest_border_deviation > masker_conf.mask_max_standard_deviation:
         return st.MaskFittingResults(
             best_mask=None,
             median_color=lowest_deviation_color,
             mask_coords=reference_box[:2],
             analytics_page_path=analytics_page_path,
             analytics_mask_index=masks.index(best_mask),
             analytics_std_deviation=lowest_border_deviation,
```

### Comparing `pcleaner-1.5.4/pcleaner/main.py` & `pcleaner-1.6.0/pcleaner/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Panel Cleaner
 
 Usage:
     pcleaner clean [<image_path> ...] [--output_dir=<output_dir>] [--profile=<profile>]
         [--save-only-mask | --save-only-cleaned | --save-only-text]
         [--separate-noise-mask] [--hide-analytics] [--extract-text]
-        [--skip-text-detection] [--skip-pre-processing] [--skip-cleaning] [--skip-denoising]
+        [--skip-text-detection] [--skip-pre-processing] [--skip-masking] [--skip-denoising]
         [--keep-cache] [--cache-masks] [--debug]
     pcleaner profile (list | new <profile_name> [<profile_path>] | add <profile_name> <profile_path> |
         open <profile_name> | delete <profile_name> | set-default <profile_name> | repair <profile_name> |
         purge-missing) [--debug]
     pcleaner gui [<image_path> ...] [--debug]
-    pcleaner ocr [<image_path> ...] [--output-path=<output_path>] [--debug]
+    pcleaner ocr [<image_path> ...] [--output-path=<output_path>] [--cache-masks] [--debug]
     pcleaner config (show | open)
     pcleaner cache clear (all | models | cleaner)
     pcleaner load models [--cuda | --cpu | --both] [--force]
     pcleaner --help
     pcleaner --version
 
 Subcommands:
@@ -61,15 +61,15 @@
     -t --save-only-text             Save only the text from the image cut out of the original image. This will
                                     automatically set the --extract-text option.
     -e --extract-text               Extract the text bubbles from the original image. Essentially deleting everything
                                     except the text. The cleaning or denoising step must be run for this to work.
     -n --separate-noise-mask        Save the noise mask separately from the main mask.
     -T --skip-text-detection        Do not run the text detection AI model. This is step 1/4.
     -P --skip-pre-processing        Do not run data pre-processing. This is step 2/4.
-    -C --skip-cleaning              Do not run the cleaning process. This is step 3/4.
+    -M --skip-masking               Do not run the masking process. This is step 3/4.
     -D --skip-denoising             Do not run the denoising process. This an optional step 4/4.
     -s --cache-masks                Save the masks used to clean the image in the cache directory.
     -a --hide-analytics             Hide the analytics. These are the statistics about the
                                     cleaning accuracy.
     <profile_path>                  The path to the profile file to add.
     <profile_name>                  The saved name of the profile to open, delete, or set as default.
     --output-path=<output_path>     The path to save the OCR output file to.
@@ -117,15 +117,15 @@
 from logzero import logger, loglevel, DEBUG, INFO
 from tqdm import tqdm
 from natsort import natsorted
 import torch
 import tifffile
 
 from pcleaner import __version__
-import pcleaner.cleaner as cl
+import pcleaner.masker as cl
 import pcleaner.config as cfg
 import pcleaner.cli_utils as cli
 import pcleaner.pre_processor as pp
 import pcleaner.analytics as an
 import pcleaner.structures as st
 import pcleaner.profile_cli as pc
 import pcleaner.denoiser as dn
@@ -183,15 +183,15 @@
             raise ValueError("Invalid profile subcommand.")
     elif args.gui:
         gui.launch(args.image_path)
 
     elif args.ocr:
         config = cfg.load_config()
         image_paths = discover_all_images(args.image_path)
-        run_ocr(config, image_paths, args.output_path)
+        run_ocr(config, image_paths, args.output_path, cache_masks=args.cache_masks)
 
     elif args.cache and args.clear:
         config = cfg.load_config()
         clear_cache(config, args.all, args.models, args.cleaner)
 
     elif args.load and args.models:
         config = cfg.load_config()
@@ -221,15 +221,15 @@
         start = time.time()
         run_cleaner(
             image_paths=args.image_path,
             output_dir=args.output_dir,
             config=config,
             skip_text_detection=args.skip_text_detection,
             skip_pre_processing=args.skip_pre_processing,
-            skip_cleaning=args.skip_cleaning,
+            skip_masking=args.skip_masking,
             skip_denoising=args.skip_denoising,
             save_only_mask=args.save_only_mask,
             save_only_cleaned=args.save_only_cleaned,
             save_only_text=args.save_only_text,
             extract_text=args.extract_text,
             cache_masks=args.cache_masks,
             separate_noise_mask=args.separate_noise_mask,
@@ -247,50 +247,50 @@
 
 def run_cleaner(
     image_paths: list[Path],
     output_dir: Path,
     config: cfg.Config,
     skip_text_detection: bool,
     skip_pre_processing: bool,
-    skip_cleaning: bool,
+    skip_masking: bool,
     skip_denoising: bool,
     save_only_mask: bool,
     save_only_cleaned: bool,
     save_only_text: bool,
     extract_text: bool,
     cache_masks: bool,
     separate_noise_mask: bool,
     hide_analytics: bool,
     keep_cache: bool,
     debug: bool,
 ):
     """
-    Run the cleaner on the given images.
+    Run the masker on the given images.
 
     :param image_paths: The paths to the images to clean.
     :param output_dir: The directory to save the output files to.
     :param config: The config to use.
     :param skip_text_detection: Whether to skip the text detection step.
     :param skip_pre_processing: Whether to skip the pre-processing step.
-    :param skip_cleaning: Whether to skip the cleaning step.
+    :param skip_masking: Whether to skip the masking step.
     :param skip_denoising: Whether to skip the denoising step.
     :param save_only_mask: Whether to save only the mask.
     :param save_only_cleaned: Whether to save only the cleaned image.
     :param save_only_text: Whether to save only the text.
     :param extract_text: Whether to extract the text from the image.
     :param cache_masks: Whether to save the masks used to clean the image in the cache directory.
     :param separate_noise_mask: Whether to save the noise mask separately.
     :param hide_analytics: Whether to hide the analytics.
     :param keep_cache: Whether to keep the cache directory for the text detection step.
     :param debug: Whether to show debug information.
     """
     profile = config.current_profile
 
     # Catch jokesters who want to skip all 4 steps.
-    if skip_text_detection and skip_pre_processing and skip_cleaning and skip_denoising:
+    if skip_text_detection and skip_pre_processing and skip_masking and skip_denoising:
         print("Well how about that, you want to skip all 4 steps? I guess I'm not needed here.")
         return
 
     cache_dir = config.get_cleaner_cache_dir()
     logger.debug(f"Cache directory: {cache_dir}")
 
     # If caching masks, direct the user to the cache directory.
@@ -351,51 +351,51 @@
             )
             if ocr_analytic:
                 ocr_analytics.append(ocr_analytic)
 
         if ocr_analytics and not hide_analytics:
             an.show_ocr_analytics(ocr_analytics, profile.pre_processor.ocr_max_size)
 
-    if not skip_cleaning:
-        print("Running Cleaner...")
+    if not skip_masking:
+        print("Running Masker...")
         # Read the json files in the image directory.
         json_files = Path(cache_dir).glob("*_clean.json")
 
         # When denoising, we don't immediately output the cleaned image.
         # But when not, we do, since denoising is optional.
         if not skip_denoising:
-            cleaner_output_dir = None
+            masker_output_dir = None
         else:
-            cleaner_output_dir = output_dir
+            masker_output_dir = output_dir
 
         # Zip together the json files and the out path thing.
         data = [
-            st.CleanerData(
+            st.MaskerData(
                 json_file,
-                cleaner_output_dir,
+                masker_output_dir,
                 cache_dir,
                 profile.general,
-                profile.cleaner,
+                profile.masker,
                 save_only_mask,
                 save_only_cleaned,
                 save_only_text,
                 extract_text,
                 cache_masks,
                 debug,
             )
             for json_file in json_files
         ]
 
-        cleaner_analytics_raw = []
+        masker_analytics_raw = []
         with Pool() as pool:
             for analytic in tqdm(pool.imap(cl.clean_page, data), total=len(data)):
-                cleaner_analytics_raw.extend(analytic)
+                masker_analytics_raw.extend(analytic)
 
-        if not hide_analytics and cleaner_analytics_raw:
-            an.show_cleaner_analytics(cleaner_analytics_raw)
+        if not hide_analytics and masker_analytics_raw:
+            an.show_masker_analytics(masker_analytics_raw)
 
     if not skip_denoising:
         print("Running Denoiser...")
         # Read the json files in the image directory.
         json_files = Path(cache_dir).glob("*_mask_data.json")
 
         # Zip together the json files and the out path thing.
@@ -421,33 +421,42 @@
             for analytic in tqdm(pool.imap(dn.denoise_page, data), total=len(data)):
                 denoise_analytics_raw.append(analytic)
 
         if not hide_analytics and denoise_analytics_raw:
             an.show_denoise_analytics(
                 denoise_analytics_raw,
                 profile.denoiser.noise_min_standard_deviation,
-                profile.cleaner.mask_max_standard_deviation,
+                profile.masker.mask_max_standard_deviation,
             )
 
         print("Done!")
 
 
-def run_ocr(config: cfg.Config, image_paths: list[Path], output_path: str | None):
+def run_ocr(
+    config: cfg.Config, image_paths: list[Path], output_path: str | None, cache_masks: bool
+):
     """
     Run OCR on the given images. This is a byproduct of the pre-processing step,
     expanded to all bubbles.
 
     :param config: The config to use.
     :param image_paths: The images to run OCR on.
     :param output_path: The path to output the results to.
+    :param cache_masks: Whether to cache the masks.
     """
     cache_dir = config.get_cleaner_cache_dir()
     profile = config.current_profile
     logger.debug(f"Cache directory: {cache_dir}")
 
+    # If caching masks, direct the user to the cache directory.
+    if cache_masks:
+        print(
+            f"You can find the masks being generated in real-time in the cache directory:\n\n{cache_dir}\n"
+        )
+
     # Delete the cache directory if not explicitly keeping it.
     if len(list(cache_dir.glob("*"))) > 0:
         cli.empty_cache_dir(cache_dir)
     # Get the model file, downloading it if necessary.
     cuda = torch.cuda.is_available()
     model_path = config.get_model_path(cuda)
 
@@ -480,16 +489,17 @@
 
     mocr = MangaOcr()
     ocr_analytics = []
     for json_file_path in tqdm(list(cache_dir.glob("*.json"))):
         ocr_analytic = pp.prep_json_file(
             json_file_path,
             pre_processor_conf=config.current_profile.pre_processor,
-            cache_masks=False,
+            cache_masks=cache_masks,
             mocr=mocr,
+            cache_masks_ocr=True,
         )
         if ocr_analytic:
             ocr_analytics.append(ocr_analytic)
 
     # Output the OCRed text from the analytics.
     removed_texts = list(itertools.chain.from_iterable(a[3] for a in ocr_analytics))
```

### Comparing `pcleaner-1.5.4/pcleaner/model_downloader.py` & `pcleaner-1.6.0/pcleaner/model_downloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/pre_processor.py` & `pcleaner-1.6.0/pcleaner/pre_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 
 def prep_json_file(
     json_file_path: Path,
     pre_processor_conf: cfg.PreProcessorConfig,
     cache_masks: bool,
     mocr: MangaOcr | None = None,
+    cache_masks_ocr: bool = False,
 ) -> tuple[int, tuple[int, ...], tuple[int, ...], tuple[tuple[str, str], ...]] | None:
     """
     Load the generated json file, and clean the data, leaving only the
     relevant data for the following steps.
 
     Check that this file wasn't already processed, and if it was, skip it.
     Processed json files have the file name ending with '_clean.json'.
@@ -55,14 +56,15 @@
 
     Analytics data is returned if the manga ocr object is given.
 
     :param json_file_path: Path to the json file.
     :param pre_processor_conf: Pre processor configuration, part of the profile.
     :param cache_masks: Whether to cache the masks.
     :param mocr: [Optional] Manga ocr object.
+    :param cache_masks_ocr: [Optional] Whether to cache the masks early for ocr.
     :return: Analytics data if the manga ocr object is given, None otherwise.
     """
 
     # Check if the file was already processed.
     if json_file_path.name.endswith("_clean.json"):
         return
     if json_file_path.name.endswith("_mask_data.json"):
@@ -87,33 +89,40 @@
             # Sussy box. Discard if it's too small.
             if data["language"] == "unknown" and box_size < scale_area(
                 pre_processor_conf.suspicious_box_min_size
             ):
                 continue
             boxes.append(data["xyxy"])
 
+    # Sort boxes by their x+y coordinates, using the top right corner as the reference.
+    boxes.sort(key=lambda box: box[1] - 0.4 * box[2])
+
     page_data = st.PageData(image_path, mask_path, original_path, scale, boxes, [], [], [])
 
+    # Pad the boxes a bit, save a copy, and then pad them some more.
+    # The copy is used as a smaller mask, and the padded copy is used as a larger mask.
+    page_data.grow_boxes(scale_len(pre_processor_conf.box_padding_initial), st.BoxType.BOX)
+    page_data.right_pad_boxes(
+        scale_len(pre_processor_conf.box_right_padding_initial), st.BoxType.BOX
+    )
+
+    # Draw the boxes on the image and save it.
+    if cache_masks and cache_masks_ocr:
+        page_data.visualize(Path(page_data.image_path))
+
     # Run OCR to discard small boxes that only contain symbols.
     analytics = None
     if mocr is not None:
         page_data, analytics = ocr_check(
             page_data,
             mocr,
             scale_area(pre_processor_conf.ocr_max_size),
             pre_processor_conf.ocr_blacklist_pattern,
         )
 
-    # Pad the boxes a bit, save a copy, and then pad them some more.
-    # The copy is used as a smaller mask, and the padded copy is used as a larger mask.
-    page_data.grow_boxes(scale_len(pre_processor_conf.box_padding_initial), st.BoxType.BOX)
-    page_data.right_pad_boxes(
-        scale_len(pre_processor_conf.box_right_padding_initial), st.BoxType.BOX
-    )
-
     # A shallow copy of the box list suffices, because the tuples inside are immutable.
     page_data.extended_boxes = page_data.boxes.copy()
 
     page_data.grow_boxes(
         scale_len(pre_processor_conf.box_padding_extended), st.BoxType.EXTENDED_BOX
     )
     page_data.right_pad_boxes(
@@ -134,22 +143,26 @@
     json_out_path = json_file_path.parent / f"{json_file_path.stem}_clean.json"
     # Remove the _image_size attribute, because it's a cached value that may be unset.
     page_data_dict = asdict(page_data)
     del page_data_dict["_image_size"]
     json_out_path.write_text(json.dumps(page_data_dict, indent=4))
 
     # Draw the boxes on the image and save it.
-    if cache_masks:
+    if cache_masks and not cache_masks_ocr:
         page_data.visualize(Path(page_data.image_path))
 
     return analytics
 
 
 def ocr_check(
-    page_data: st.PageData, mocr: MangaOcr, max_box_size: int, ocr_blacklist_pattern: str
+    page_data: st.PageData,
+    mocr: MangaOcr,
+    max_box_size: int,
+    ocr_blacklist_pattern: str,
+    box_padding: int = 0,
 ) -> tuple[st.PageData, tuple[int, tuple[int, ...], tuple[int, ...], tuple[tuple[str, str], ...]]]:
     """
     Run OCR on small boxes to determine whether they contain mere symbols,
     in which case these boxes do not need to be cleaned and can be removed
     from the dataset.
 
     The page_data object is modified in place.
@@ -163,17 +176,19 @@
     (Returning the page data isn't strictly necessary, since it's modified in place,
     but this makes that fact more explicit.)
 
     :param page_data: PageData object containing the data for the page.
     :param mocr: Manga ocr object.
     :param max_box_size: Maximum size of a box in pixels, to consider it for ocr.
     :param ocr_blacklist_pattern: Regex pattern to match against the ocr result.
+    :param box_padding: [Optional] Padding to add to the box before running ocr.
     :return: The modified page data and Analytics data.
     """
     base_image = Image.open(page_data.image_path)
+    image_width, image_height = base_image.size
     candidate_small_bubbles = [
         box for box in page_data.boxes if page_data.box_size(box) < max_box_size
     ]
     if not candidate_small_bubbles:
         return page_data, (len(page_data.boxes), (), (), ())
     # Check if the small bubbles only contain symbols.
     # If they do, then they are probably not text.
```

### Comparing `pcleaner-1.5.4/pcleaner/profile_cli.py` & `pcleaner-1.6.0/pcleaner/profile_cli.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.5.4/pcleaner/structures.py` & `pcleaner-1.6.0/pcleaner/structures.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
 import re
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
+from importlib import resources
+from pcleaner import data
 
 import magic
-from PIL import Image, ImageDraw
+from PIL import Image, ImageDraw, ImageFont
 
 import pcleaner.config as cfg
 
 
 class BoxType(Enum):
     BOX = 0
     EXTENDED_BOX = 1
@@ -144,16 +146,34 @@
 
         :param image_path: The path to the image to visualize the boxes on.
         :param out_dir: [Optional] The directory to save the visualization to.
             By default, the visualization is saved to the same directory as the image.
         """
         image = Image.open(image_path)
         draw = ImageDraw.Draw(image)
-        for box in self.boxes:
+        font_path = str(resources.path(data, "LiberationSans-Regular.ttf"))
+        # Figure out the optimal font size based on the image size. E.g. 30 for a 1600px image.
+        font_size = int(image.size[0] / 50)
+
+        for index, box in enumerate(self.boxes):
             draw.rectangle(box, outline="green")
+            # Draw the box number, with a white background, respecting font size.
+            draw.rectangle(
+                (box[2] - font_size, box[1] + 2, box[2] - 2, box[1] + font_size),
+                fill="white",
+                outline="white",
+            )
+            draw.text(
+                (box[2] - font_size, box[1]),
+                str(index + 1),
+                fill="green",
+                font=ImageFont.truetype(font_path, font_size),
+                direction="rtl",
+            )
+
         for box in self.extended_boxes:
             draw.rectangle(box, outline="red")
         for box in self.merged_extended_boxes:
             draw.rectangle(box, outline="purple")
         for box in self.reference_boxes:
             draw.rectangle(box, outline="blue")
         # Save the image.
@@ -258,36 +278,36 @@
 
     @property
     def noise_mask_data(self) -> tuple[tuple[int, int, int, int], float]:
         return self.mask_box, self.analytics_std_deviation
 
 
 @dataclass
-class CleanerData:
+class MaskerData:
     """
-    This is a simple struct to hold the inputs for the cleaner.
+    This is a simple struct to hold the inputs for the masker.
     The data is a tuple of:
     - The json file path.
     - The image output directory. When none, output to the cache dir for denoising to continue.
     - The image cache directory.
     - The general config.
-    - The cleaner config.
+    - The masker config.
     - The save only mask flag.
     - The save only cleaned flag.
     - The save only text flag.
     - The extract text flag.
     - The show masks flag. (when true, save intermediate masks to the cache directory)
     - The debug flag.
     """
 
     json_path: Path
     output_dir: Path | None
     cache_dir: Path
     general_config: cfg.GeneralConfig
-    cleaner_config: cfg.CleanerConfig
+    masker_config: cfg.MaskerConfig
     save_only_mask: bool
     save_only_cleaned: bool
     save_only_text: bool
     extract_text: bool
     show_masks: bool
     debug: bool
```

### Comparing `pcleaner-1.5.4/pcleaner.egg-info/PKG-INFO` & `pcleaner-1.6.0/pcleaner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.5.4
+Version: 1.6.0
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pcleaner-1.5.4/pcleaner.egg-info/SOURCES.txt` & `pcleaner-1.6.0/pcleaner.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 pcleaner/__init__.py
 pcleaner/analytics.py
-pcleaner/cleaner.py
 pcleaner/cli_utils.py
 pcleaner/config.py
 pcleaner/ctd_interface.py
 pcleaner/denoiser.py
 pcleaner/helpers.py
 pcleaner/image_ops.py
 pcleaner/main.py
+pcleaner/masker.py
 pcleaner/model_downloader.py
 pcleaner/pre_processor.py
 pcleaner/profile_cli.py
 pcleaner/structures.py
 pcleaner.egg-info/PKG-INFO
 pcleaner.egg-info/SOURCES.txt
 pcleaner.egg-info/dependency_links.txt
@@ -37,19 +37,22 @@
 pcleaner/comic_text_detector/utils/imgproc_utils.py
 pcleaner/comic_text_detector/utils/io_utils.py
 pcleaner/comic_text_detector/utils/loss.py
 pcleaner/comic_text_detector/utils/textblock.py
 pcleaner/comic_text_detector/utils/textmask.py
 pcleaner/comic_text_detector/utils/weight_init.py
 pcleaner/comic_text_detector/utils/yolov5_utils.py
+pcleaner/data/__init__.py
 pcleaner/gui/__init__.py
 pcleaner/gui/file_table.py
 pcleaner/gui/launcher.py
 pcleaner/gui/mainwindow_driver.py
+pcleaner/gui/profile_parser.py
 pcleaner/gui/worker_thread.py
+pcleaner/gui/CustomQ/CComboBox.py
 pcleaner/gui/CustomQ/CTableWidget.py
 pcleaner/gui/CustomQ/__init__.py
 pcleaner/gui/rc_generated_files/__init__.py
 pcleaner/gui/rc_generated_files/icons_rc.py
 pcleaner/gui/ui_generated_files/__init__.py
 pcleaner/gui/ui_generated_files/ui_ImageDetails.py
 pcleaner/gui/ui_generated_files/ui_Mainwindow.py
```

### Comparing `pcleaner-1.5.4/setup.cfg` & `pcleaner-1.6.0/setup.cfg`

 * *Files identical despite different names*

