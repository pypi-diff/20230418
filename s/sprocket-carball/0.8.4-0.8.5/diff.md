# Comparing `tmp/sprocket_carball-0.8.4.linux-x86_64.tar.gz` & `tmp/sprocket_carball-0.8.5.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocket_carball-0.8.4.linux-x86_64.tar", last modified: Tue Apr 18 17:38:08 2023, max compression
+gzip compressed data, was "sprocket_carball-0.8.5.linux-x86_64.tar", last modified: Tue Apr 18 17:40:35 2023, max compression
```

## Comparing `sprocket_carball-0.8.4.linux-x86_64.tar` & `sprocket_carball-0.8.5.linux-x86_64.tar`

### file list

```diff
@@ -1,368 +1,368 @@
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.395659 ./
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.395659 ./usr/
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.735660 ./usr/local/
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.735660 ./usr/local/bin/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      984 2023-04-18 17:38:08.735660 ./usr/local/bin/carball
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.395659 ./usr/local/lib/
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.395659 ./usr/local/lib/python3.10/
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.691660 ./usr/local/lib/python3.10/dist-packages/
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.519659 ./usr/local/lib/python3.10/dist-packages/carball/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.176219 ./
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.176219 ./usr/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.552220 ./usr/local/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.552220 ./usr/local/bin/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      984 2023-04-18 17:40:35.552220 ./usr/local/bin/carball
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.176219 ./usr/local/lib/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.176219 ./usr/local/lib/python3.10/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.512220 ./usr/local/lib/python3.10/dist-packages/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      223 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.679660 ./usr/local/lib/python3.10/dist-packages/carball/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      403 2023-04-18 17:38:08.519659 ./usr/local/lib/python3.10/dist-packages/carball/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2197 2023-04-18 17:38:08.643660 ./usr/local/lib/python3.10/dist-packages/carball/__pycache__/command_line.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2563 2023-04-18 17:38:08.679660 ./usr/local/lib/python3.10/dist-packages/carball/__pycache__/decompile_replays.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.527660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.500220 ./usr/local/lib/python3.10/dist-packages/carball/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      403 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2197 2023-04-18 17:40:35.464220 ./usr/local/lib/python3.10/dist-packages/carball/__pycache__/command_line.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2563 2023-04-18 17:40:35.500220 ./usr/local/lib/python3.10/dist-packages/carball/__pycache__/decompile_replays.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        2 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/PROTOBUF_VERSION
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.607660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      161 2023-04-18 17:38:08.527660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    15971 2023-04-18 17:38:08.607660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/__pycache__/analysis_manager.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.432220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      161 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    15971 2023-04-18 17:40:35.432220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/__pycache__/analysis_manager.cpython-310.pyc
 -rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    17254 2023-04-16 06:18:49.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/analysis_manager.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.531659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.531659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      169 2023-04-18 17:38:08.531659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1555 2023-04-18 17:38:08.531659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/__pycache__/cleaner.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2221 2023-04-18 17:38:08.531659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/__pycache__/frame_cleaner.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      169 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1555 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/__pycache__/cleaner.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2221 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/__pycache__/frame_cleaner.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1383 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/cleaner.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2295 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/frame_cleaner.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.523659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.527660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      171 2023-04-18 17:38:08.523659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1044 2023-04-18 17:38:08.523659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/basic_math.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3288 2023-04-18 17:38:08.523659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/dropshot.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5196 2023-04-18 17:38:08.523659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/field_constants.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1276 2023-04-18 17:38:08.527660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/playlist.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      171 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1044 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/basic_math.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3288 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/dropshot.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5196 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/field_constants.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1276 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/playlist.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      815 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/basic_math.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5721 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/dropshot.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6198 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/field_constants.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1187 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/playlist.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.579660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.400220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.599660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      168 2023-04-18 17:38:08.579660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8945 2023-04-18 17:38:08.599660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/__pycache__/carry_detection.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5292 2023-04-18 17:38:08.595660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/__pycache__/event_creator.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.595660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.424220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      168 2023-04-18 17:40:35.400220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8945 2023-04-18 17:40:35.424220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/__pycache__/carry_detection.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5292 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/__pycache__/event_creator.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.420220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.599660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      188 2023-04-18 17:38:08.595660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2521 2023-04-18 17:38:08.599660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/__pycache__/pickup_analysis.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.420220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      188 2023-04-18 17:40:35.420220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2521 2023-04-18 17:40:35.420220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/__pycache__/pickup_analysis.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3707 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/pickup_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.591660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.591660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      183 2023-04-18 17:38:08.591660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1999 2023-04-18 17:38:08.591660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/__pycache__/bump_analysis.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      183 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1999 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/__pycache__/bump_analysis.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1277 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/bump_analysis.py
 -rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    15129 2023-04-18 17:32:26.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/carry_detection.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.595660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.595660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      177 2023-04-18 17:38:08.595660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1434 2023-04-18 17:38:08.595660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/__pycache__/ball.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1016 2023-04-18 17:38:08.595660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/__pycache__/damage.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.420220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      177 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1434 2023-04-18 17:40:35.420220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/__pycache__/ball.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1016 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/__pycache__/damage.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1386 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/ball.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      935 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/damage.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5568 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/event_creator.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.587660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.587660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      180 2023-04-18 17:38:08.587660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4274 2023-04-18 17:38:08.587660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/__pycache__/fifty_analysis.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      180 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4274 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/__pycache__/fifty_analysis.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7419 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/fifty_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.579660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.400220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.583660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      182 2023-04-18 17:38:08.579660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8113 2023-04-18 17:38:08.583660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/__pycache__/base_hit.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6535 2023-04-18 17:38:08.579660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/__pycache__/hit_analysis.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.404219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      182 2023-04-18 17:40:35.404219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8113 2023-04-18 17:40:35.404219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/__pycache__/base_hit.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6535 2023-04-18 17:40:35.400220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/__pycache__/hit_analysis.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11653 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/base_hit.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11223 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hit_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.583660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.404219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    41555 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/Vehicle Specifications v1.39 - Hitboxes, Handling.xlsx
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.583660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      189 2023-04-18 17:38:08.583660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2218 2023-04-18 17:38:08.583660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/__pycache__/car.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1733 2023-04-18 17:38:08.583660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/__pycache__/hitbox.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      189 2023-04-18 17:40:35.404219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2218 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/__pycache__/car.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1733 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/__pycache__/hitbox.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1662 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/car.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1973 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/hitbox.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.587660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.587660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      181 2023-04-18 17:38:08.587660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3316 2023-04-18 17:38:08.587660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/__pycache__/pressure_analysis.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.412220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      181 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3316 2023-04-18 17:40:35.412220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/__pycache__/pressure_analysis.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3373 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/pressure_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.591660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.412220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.591660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      186 2023-04-18 17:38:08.591660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6871 2023-04-18 17:38:08.591660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/__pycache__/kickoff_analysis.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.412220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      186 2023-04-18 17:40:35.412220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6871 2023-04-18 17:40:35.412220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/__pycache__/kickoff_analysis.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10002 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/kickoff_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.531659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.543660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      173 2023-04-18 17:38:08.535659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3073 2023-04-18 17:38:08.543660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/__pycache__/saltie_game.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.535659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      173 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3073 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/__pycache__/saltie_game.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      459 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiDemo.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2531 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiGame.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      383 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiGoal.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      479 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiMutators.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1473 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiPlayer.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1406 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiPlayerCameraSettings.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3124 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiPlayerLoadout.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      681 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiTeam.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.539659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      820 2023-04-18 17:38:08.539659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiDemo.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2370 2023-04-18 17:38:08.535659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiGame.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      765 2023-04-18 17:38:08.535659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiGoal.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      840 2023-04-18 17:38:08.539659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiMutators.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1210 2023-04-18 17:38:08.535659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiPlayer.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      991 2023-04-18 17:38:08.539659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiPlayerCameraSettings.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1816 2023-04-18 17:38:08.539659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiPlayerLoadout.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      977 2023-04-18 17:38:08.539659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiTeam.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      182 2023-04-18 17:38:08.535659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/__init__.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      820 2023-04-18 17:40:35.360219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiDemo.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2370 2023-04-18 17:40:35.360219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiGame.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      765 2023-04-18 17:40:35.360219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiGoal.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      840 2023-04-18 17:40:35.360219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiMutators.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1210 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiPlayer.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      991 2023-04-18 17:40:35.360219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiPlayerCameraSettings.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1816 2023-04-18 17:40:35.360219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiPlayerLoadout.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      977 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiTeam.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      182 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/__init__.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4703 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/saltie_game.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.603660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.424220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.607660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      171 2023-04-18 17:38:08.603660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6240 2023-04-18 17:38:08.603660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__pycache__/ball_simulator.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      830 2023-04-18 17:38:08.607660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__pycache__/bounce.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      409 2023-04-18 17:38:08.603660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__pycache__/map_constants.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.428220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      171 2023-04-18 17:40:35.424220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6240 2023-04-18 17:40:35.424220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__pycache__/ball_simulator.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      830 2023-04-18 17:40:35.428220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__pycache__/bounce.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      409 2023-04-18 17:40:35.428220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__pycache__/map_constants.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11609 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/ball_simulator.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      855 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/bounce.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      238 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/map_constants.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.543660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.559660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      167 2023-04-18 17:38:08.543660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4771 2023-04-18 17:38:08.559660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__pycache__/stats.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3469 2023-04-18 17:38:08.547659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__pycache__/stats_list.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3938 2023-04-18 17:38:08.547659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__pycache__/stats_manager.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.543660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.384220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      167 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4771 2023-04-18 17:40:35.384220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__pycache__/stats.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3469 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__pycache__/stats_list.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3938 2023-04-18 17:40:35.372219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__pycache__/stats_manager.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.543660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      180 2023-04-18 17:38:08.543660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1476 2023-04-18 17:38:08.543660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/__pycache__/distance_hit_ball_forward.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      180 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1476 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/__pycache__/distance_hit_ball_forward.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1023 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/distance_hit_ball_forward.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.571660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.575660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      173 2023-04-18 17:38:08.571660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5035 2023-04-18 17:38:08.575660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/__pycache__/boost.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.396220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      173 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5035 2023-04-18 17:40:35.396220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/__pycache__/boost.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6918 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/boost.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.547659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.547659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      176 2023-04-18 17:38:08.547659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2607 2023-04-18 17:38:08.547659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/__pycache__/controls.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      176 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2607 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/__pycache__/controls.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2829 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/controls.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.559660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.380220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.559660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      173 2023-04-18 17:38:08.559660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1646 2023-04-18 17:38:08.559660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/__pycache__/demos.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.384220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      173 2023-04-18 17:40:35.380220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1646 2023-04-18 17:40:35.380220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/__pycache__/demos.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1623 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/demos.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.567659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.571660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      176 2023-04-18 17:38:08.571660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2416 2023-04-18 17:38:08.571660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/__pycache__/ball_carry.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      176 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2416 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/__pycache__/ball_carry.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3342 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/ball_carry.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.547659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.372219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      343 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.551659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      562 2023-04-18 17:38:08.547659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2194 2023-04-18 17:38:08.551659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__pycache__/ball_phase_times.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3268 2023-04-18 17:38:08.551659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__pycache__/damage.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3043 2023-04-18 17:38:08.551659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__pycache__/goals.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.376219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      562 2023-04-18 17:40:35.372219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2194 2023-04-18 17:40:35.376219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__pycache__/ball_phase_times.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3268 2023-04-18 17:40:35.372219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__pycache__/damage.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3043 2023-04-18 17:40:35.372219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__pycache__/goals.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2082 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/ball_phase_times.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3902 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/damage.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2575 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/goals.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.571660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.571660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      176 2023-04-18 17:38:08.571660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2132 2023-04-18 17:38:08.571660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/__pycache__/kickoff_stat.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      176 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2132 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/__pycache__/kickoff_stat.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2211 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/kickoff_stat.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.551659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.376219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.559660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      178 2023-04-18 17:38:08.551659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3319 2023-04-18 17:38:08.555660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/ball_distances.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7520 2023-04-18 17:38:08.559660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/per_possession.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2528 2023-04-18 17:38:08.555660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/possession.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2156 2023-04-18 17:38:08.555660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/turnovers.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.380220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      178 2023-04-18 17:40:35.376219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3319 2023-04-18 17:40:35.376219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/ball_distances.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7520 2023-04-18 17:40:35.380220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/per_possession.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2528 2023-04-18 17:40:35.380220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/possession.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2156 2023-04-18 17:40:35.376219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/turnovers.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3521 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/ball_distances.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10214 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/per_possession.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2982 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/possession.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2243 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/turnovers.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.575660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.396220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.579660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      174 2023-04-18 17:38:08.575660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3323 2023-04-18 17:38:08.575660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/__pycache__/goals.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7112 2023-04-18 17:38:08.575660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/__pycache__/rumble.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.400220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      174 2023-04-18 17:40:35.396220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3323 2023-04-18 17:40:35.400220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/__pycache__/goals.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7112 2023-04-18 17:40:35.396220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/__pycache__/rumble.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3475 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/goals.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     8977 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/rumble.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4033 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/stats.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3336 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/stats_list.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3851 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/stats_manager.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.563660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.384220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.567659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      178 2023-04-18 17:38:08.563660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1851 2023-04-18 17:38:08.567659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/averages.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2010 2023-04-18 17:38:08.563660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/hit_counts.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6267 2023-04-18 17:38:08.563660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/positional_tendencies.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2519 2023-04-18 17:38:08.567659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/relative_position_tendencies.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2084 2023-04-18 17:38:08.567659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/speed_tendencies.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5290 2023-04-18 17:38:08.567659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/team_tendencies.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      178 2023-04-18 17:40:35.384220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1851 2023-04-18 17:40:35.388219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/averages.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2010 2023-04-18 17:40:35.384220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/hit_counts.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6267 2023-04-18 17:40:35.384220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/positional_tendencies.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2519 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/relative_position_tendencies.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2084 2023-04-18 17:40:35.388219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/speed_tendencies.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5290 2023-04-18 17:40:35.388219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/team_tendencies.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1330 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/averages.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1583 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/hit_counts.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6969 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/positional_tendencies.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2777 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/relative_position_tendencies.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1962 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/speed_tendencies.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6502 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/team_tendencies.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.543660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.543660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      173 2023-04-18 17:38:08.543660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1876 2023-04-18 17:38:08.543660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/__pycache__/pandas_utils.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      173 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1876 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/__pycache__/pandas_utils.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1708 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/pandas_utils.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.527660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.531659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      167 2023-04-18 17:38:08.527660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      632 2023-04-18 17:38:08.531659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/json_encoder.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2173 2023-04-18 17:38:08.531659 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/numpy_manager.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2371 2023-04-18 17:38:08.527660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/pandas_manager.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      858 2023-04-18 17:38:08.527660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/proto_manager.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1398 2023-04-18 17:38:08.527660 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/split_location.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      167 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      632 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/json_encoder.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2173 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/numpy_manager.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2371 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/pandas_manager.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      858 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/proto_manager.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1398 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/split_location.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      316 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/json_encoder.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1974 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/numpy_manager.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2050 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/pandas_manager.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      374 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/proto_manager.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1265 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/split_location.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2558 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/command_line.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.611660 ./usr/local/lib/python3.10/dist-packages/carball/controls/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.432220 ./usr/local/lib/python3.10/dist-packages/carball/controls/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/controls/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.611660 ./usr/local/lib/python3.10/dist-packages/carball/controls/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      161 2023-04-18 17:38:08.611660 ./usr/local/lib/python3.10/dist-packages/carball/controls/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1762 2023-04-18 17:38:08.611660 ./usr/local/lib/python3.10/dist-packages/carball/controls/__pycache__/controls.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2743 2023-04-18 17:38:08.611660 ./usr/local/lib/python3.10/dist-packages/carball/controls/__pycache__/rotations.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.432220 ./usr/local/lib/python3.10/dist-packages/carball/controls/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      161 2023-04-18 17:40:35.432220 ./usr/local/lib/python3.10/dist-packages/carball/controls/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1762 2023-04-18 17:40:35.432220 ./usr/local/lib/python3.10/dist-packages/carball/controls/__pycache__/controls.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2743 2023-04-18 17:40:35.432220 ./usr/local/lib/python3.10/dist-packages/carball/controls/__pycache__/rotations.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2203 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/controls/controls.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3427 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/controls/rotations.py
 -rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2586 2023-04-16 23:12:44.000000 ./usr/local/lib/python3.10/dist-packages/carball/decompile_replays.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.643660 ./usr/local/lib/python3.10/dist-packages/carball/extras/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/extras/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/extras/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.647660 ./usr/local/lib/python3.10/dist-packages/carball/extras/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      159 2023-04-18 17:38:08.647660 ./usr/local/lib/python3.10/dist-packages/carball/extras/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1846 2023-04-18 17:38:08.643660 ./usr/local/lib/python3.10/dist-packages/carball/extras/__pycache__/per_goal_analysis.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/extras/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      159 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/extras/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1846 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/extras/__pycache__/per_goal_analysis.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1770 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/extras/per_goal_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.519659 ./usr/local/lib/python3.10/dist-packages/carball/generated/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.519659 ./usr/local/lib/python3.10/dist-packages/carball/generated/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      162 2023-04-18 17:38:08.519659 ./usr/local/lib/python3.10/dist-packages/carball/generated/__pycache__/__init__.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.475659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.519659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      166 2023-04-18 17:38:08.479659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3007 2023-04-18 17:38:08.519659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/game_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1928 2023-04-18 17:38:08.515659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/party_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1678 2023-04-18 17:38:08.519659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/player_id_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3902 2023-04-18 17:38:08.479659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/player_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2350 2023-04-18 17:38:08.475659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/team_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5076 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/game_pb2.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.479659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.487659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      175 2023-04-18 17:38:08.483659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2686 2023-04-18 17:38:08.483659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/camera_settings_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8224 2023-04-18 17:38:08.487659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/game_metadata_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2670 2023-04-18 17:38:08.487659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/mutators_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5371 2023-04-18 17:38:08.483659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/player_loadout_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4653 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/camera_settings_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    19305 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/game_metadata_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3635 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/mutators_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    12482 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/player_loadout_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2397 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/party_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1793 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/player_id_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8237 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/player_pb2.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.487659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.515659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      172 2023-04-18 17:38:08.487659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2538 2023-04-18 17:38:08.495659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/ball_stats_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1428 2023-04-18 17:38:08.507659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/data_frame_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7293 2023-04-18 17:38:08.503659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/dropshot_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    11109 2023-04-18 17:38:08.495659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/events_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3266 2023-04-18 17:38:08.507659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/extra_mode_stats_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3649 2023-04-18 17:38:08.495659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/game_stats_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1708 2023-04-18 17:38:08.515659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/goal_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7994 2023-04-18 17:38:08.515659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/kickoff_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3677 2023-04-18 17:38:08.487659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/per_possession_stats_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    13364 2023-04-18 17:38:08.511659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/player_stats_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4030 2023-04-18 17:38:08.503659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/rumble_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8655 2023-04-18 17:38:08.499659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/stats_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4123 2023-04-18 17:38:08.499659 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/team_stats_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3714 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/ball_stats_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1383 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/data_frame_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    18134 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/dropshot_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    31534 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/events_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5766 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/extra_mode_stats_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6701 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/game_stats_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1837 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/goal_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    18809 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/kickoff_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7823 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/per_possession_stats_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    34767 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/player_stats_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7450 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/rumble_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    21715 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/stats_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7909 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/team_stats_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3568 2023-04-18 17:32:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/team_pb2.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.519659 ./usr/local/lib/python3.10/dist-packages/carball/generated/binaries/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/binaries/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.519659 ./usr/local/lib/python3.10/dist-packages/carball/generated/binaries/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      171 2023-04-18 17:38:08.519659 ./usr/local/lib/python3.10/dist-packages/carball/generated/binaries/__pycache__/__init__.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.611660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.340219 ./usr/local/lib/python3.10/dist-packages/carball/generated/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/generated/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      162 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/generated/__pycache__/__init__.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.340219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      166 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3007 2023-04-18 17:40:35.340219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/game_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1928 2023-04-18 17:40:35.340219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/party_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1678 2023-04-18 17:40:35.340219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/player_id_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3902 2023-04-18 17:40:35.304219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/player_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2350 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/team_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5076 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/game_pb2.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.304219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.312219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      175 2023-04-18 17:40:35.308219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2686 2023-04-18 17:40:35.308219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/camera_settings_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8224 2023-04-18 17:40:35.312219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/game_metadata_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2670 2023-04-18 17:40:35.312219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/mutators_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5371 2023-04-18 17:40:35.304219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/player_loadout_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4653 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/camera_settings_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    19305 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/game_metadata_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3635 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/mutators_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    12482 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/player_loadout_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2397 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/party_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1793 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/player_id_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8237 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/player_pb2.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.312219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.340219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      172 2023-04-18 17:40:35.312219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2538 2023-04-18 17:40:35.320219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/ball_stats_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1428 2023-04-18 17:40:35.328219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/data_frame_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7293 2023-04-18 17:40:35.328219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/dropshot_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    11109 2023-04-18 17:40:35.320219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/events_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3266 2023-04-18 17:40:35.332219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/extra_mode_stats_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3649 2023-04-18 17:40:35.320219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/game_stats_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1708 2023-04-18 17:40:35.340219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/goal_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7994 2023-04-18 17:40:35.336219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/kickoff_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3677 2023-04-18 17:40:35.312219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/per_possession_stats_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    13364 2023-04-18 17:40:35.336219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/player_stats_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4030 2023-04-18 17:40:35.328219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/rumble_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8655 2023-04-18 17:40:35.324219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/stats_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4123 2023-04-18 17:40:35.324219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/team_stats_pb2.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3714 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/ball_stats_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1383 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/data_frame_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    18134 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/dropshot_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    31534 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/events_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5766 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/extra_mode_stats_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6701 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/game_stats_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1837 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/goal_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    18809 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/kickoff_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7823 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/per_possession_stats_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    34767 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/player_stats_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7450 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/rumble_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    21715 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/stats_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7909 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/team_stats_pb2.py
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3568 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/team_pb2.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/generated/binaries/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/binaries/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/generated/binaries/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      171 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/generated/binaries/__pycache__/__init__.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.436220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.643660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      164 2023-04-18 17:38:08.615660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2934 2023-04-18 17:38:08.635660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/actor_parsing.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1372 2023-04-18 17:38:08.615660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/bots.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2895 2023-04-18 17:38:08.611660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/dropshot.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    10052 2023-04-18 17:38:08.623660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/frame_parser.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8300 2023-04-18 17:38:08.619660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/game.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1553 2023-04-18 17:38:08.615660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/game_info.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1285 2023-04-18 17:38:08.635660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/goal.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8156 2023-04-18 17:38:08.615660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/player.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1495 2023-04-18 17:38:08.643660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/team.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.623660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.464220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      164 2023-04-18 17:40:35.436220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2934 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/actor_parsing.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1372 2023-04-18 17:40:35.436220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/bots.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2895 2023-04-18 17:40:35.436220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/dropshot.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    10052 2023-04-18 17:40:35.444220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/frame_parser.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8300 2023-04-18 17:40:35.440220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/game.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1553 2023-04-18 17:40:35.440220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/game_info.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1285 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/goal.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8156 2023-04-18 17:40:35.436220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/player.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1495 2023-04-18 17:40:35.464220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/team.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.444220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      435 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.631660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      742 2023-04-18 17:38:08.623660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1718 2023-04-18 17:38:08.631660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/ball.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1788 2023-04-18 17:38:08.627660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/base.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2849 2023-04-18 17:38:08.631660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/boost.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1024 2023-04-18 17:38:08.631660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/camera.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2166 2023-04-18 17:38:08.627660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/car.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1774 2023-04-18 17:38:08.623660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/dropshot.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1315 2023-04-18 17:38:08.631660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/game_event.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      877 2023-04-18 17:38:08.627660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/game_info.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2110 2023-04-18 17:38:08.627660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/jump.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2345 2023-04-18 17:38:08.627660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/player.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1331 2023-04-18 17:38:08.623660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/rumble.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      929 2023-04-18 17:38:08.631660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/team.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      742 2023-04-18 17:40:35.444220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1718 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/ball.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1788 2023-04-18 17:40:35.452220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/base.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2849 2023-04-18 17:40:35.452220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/boost.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1024 2023-04-18 17:40:35.452220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/camera.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2166 2023-04-18 17:40:35.448220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/car.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1774 2023-04-18 17:40:35.444220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/dropshot.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1315 2023-04-18 17:40:35.452220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/game_event.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      877 2023-04-18 17:40:35.448220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/game_info.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2110 2023-04-18 17:40:35.448220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/jump.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2345 2023-04-18 17:40:35.448220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/player.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1331 2023-04-18 17:40:35.444220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/rumble.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      929 2023-04-18 17:40:35.452220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/team.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1649 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/ball.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1210 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/base.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4316 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/boost.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1053 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/camera.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3497 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/car.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1719 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/dropshot.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1034 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/game_event.py
@@ -375,121 +375,121 @@
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1374 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/bots.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2021 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/dropshot.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12747 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/frame_parser.py
 -rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    13147 2023-04-16 06:04:04.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/game.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1614 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/game_info.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      932 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/goal.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11640 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/player.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.639660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.639660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      177 2023-04-18 17:38:08.639660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1787 2023-04-18 17:38:08.639660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/__pycache__/sanity_check.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.635660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      177 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1787 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/__pycache__/sanity_check.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.639660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      189 2023-04-18 17:38:08.635660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1985 2023-04-18 17:38:08.639660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__pycache__/base_check.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      449 2023-04-18 17:38:08.635660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__pycache__/game_check.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      787 2023-04-18 17:38:08.635660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__pycache__/player_check.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      189 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1985 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__pycache__/base_check.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      449 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__pycache__/game_check.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      787 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__pycache__/player_check.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1261 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/base_check.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      117 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/game_check.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      298 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/player_check.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.639660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.643660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      184 2023-04-18 17:38:08.639660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1096 2023-04-18 17:38:08.643660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__pycache__/ball_data_frame_check.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1731 2023-04-18 17:38:08.643660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__pycache__/player_attributes_check.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1317 2023-04-18 17:38:08.639660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__pycache__/player_data_frame_check.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.464220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      184 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1096 2023-04-18 17:40:35.464220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__pycache__/ball_data_frame_check.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1731 2023-04-18 17:40:35.464220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__pycache__/player_attributes_check.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1317 2023-04-18 17:40:35.464220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__pycache__/player_data_frame_check.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      496 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/ball_data_frame_check.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1037 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/player_attributes_check.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      813 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/player_data_frame_check.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.639660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.639660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      184 2023-04-18 17:38:08.639660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      800 2023-04-18 17:38:08.639660 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/__pycache__/errors.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      184 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      800 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/__pycache__/errors.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      275 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/errors.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1459 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/sanity_check.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1195 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/team.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.647660 ./usr/local/lib/python3.10/dist-packages/carball/tests/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/tests/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.679660 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      158 2023-04-18 17:38:08.647660 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2990 2023-04-18 17:38:08.655660 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/analysis_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      358 2023-04-18 17:38:08.647660 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/conftest.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3174 2023-04-18 17:38:08.647660 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/export_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2688 2023-04-18 17:38:08.675660 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/game_creation_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1359 2023-04-18 17:38:08.675660 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/read_pandas_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      955 2023-04-18 17:38:08.679660 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/tiles_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     9954 2023-04-18 17:38:08.651660 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/utils.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.500220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      158 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2990 2023-04-18 17:40:35.476220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/analysis_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      358 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/conftest.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3174 2023-04-18 17:40:35.472220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/export_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2688 2023-04-18 17:40:35.496220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/game_creation_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1359 2023-04-18 17:40:35.496220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/read_pandas_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      955 2023-04-18 17:40:35.500220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/tiles_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     9954 2023-04-18 17:40:35.472220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/utils.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3666 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/analysis_test.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.647660 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.647660 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      171 2023-04-18 17:38:08.647660 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1219 2023-04-18 17:38:08.647660 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/__pycache__/benchmarking.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      171 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1219 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/__pycache__/benchmarking.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1577 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/benchmarking.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      124 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/conftest.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.655660 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.659660 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      163 2023-04-18 17:38:08.659660 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1615 2023-04-18 17:38:08.659660 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/__pycache__/data_frame_docs.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      163 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1615 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/__pycache__/data_frame_docs.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1610 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/data_frame_docs.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2641 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/export_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2791 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/game_creation_test.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.651660 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.472220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.655660 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      167 2023-04-18 17:38:08.651660 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1351 2023-04-18 17:38:08.655660 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/camera_settings_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1429 2023-04-18 17:38:08.655660 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/command_line_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1114 2023-04-18 17:38:08.651660 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/error_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2210 2023-04-18 17:38:08.655660 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/leader_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1010 2023-04-18 17:38:08.651660 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/offline_test.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.476220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      167 2023-04-18 17:40:35.472220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1351 2023-04-18 17:40:35.476220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/camera_settings_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1429 2023-04-18 17:40:35.476220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/command_line_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1114 2023-04-18 17:40:35.472220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/error_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2210 2023-04-18 17:40:35.476220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/leader_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1010 2023-04-18 17:40:35.476220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/offline_test.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1100 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/camera_settings_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      796 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/command_line_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      668 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/error_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2809 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/leader_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      635 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/offline_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      819 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/read_pandas_test.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.659660 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.675660 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      164 2023-04-18 17:38:08.659660 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5765 2023-04-18 17:38:08.663660 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/boost_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      988 2023-04-18 17:38:08.659660 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/demo_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    13203 2023-04-18 17:38:08.671660 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/dribble_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4887 2023-04-18 17:38:08.667660 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/dropshot_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2740 2023-04-18 17:38:08.659660 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/fifty_fifty_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5615 2023-04-18 17:38:08.663660 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/hit_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4318 2023-04-18 17:38:08.667660 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/kickoff_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6014 2023-04-18 17:38:08.675660 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/rumble_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1165 2023-04-18 17:38:08.671660 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/team_test.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.496220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      164 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5765 2023-04-18 17:40:35.484220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/boost_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      988 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/demo_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    13203 2023-04-18 17:40:35.492220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/dribble_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4887 2023-04-18 17:40:35.488220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/dropshot_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2740 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/fifty_fifty_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5615 2023-04-18 17:40:35.484220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/hit_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4318 2023-04-18 17:40:35.488220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/kickoff_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6014 2023-04-18 17:40:35.496220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/rumble_test.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1165 2023-04-18 17:40:35.492220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/team_test.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6280 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/boost_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      494 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/demo_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    16228 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/dribble_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     8308 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/dropshot_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2911 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/fifty_fifty_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6753 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/hit_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5648 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/kickoff_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10956 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/rumble_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      814 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/team_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      574 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/tiles_test.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12330 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/utils.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.691660 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.4-py3.10.egg-info/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6722 2023-04-18 17:38:08.059658 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.4-py3.10.egg-info/PKG-INFO
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8448 2023-04-18 17:38:08.151658 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.4-py3.10.egg-info/SOURCES.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)        1 2023-04-18 17:38:08.059658 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.4-py3.10.egg-info/dependency_links.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       54 2023-04-18 17:38:08.059658 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.4-py3.10.egg-info/entry_points.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       61 2023-04-18 17:38:08.059658 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.4-py3.10.egg-info/requires.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       14 2023-04-18 17:38:08.059658 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.4-py3.10.egg-info/top_level.txt
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.475659 ./usr/local/lib/python3.10/dist-packages/utils/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.516220 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6722 2023-04-18 17:40:34.840217 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/PKG-INFO
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8448 2023-04-18 17:40:34.932218 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/SOURCES.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)        1 2023-04-18 17:40:34.840217 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/dependency_links.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       54 2023-04-18 17:40:34.840217 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/entry_points.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       61 2023-04-18 17:40:34.840217 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/requires.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       14 2023-04-18 17:40:34.840217 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/top_level.txt
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/utils/
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/utils/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:38:08.475659 ./usr/local/lib/python3.10/dist-packages/utils/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      150 2023-04-18 17:38:08.475659 ./usr/local/lib/python3.10/dist-packages/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2726 2023-04-18 17:38:08.475659 ./usr/local/lib/python3.10/dist-packages/utils/__pycache__/create_proto.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2116 2023-04-18 17:38:08.475659 ./usr/local/lib/python3.10/dist-packages/utils/__pycache__/import_fixer.cpython-310.pyc
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/utils/__pycache__/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      150 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/utils/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2726 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/utils/__pycache__/create_proto.cpython-310.pyc
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2116 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/utils/__pycache__/import_fixer.cpython-310.pyc
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2544 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/utils/create_proto.py
 -rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2610 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/utils/import_fixer.py
```

### ./usr/local/bin/carball

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python
-# EASY-INSTALL-ENTRY-SCRIPT: 'sprocket-carball==0.8.4','console_scripts','carball'
+# EASY-INSTALL-ENTRY-SCRIPT: 'sprocket-carball==0.8.5','console_scripts','carball'
 import re
 import sys
 
 # for compatibility with easy_install; see #2198
-__requires__ = 'sprocket-carball==0.8.4'
+__requires__ = 'sprocket-carball==0.8.5'
 
 try:
     from importlib.metadata import distribution
 except ImportError:
     try:
         from importlib_metadata import distribution
     except ImportError:
@@ -26,8 +26,8 @@
 
 
 globals().setdefault('load_entry_point', importlib_load_entry_point)
 
 
 if __name__ == '__main__':
     sys.argv[0] = re.sub(r'(-script\.pyw?|\.exe)?$', '', sys.argv[0])
-    sys.exit(load_entry_point('sprocket-carball==0.8.4', 'console_scripts', 'carball')())
+    sys.exit(load_entry_point('sprocket-carball==0.8.5', 'console_scripts', 'carball')())
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:38:08 2023 UTC, .py size: 0 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 80d5 3e64 0000 0000  o.........>d....
+00000000: 6f0d 0d0a 0000 0000 13d6 3e64 0000 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0400 0000 6400  .....@...s....d.
 00000030: 5300 2901 4ea9 0072 0100 0000 7201 0000  S.).N..r....r...
 00000040: 0072 0100 0000 fa45 2f75 7372 2f6c 6f63  .r.....E/usr/loc
 00000050: 616c 2f6c 6962 2f70 7974 686f 6e33 2e31  al/lib/python3.1
 00000060: 302f 6469 7374 2d70 6163 6b61 6765 732f  0/dist-packages/
 00000070: 6361 7262 616c 6c2f 6765 6e65 7261 7465  carball/generate
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:38:08 2023 UTC, .py size: 0 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 80d5 3e64 0000 0000  o.........>d....
+00000000: 6f0d 0d0a 0000 0000 13d6 3e64 0000 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0400 0000 6400  .....@...s....d.
 00000030: 5300 2901 4ea9 0072 0100 0000 7201 0000  S.).N..r....r...
 00000040: 0072 0100 0000 fa49 2f75 7372 2f6c 6f63  .r.....I/usr/loc
 00000050: 616c 2f6c 6962 2f70 7974 686f 6e33 2e31  al/lib/python3.1
 00000060: 302f 6469 7374 2d70 6163 6b61 6765 732f  0/dist-packages/
 00000070: 6361 7262 616c 6c2f 6765 6e65 7261 7465  carball/generate
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/game_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 5076 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 d413 0000  o.......H.>d....
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 d413 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 001d 0000 0040 0000 0073 a402 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/party_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 2397 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 5d09 0000  o.......H.>d]...
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 5d09 0000  o.........>d]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0018 0000 0040 0000 0073 5c01 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/player_id_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 1793 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 0107 0000  o.......H.>d....
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 0107 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0017 0000 0040 0000 0073 1201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/player_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 8237 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 2d20 0000  o.......H.>d- ..
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 2d20 0000  o.........>d- ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0026 0000 0040 0000 0073 d403 0000 6400  .&...@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/team_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 3568 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 f00d 0000  o.......H.>d....
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 f00d 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 001b 0000 0040 0000 0073 e801 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:38:08 2023 UTC, .py size: 0 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 80d5 3e64 0000 0000  o.........>d....
+00000000: 6f0d 0d0a 0000 0000 13d6 3e64 0000 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0400 0000 6400  .....@...s....d.
 00000030: 5300 2901 4ea9 0072 0100 0000 7201 0000  S.).N..r....r...
 00000040: 0072 0100 0000 fa52 2f75 7372 2f6c 6f63  .r.....R/usr/loc
 00000050: 616c 2f6c 6962 2f70 7974 686f 6e33 2e31  al/lib/python3.1
 00000060: 302f 6469 7374 2d70 6163 6b61 6765 732f  0/dist-packages/
 00000070: 6361 7262 616c 6c2f 6765 6e65 7261 7465  carball/generate
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/camera_settings_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 4653 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 2d12 0000  o.......H.>d-...
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 2d12 0000  o.........>d-...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 001e 0000 0040 0000 0073 1202 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/game_metadata_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 19305 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 694b 0000  o.......H.>diK..
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 694b 0000  o.........>diK..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0028 0000 0040 0000 0073 d408 0000 6400  .(...@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a04 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c05 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c05 6d08 5a09 0100 6400 6409 6c05 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/mutators_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 3635 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 330e 0000  o.......H.>d3...
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 330e 0000  o.........>d3...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0018 0000 0040 0000 0073 ee01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a04 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c05 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c05 6d08 5a09 0100 6400 6409 6c05 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/player_loadout_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 12482 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 c230 0000  o.......H.>d.0..
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 c230 0000  o.........>d.0..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0032 0000 0040 0000 0073 0a05 0000 6400  .2...@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:38:08 2023 UTC, .py size: 0 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 80d5 3e64 0000 0000  o.........>d....
+00000000: 6f0d 0d0a 0000 0000 13d6 3e64 0000 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0400 0000 6400  .....@...s....d.
 00000030: 5300 2901 4ea9 0072 0100 0000 7201 0000  S.).N..r....r...
 00000040: 0072 0100 0000 fa4f 2f75 7372 2f6c 6f63  .r.....O/usr/loc
 00000050: 616c 2f6c 6962 2f70 7974 686f 6e33 2e31  al/lib/python3.1
 00000060: 302f 6469 7374 2d70 6163 6b61 6765 732f  0/dist-packages/
 00000070: 6361 7262 616c 6c2f 6765 6e65 7261 7465  carball/generate
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/ball_stats_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 3714 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 820e 0000  o.......H.>d....
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 820e 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 001a 0000 0040 0000 0073 d401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/data_frame_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 1383 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 6705 0000  o.......H.>dg...
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 6705 0000  o.........>dg...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0011 0000 0040 0000 0073 e400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/dropshot_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 18134 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 d646 0000  o.......H.>d.F..
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 d646 0000  o.........>d.F..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 001a 0000 0040 0000 0073 a407 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a04 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c05 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c05 6d08 5a09 0100 6400 6409 6c05 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/events_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 31534 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 2e7b 0000  o.......H.>d.{..
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 2e7b 0000  o.........>d.{..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 002f 0000 0040 0000 0073 580d 0000 6400  ./...@...sX...d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/extra_mode_stats_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 5766 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 8616 0000  o.......H.>d....
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 8616 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 001c 0000 0040 0000 0073 8e02 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/game_stats_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 6701 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 2d1a 0000  o.......H.>d-...
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 2d1a 0000  o.........>d-...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0020 0000 0040 0000 0073 1e03 0000 6400  . ...@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/goal_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 1837 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 2d07 0000  o.......H.>d-...
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 2d07 0000  o.........>d-...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0017 0000 0040 0000 0073 0801 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/kickoff_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 18809 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 7949 0000  o.......H.>dyI..
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 7949 0000  o.........>dyI..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0020 0000 0040 0000 0073 7408 0000 6400  . ...@...st...d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a04 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c05 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c05 6d08 5a09 0100 6400 6409 6c05 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/per_possession_stats_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 7823 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 8f1e 0000  o.......H.>d....
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 8f1e 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0020 0000 0040 0000 0073 5803 0000 6400  . ...@...sX...d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/player_stats_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 34767 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 cf87 0000  o.......H.>d....
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 cf87 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0026 0000 0040 0000 0073 ee0d 0000 6400  .&...@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/rumble_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 7450 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 1a1d 0000  o.......H.>d....
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 1a1d 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 001a 0000 0040 0000 0073 ae03 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a04 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c05 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c05 6d08 5a09 0100 6400 6409 6c05 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/stats_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 21715 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 d354 0000  o.......H.>d.T..
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 d354 0000  o.........>d.T..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0023 0000 0040 0000 0073 a608 0000 6400  .#...@...s....d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/team_stats_pb2.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:32:56 2023 UTC, .py size: 7909 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 48d4 3e64 e51e 0000  o.......H.>d....
+00000000: 6f0d 0d0a 0000 0000 07d6 3e64 e51e 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 001c 0000 0040 0000 0073 7c03 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 5a00 6500 6a01 6400 1900 6402  d.l.Z.e.j.d...d.
 00000040: 6b00 720f 6403 6404 8400 7012 6405 6404  k.r.d.d...p.d.d.
 00000050: 8400 5a02 6400 6406 6c03 6d04 5a05 0100  ..Z.d.d.l.m.Z...
 00000060: 6400 6407 6c03 6d06 5a07 0100 6400 6408  d.d.l.m.Z...d.d.
 00000070: 6c03 6d08 5a09 0100 6400 6409 6c03 6d0a  l.m.Z...d.d.l.m.
```

### ./usr/local/lib/python3.10/dist-packages/carball/generated/binaries/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 17:38:08 2023 UTC, .py size: 0 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 80d5 3e64 0000 0000  o.........>d....
+00000000: 6f0d 0d0a 0000 0000 13d6 3e64 0000 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0400 0000 6400  .....@...s....d.
 00000030: 5300 2901 4ea9 0072 0100 0000 7201 0000  S.).N..r....r...
 00000040: 0072 0100 0000 fa4e 2f75 7372 2f6c 6f63  .r.....N/usr/loc
 00000050: 616c 2f6c 6962 2f70 7974 686f 6e33 2e31  al/lib/python3.1
 00000060: 302f 6469 7374 2d70 6163 6b61 6765 732f  0/dist-packages/
 00000070: 6361 7262 616c 6c2f 6765 6e65 7261 7465  carball/generate
```

### Comparing `./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.4-py3.10.egg-info/PKG-INFO` & `./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocket-carball
-Version: 0.8.4
+Version: 0.8.5
 Summary: Rocket League replay parsing and analysis.
 Home-page: https://github.com/SprocketBot/carball
 Author: Sprocket Dev Team
 Author-email: asaxplayinghorse@gmail.com
 License: Apache 2.0
 Keywords: rocket-league
 Description-Content-Type: text/markdown
```

### Comparing `./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.4-py3.10.egg-info/SOURCES.txt` & `./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/SOURCES.txt`

 * *Files identical despite different names*

