# Comparing `tmp/sprocket_carball-0.8.5.linux-x86_64.tar.gz` & `tmp/sprocket_carball-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocket_carball-0.8.5.linux-x86_64.tar", last modified: Tue Apr 18 17:40:35 2023, max compression
+gzip compressed data, was "sprocket_carball-0.8.6.tar", last modified: Tue Apr 18 17:41:54 2023, max compression
```

## Comparing `sprocket_carball-0.8.5.linux-x86_64.tar` & `sprocket_carball-0.8.6.tar`

### file list

```diff
@@ -1,495 +1,257 @@
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.176219 ./
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.176219 ./usr/
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.552220 ./usr/local/
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.552220 ./usr/local/bin/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      984 2023-04-18 17:40:35.552220 ./usr/local/bin/carball
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.176219 ./usr/local/lib/
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.176219 ./usr/local/lib/python3.10/
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.512220 ./usr/local/lib/python3.10/dist-packages/
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      223 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.500220 ./usr/local/lib/python3.10/dist-packages/carball/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      403 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2197 2023-04-18 17:40:35.464220 ./usr/local/lib/python3.10/dist-packages/carball/__pycache__/command_line.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2563 2023-04-18 17:40:35.500220 ./usr/local/lib/python3.10/dist-packages/carball/__pycache__/decompile_replays.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        2 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/PROTOBUF_VERSION
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.432220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      161 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    15971 2023-04-18 17:40:35.432220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/__pycache__/analysis_manager.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    17254 2023-04-16 06:18:49.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/analysis_manager.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      169 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1555 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/__pycache__/cleaner.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2221 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/__pycache__/frame_cleaner.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1383 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/cleaner.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2295 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/frame_cleaner.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      171 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1044 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/basic_math.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3288 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/dropshot.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5196 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/field_constants.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1276 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/__pycache__/playlist.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      815 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/basic_math.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5721 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/dropshot.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6198 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/field_constants.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1187 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/playlist.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.400220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.424220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      168 2023-04-18 17:40:35.400220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8945 2023-04-18 17:40:35.424220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/__pycache__/carry_detection.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5292 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/__pycache__/event_creator.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.420220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.420220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      188 2023-04-18 17:40:35.420220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2521 2023-04-18 17:40:35.420220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/__pycache__/pickup_analysis.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3707 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/pickup_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      183 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1999 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/__pycache__/bump_analysis.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1277 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/bump_analysis.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    15129 2023-04-18 17:32:26.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/carry_detection.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.420220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      177 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1434 2023-04-18 17:40:35.420220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/__pycache__/ball.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1016 2023-04-18 17:40:35.416220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/__pycache__/damage.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1386 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/ball.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      935 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/damage.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5568 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/event_creator.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      180 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4274 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/__pycache__/fifty_analysis.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7419 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/fifty_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.400220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.404219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      182 2023-04-18 17:40:35.404219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8113 2023-04-18 17:40:35.404219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/__pycache__/base_hit.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6535 2023-04-18 17:40:35.400220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/__pycache__/hit_analysis.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11653 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/base_hit.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11223 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hit_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.404219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    41555 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/Vehicle Specifications v1.39 - Hitboxes, Handling.xlsx
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      189 2023-04-18 17:40:35.404219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2218 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/__pycache__/car.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1733 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/__pycache__/hitbox.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1662 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/car.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1973 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/hitbox.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.412220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      181 2023-04-18 17:40:35.408220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3316 2023-04-18 17:40:35.412220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/__pycache__/pressure_analysis.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3373 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/pressure_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.412220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.412220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      186 2023-04-18 17:40:35.412220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6871 2023-04-18 17:40:35.412220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/__pycache__/kickoff_analysis.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10002 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/kickoff_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      173 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3073 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/__pycache__/saltie_game.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      459 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiDemo.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2531 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiGame.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      383 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiGoal.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      479 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiMutators.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1473 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiPlayer.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1406 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiPlayerCameraSettings.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3124 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiPlayerLoadout.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      681 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiTeam.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      820 2023-04-18 17:40:35.360219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiDemo.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2370 2023-04-18 17:40:35.360219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiGame.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      765 2023-04-18 17:40:35.360219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiGoal.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      840 2023-04-18 17:40:35.360219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiMutators.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1210 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiPlayer.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      991 2023-04-18 17:40:35.360219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiPlayerCameraSettings.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1816 2023-04-18 17:40:35.360219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiPlayerLoadout.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      977 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/ApiTeam.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      182 2023-04-18 17:40:35.356219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/__pycache__/__init__.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4703 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/saltie_game.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.424220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.428220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      171 2023-04-18 17:40:35.424220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6240 2023-04-18 17:40:35.424220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__pycache__/ball_simulator.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      830 2023-04-18 17:40:35.428220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__pycache__/bounce.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      409 2023-04-18 17:40:35.428220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/__pycache__/map_constants.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11609 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/ball_simulator.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      855 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/bounce.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      238 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/map_constants.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.384220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      167 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4771 2023-04-18 17:40:35.384220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__pycache__/stats.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3469 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__pycache__/stats_list.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3938 2023-04-18 17:40:35.372219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/__pycache__/stats_manager.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      180 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1476 2023-04-18 17:40:35.364220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/__pycache__/distance_hit_ball_forward.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1023 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/distance_hit_ball_forward.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.396220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      173 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5035 2023-04-18 17:40:35.396220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/__pycache__/boost.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6918 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/boost.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      176 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2607 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/__pycache__/controls.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2829 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/controls.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.380220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.384220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      173 2023-04-18 17:40:35.380220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1646 2023-04-18 17:40:35.380220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/__pycache__/demos.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1623 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/demos.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      176 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2416 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/__pycache__/ball_carry.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3342 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/ball_carry.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.372219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      343 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.376219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      562 2023-04-18 17:40:35.372219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2194 2023-04-18 17:40:35.376219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__pycache__/ball_phase_times.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3268 2023-04-18 17:40:35.372219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__pycache__/damage.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3043 2023-04-18 17:40:35.372219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/__pycache__/goals.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2082 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/ball_phase_times.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3902 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/damage.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2575 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/goals.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      176 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2132 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/__pycache__/kickoff_stat.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2211 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/kickoff_stat.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.376219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.380220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      178 2023-04-18 17:40:35.376219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3319 2023-04-18 17:40:35.376219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/ball_distances.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7520 2023-04-18 17:40:35.380220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/per_possession.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2528 2023-04-18 17:40:35.380220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/possession.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2156 2023-04-18 17:40:35.376219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/__pycache__/turnovers.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3521 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/ball_distances.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10214 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/per_possession.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2982 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/possession.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2243 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/turnovers.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.396220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.400220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      174 2023-04-18 17:40:35.396220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3323 2023-04-18 17:40:35.400220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/__pycache__/goals.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7112 2023-04-18 17:40:35.396220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/__pycache__/rumble.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3475 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/goals.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     8977 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/rumble.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4033 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/stats.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3336 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/stats_list.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3851 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/stats_manager.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.384220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      178 2023-04-18 17:40:35.384220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1851 2023-04-18 17:40:35.388219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/averages.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2010 2023-04-18 17:40:35.384220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/hit_counts.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6267 2023-04-18 17:40:35.384220 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/positional_tendencies.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2519 2023-04-18 17:40:35.392219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/relative_position_tendencies.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2084 2023-04-18 17:40:35.388219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/speed_tendencies.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5290 2023-04-18 17:40:35.388219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/__pycache__/team_tendencies.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1330 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/averages.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1583 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/hit_counts.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6969 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/positional_tendencies.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2777 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/relative_position_tendencies.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1962 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/speed_tendencies.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6502 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/team_tendencies.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      173 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1876 2023-04-18 17:40:35.368219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/__pycache__/pandas_utils.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1708 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/pandas_utils.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      167 2023-04-18 17:40:35.348219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      632 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/json_encoder.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2173 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/numpy_manager.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2371 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/pandas_manager.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      858 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/proto_manager.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1398 2023-04-18 17:40:35.352219 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/__pycache__/split_location.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      316 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/json_encoder.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1974 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/numpy_manager.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2050 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/pandas_manager.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      374 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/proto_manager.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1265 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/split_location.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2558 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/command_line.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.432220 ./usr/local/lib/python3.10/dist-packages/carball/controls/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/controls/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.432220 ./usr/local/lib/python3.10/dist-packages/carball/controls/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      161 2023-04-18 17:40:35.432220 ./usr/local/lib/python3.10/dist-packages/carball/controls/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1762 2023-04-18 17:40:35.432220 ./usr/local/lib/python3.10/dist-packages/carball/controls/__pycache__/controls.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2743 2023-04-18 17:40:35.432220 ./usr/local/lib/python3.10/dist-packages/carball/controls/__pycache__/rotations.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2203 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/controls/controls.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3427 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/controls/rotations.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2586 2023-04-16 23:12:44.000000 ./usr/local/lib/python3.10/dist-packages/carball/decompile_replays.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/extras/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/extras/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/extras/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      159 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/extras/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1846 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/extras/__pycache__/per_goal_analysis.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1770 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/extras/per_goal_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.340219 ./usr/local/lib/python3.10/dist-packages/carball/generated/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/generated/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      162 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/generated/__pycache__/__init__.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.340219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      166 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3007 2023-04-18 17:40:35.340219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/game_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1928 2023-04-18 17:40:35.340219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/party_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1678 2023-04-18 17:40:35.340219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/player_id_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3902 2023-04-18 17:40:35.304219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/player_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2350 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/__pycache__/team_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5076 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/game_pb2.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.304219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.312219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      175 2023-04-18 17:40:35.308219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2686 2023-04-18 17:40:35.308219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/camera_settings_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8224 2023-04-18 17:40:35.312219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/game_metadata_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2670 2023-04-18 17:40:35.312219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/mutators_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5371 2023-04-18 17:40:35.304219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/__pycache__/player_loadout_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4653 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/camera_settings_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    19305 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/game_metadata_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3635 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/mutators_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    12482 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/player_loadout_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2397 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/party_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1793 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/player_id_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8237 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/player_pb2.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.312219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.340219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      172 2023-04-18 17:40:35.312219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2538 2023-04-18 17:40:35.320219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/ball_stats_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1428 2023-04-18 17:40:35.328219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/data_frame_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7293 2023-04-18 17:40:35.328219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/dropshot_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    11109 2023-04-18 17:40:35.320219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/events_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3266 2023-04-18 17:40:35.332219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/extra_mode_stats_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3649 2023-04-18 17:40:35.320219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/game_stats_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1708 2023-04-18 17:40:35.340219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/goal_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7994 2023-04-18 17:40:35.336219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/kickoff_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3677 2023-04-18 17:40:35.312219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/per_possession_stats_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    13364 2023-04-18 17:40:35.336219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/player_stats_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4030 2023-04-18 17:40:35.328219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/rumble_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8655 2023-04-18 17:40:35.324219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/stats_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4123 2023-04-18 17:40:35.324219 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/__pycache__/team_stats_pb2.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3714 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/ball_stats_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1383 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/data_frame_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    18134 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/dropshot_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    31534 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/events_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5766 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/extra_mode_stats_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6701 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/game_stats_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1837 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/goal_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    18809 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/kickoff_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7823 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/per_possession_stats_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    34767 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/player_stats_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7450 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/rumble_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    21715 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/stats_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     7909 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/team_stats_pb2.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3568 2023-04-18 17:40:23.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/api/team_pb2.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/generated/binaries/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 ./usr/local/lib/python3.10/dist-packages/carball/generated/binaries/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/generated/binaries/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      171 2023-04-18 17:40:35.344219 ./usr/local/lib/python3.10/dist-packages/carball/generated/binaries/__pycache__/__init__.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.436220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.464220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      164 2023-04-18 17:40:35.436220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2934 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/actor_parsing.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1372 2023-04-18 17:40:35.436220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/bots.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2895 2023-04-18 17:40:35.436220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/dropshot.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    10052 2023-04-18 17:40:35.444220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/frame_parser.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8300 2023-04-18 17:40:35.440220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/game.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1553 2023-04-18 17:40:35.440220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/game_info.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1285 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/goal.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8156 2023-04-18 17:40:35.436220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/player.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1495 2023-04-18 17:40:35.464220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/__pycache__/team.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.444220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      435 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      742 2023-04-18 17:40:35.444220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1718 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/ball.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1788 2023-04-18 17:40:35.452220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/base.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2849 2023-04-18 17:40:35.452220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/boost.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1024 2023-04-18 17:40:35.452220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/camera.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2166 2023-04-18 17:40:35.448220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/car.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1774 2023-04-18 17:40:35.444220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/dropshot.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1315 2023-04-18 17:40:35.452220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/game_event.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      877 2023-04-18 17:40:35.448220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/game_info.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2110 2023-04-18 17:40:35.448220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/jump.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2345 2023-04-18 17:40:35.448220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/player.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1331 2023-04-18 17:40:35.444220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/rumble.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      929 2023-04-18 17:40:35.452220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/__pycache__/team.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1649 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/ball.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1210 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/base.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4316 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/boost.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1053 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/camera.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3497 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/car.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1719 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/dropshot.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1034 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/game_event.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      388 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/game_info.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1386 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/jump.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4207 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/player.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1122 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/rumble.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      466 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/team.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3761 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor_parsing.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1374 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/bots.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2021 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/dropshot.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12747 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/frame_parser.py
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    13147 2023-04-16 06:04:04.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/game.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1614 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/game_info.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      932 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/goal.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11640 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/player.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      177 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1787 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/__pycache__/sanity_check.cpython-310.pyc
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      189 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1985 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__pycache__/base_check.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      449 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__pycache__/game_check.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      787 2023-04-18 17:40:35.456220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/__pycache__/player_check.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1261 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/base_check.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      117 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/game_check.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      298 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/player_check.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.464220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      184 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1096 2023-04-18 17:40:35.464220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__pycache__/ball_data_frame_check.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1731 2023-04-18 17:40:35.464220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__pycache__/player_attributes_check.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1317 2023-04-18 17:40:35.464220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/__pycache__/player_data_frame_check.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      496 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/ball_data_frame_check.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1037 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/player_attributes_check.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      813 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/player_data_frame_check.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      184 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      800 2023-04-18 17:40:35.460220 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/__pycache__/errors.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      275 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/errors/errors.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1459 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/sanity_check.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1195 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/json_parser/team.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/tests/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.500220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      158 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2990 2023-04-18 17:40:35.476220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/analysis_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      358 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/conftest.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     3174 2023-04-18 17:40:35.472220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/export_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2688 2023-04-18 17:40:35.496220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/game_creation_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1359 2023-04-18 17:40:35.496220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/read_pandas_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      955 2023-04-18 17:40:35.500220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/tiles_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     9954 2023-04-18 17:40:35.472220 ./usr/local/lib/python3.10/dist-packages/carball/tests/__pycache__/utils.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3666 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/analysis_test.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      171 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1219 2023-04-18 17:40:35.468220 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/__pycache__/benchmarking.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1577 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/benchmarking.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      124 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/conftest.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      163 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1615 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/__pycache__/data_frame_docs.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1610 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/docs/data_frame_docs.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2641 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/export_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2791 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/game_creation_test.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.472220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.476220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      167 2023-04-18 17:40:35.472220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1351 2023-04-18 17:40:35.476220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/camera_settings_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1429 2023-04-18 17:40:35.476220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/command_line_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1114 2023-04-18 17:40:35.472220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/error_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2210 2023-04-18 17:40:35.476220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/leader_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1010 2023-04-18 17:40:35.476220 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/__pycache__/offline_test.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1100 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/camera_settings_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      796 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/command_line_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      668 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/error_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2809 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/leader_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      635 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/offline_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      819 2023-04-15 17:31:55.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/read_pandas_test.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.496220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      164 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5765 2023-04-18 17:40:35.484220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/boost_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      988 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/demo_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)    13203 2023-04-18 17:40:35.492220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/dribble_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4887 2023-04-18 17:40:35.488220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/dropshot_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2740 2023-04-18 17:40:35.480220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/fifty_fifty_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     5615 2023-04-18 17:40:35.484220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/hit_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     4318 2023-04-18 17:40:35.488220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/kickoff_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6014 2023-04-18 17:40:35.496220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/rumble_test.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     1165 2023-04-18 17:40:35.492220 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/__pycache__/team_test.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6280 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/boost_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      494 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/demo_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    16228 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/dribble_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     8308 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/dropshot_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2911 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/fifty_fifty_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6753 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/hit_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5648 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/kickoff_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10956 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/rumble_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      814 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/stats/team_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      574 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/tiles_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12330 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/carball/tests/utils.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.516220 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6722 2023-04-18 17:40:34.840217 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/PKG-INFO
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8448 2023-04-18 17:40:34.932218 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/SOURCES.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)        1 2023-04-18 17:40:34.840217 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/dependency_links.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       54 2023-04-18 17:40:34.840217 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/entry_points.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       61 2023-04-18 17:40:34.840217 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/requires.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       14 2023-04-18 17:40:34.840217 ./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/top_level.txt
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/utils/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/utils/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/utils/__pycache__/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)      150 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2726 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/utils/__pycache__/create_proto.cpython-310.pyc
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     2116 2023-04-18 17:40:35.300219 ./usr/local/lib/python3.10/dist-packages/utils/__pycache__/import_fixer.cpython-310.pyc
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2544 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/utils/create_proto.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2610 2023-04-15 17:31:56.000000 ./usr/local/lib/python3.10/dist-packages/utils/import_fixer.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.224520 sprocket_carball-0.8.6/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11357 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/LICENSE
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      198 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/MANIFEST.in
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      552 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/NOTICE
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6722 2023-04-18 17:41:54.224520 sprocket_carball-0.8.6/PKG-INFO
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6365 2023-04-18 17:27:43.000000 sprocket_carball-0.8.6/README.md
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.160520 sprocket_carball-0.8.6/carball/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      223 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.160520 sprocket_carball-0.8.6/carball/analysis/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        2 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/PROTOBUF_VERSION
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    17254 2023-04-16 06:18:49.000000 sprocket_carball-0.8.6/carball/analysis/analysis_manager.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.160520 sprocket_carball-0.8.6/carball/analysis/cleaner/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/cleaner/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1383 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/cleaner/cleaner.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2295 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/cleaner/frame_cleaner.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.164520 sprocket_carball-0.8.6/carball/analysis/constants/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/constants/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      815 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/constants/basic_math.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5721 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/constants/dropshot.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6198 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/constants/field_constants.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1187 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/constants/playlist.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.164520 sprocket_carball-0.8.6/carball/analysis/events/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.164520 sprocket_carball-0.8.6/carball/analysis/events/boost_pad_detection/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/boost_pad_detection/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3707 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/boost_pad_detection/pickup_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.164520 sprocket_carball-0.8.6/carball/analysis/events/bump_detection/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/bump_detection/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1277 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/bump_detection/bump_analysis.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    15129 2023-04-18 17:32:26.000000 sprocket_carball-0.8.6/carball/analysis/events/carry_detection.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.168520 sprocket_carball-0.8.6/carball/analysis/events/dropshot/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/dropshot/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1386 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/dropshot/ball.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      935 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/dropshot/damage.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5568 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/event_creator.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.168520 sprocket_carball-0.8.6/carball/analysis/events/fifty_fifty/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/fifty_fifty/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7419 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/fifty_fifty/fifty_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.168520 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11653 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/base_hit.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11223 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hit_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.168520 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    41555 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/Vehicle Specifications v1.39 - Hitboxes, Handling.xlsx
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1662 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/car.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1973 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/hitbox.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.172520 sprocket_carball-0.8.6/carball/analysis/events/hit_pressure/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_pressure/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3373 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_pressure/pressure_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.172520 sprocket_carball-0.8.6/carball/analysis/events/kickoff_detection/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/kickoff_detection/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10002 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/kickoff_detection/kickoff_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.172520 sprocket_carball-0.8.6/carball/analysis/saltie_game/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.176520 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      459 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiDemo.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2531 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiGame.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      383 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiGoal.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      479 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiMutators.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1473 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiPlayer.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1406 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiPlayerCameraSettings.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3124 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiPlayerLoadout.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      681 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiTeam.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4703 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/saltie_game.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.176520 sprocket_carball-0.8.6/carball/analysis/simulator/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/simulator/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11609 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/simulator/ball_simulator.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      855 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/simulator/bounce.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      238 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/simulator/map_constants.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.176520 sprocket_carball-0.8.6/carball/analysis/stats/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.176520 sprocket_carball-0.8.6/carball/analysis/stats/ball_forward/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/ball_forward/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1023 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/ball_forward/distance_hit_ball_forward.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.180520 sprocket_carball-0.8.6/carball/analysis/stats/boost/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/boost/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6918 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/boost/boost.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.180520 sprocket_carball-0.8.6/carball/analysis/stats/controls/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/controls/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2829 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/controls/controls.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.180520 sprocket_carball-0.8.6/carball/analysis/stats/demos/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/demos/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1623 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/demos/demos.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.180520 sprocket_carball-0.8.6/carball/analysis/stats/dribbles/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/dribbles/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3342 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/dribbles/ball_carry.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.180520 sprocket_carball-0.8.6/carball/analysis/stats/dropshot/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      343 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/dropshot/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2082 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/dropshot/ball_phase_times.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3902 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/dropshot/damage.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2575 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/dropshot/goals.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.180520 sprocket_carball-0.8.6/carball/analysis/stats/kickoffs/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/kickoffs/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2211 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/kickoffs/kickoff_stat.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.184520 sprocket_carball-0.8.6/carball/analysis/stats/possession/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/possession/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3521 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/possession/ball_distances.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10214 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/possession/per_possession.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2982 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/possession/possession.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2243 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/possession/turnovers.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.184520 sprocket_carball-0.8.6/carball/analysis/stats/rumble/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/rumble/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3475 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/rumble/goals.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     8977 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/rumble/rumble.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4033 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/stats.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3336 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/stats_list.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3851 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/stats_manager.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.188520 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1330 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/averages.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1583 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/hit_counts.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6969 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/positional_tendencies.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2777 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/relative_position_tendencies.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1962 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/speed_tendencies.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6502 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/team_tendencies.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.188520 sprocket_carball-0.8.6/carball/analysis/stats/utils/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/utils/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1708 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/utils/pandas_utils.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.188520 sprocket_carball-0.8.6/carball/analysis/utils/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/utils/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      316 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/utils/json_encoder.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1974 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/utils/numpy_manager.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2050 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/utils/pandas_manager.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      374 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/utils/proto_manager.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1265 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/utils/split_location.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2558 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/command_line.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.192520 sprocket_carball-0.8.6/carball/controls/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/controls/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2203 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/controls/controls.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3427 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/controls/rotations.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2586 2023-04-16 23:12:44.000000 sprocket_carball-0.8.6/carball/decompile_replays.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.192520 sprocket_carball-0.8.6/carball/extras/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/extras/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1770 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/extras/per_goal_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.152520 sprocket_carball-0.8.6/carball/generated/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.192520 sprocket_carball-0.8.6/carball/generated/api/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/__init__.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     5076 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/game_pb2.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.196520 sprocket_carball-0.8.6/carball/generated/api/metadata/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/metadata/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4653 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/metadata/camera_settings_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)    19305 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/metadata/game_metadata_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3635 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/metadata/mutators_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12482 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/metadata/player_loadout_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     2397 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/party_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1793 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/player_id_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     8237 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/player_pb2.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.200520 sprocket_carball-0.8.6/carball/generated/api/stats/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/__init__.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     3714 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/ball_stats_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     1383 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/data_frame_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)    18134 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/dropshot_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)    31534 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/events_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     5766 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/extra_mode_stats_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     6701 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/game_stats_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1837 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/goal_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)    18809 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/kickoff_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7823 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/per_possession_stats_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)    34767 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/player_stats_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7450 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/rumble_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    21715 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/stats_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     7909 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/team_stats_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     3568 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/team_pb2.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.200520 sprocket_carball-0.8.6/carball/generated/binaries/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/binaries/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.204520 sprocket_carball-0.8.6/carball/json_parser/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.208520 sprocket_carball-0.8.6/carball/json_parser/actor/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      435 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1649 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/ball.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1210 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/base.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4316 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/boost.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1053 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/camera.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3497 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/car.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1719 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/dropshot.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1034 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/game_event.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      388 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/game_info.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1386 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/jump.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4207 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/player.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1122 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/rumble.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      466 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/team.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3761 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor_parsing.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1374 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/bots.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2021 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/dropshot.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12747 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/frame_parser.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    13147 2023-04-16 06:04:04.000000 sprocket_carball-0.8.6/carball/json_parser/game.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1614 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/game_info.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      932 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/goal.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11640 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/player.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.208520 sprocket_carball-0.8.6/carball/json_parser/sanity_check/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.208520 sprocket_carball-0.8.6/carball/json_parser/sanity_check/base_checks/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/base_checks/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1261 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/base_checks/base_check.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      117 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/base_checks/game_check.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      298 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/base_checks/player_check.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.212520 sprocket_carball-0.8.6/carball/json_parser/sanity_check/checks/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/checks/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      496 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/checks/ball_data_frame_check.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1037 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/checks/player_attributes_check.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      813 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/checks/player_data_frame_check.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.212520 sprocket_carball-0.8.6/carball/json_parser/sanity_check/errors/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/errors/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      275 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/errors/errors.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1459 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/sanity_check.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1195 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/team.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.212520 sprocket_carball-0.8.6/carball/tests/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3666 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/analysis_test.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.212520 sprocket_carball-0.8.6/carball/tests/benchmarking/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/benchmarking/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1577 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/benchmarking/benchmarking.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      124 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/conftest.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.216520 sprocket_carball-0.8.6/carball/tests/docs/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/docs/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1610 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/docs/data_frame_docs.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2641 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/export_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2791 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/game_creation_test.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.216520 sprocket_carball-0.8.6/carball/tests/metadata/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/metadata/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1100 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/metadata/camera_settings_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      796 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/metadata/command_line_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      668 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/metadata/error_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2809 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/metadata/leader_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      635 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/metadata/offline_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      819 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/read_pandas_test.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.220520 sprocket_carball-0.8.6/carball/tests/stats/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6280 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/boost_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      494 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/demo_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    16228 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/dribble_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     8308 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/dropshot_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2911 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/fifty_fifty_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6753 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/hit_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5648 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/kickoff_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10956 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/rumble_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      814 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/team_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      574 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/tiles_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12330 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/utils.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      375 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/init.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)       62 2023-04-16 23:09:05.000000 sprocket_carball-0.8.6/requirements.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       38 2023-04-18 17:41:54.224520 sprocket_carball-0.8.6/setup.cfg
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1676 2023-04-18 17:41:43.000000 sprocket_carball-0.8.6/setup.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.220520 sprocket_carball-0.8.6/sprocket_carball.egg-info/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6722 2023-04-18 17:41:53.000000 sprocket_carball-0.8.6/sprocket_carball.egg-info/PKG-INFO
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8448 2023-04-18 17:41:54.000000 sprocket_carball-0.8.6/sprocket_carball.egg-info/SOURCES.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)        1 2023-04-18 17:41:53.000000 sprocket_carball-0.8.6/sprocket_carball.egg-info/dependency_links.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       54 2023-04-18 17:41:53.000000 sprocket_carball-0.8.6/sprocket_carball.egg-info/entry_points.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       61 2023-04-18 17:41:53.000000 sprocket_carball-0.8.6/sprocket_carball.egg-info/requires.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       14 2023-04-18 17:41:53.000000 sprocket_carball-0.8.6/sprocket_carball.egg-info/top_level.txt
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.224520 sprocket_carball-0.8.6/utils/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/utils/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2544 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/utils/create_proto.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2610 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/utils/import_fixer.py
```

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/analysis_manager.py` & `sprocket_carball-0.8.6/carball/analysis/analysis_manager.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/cleaner.py` & `sprocket_carball-0.8.6/carball/analysis/cleaner/cleaner.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/cleaner/frame_cleaner.py` & `sprocket_carball-0.8.6/carball/analysis/cleaner/frame_cleaner.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/basic_math.py` & `sprocket_carball-0.8.6/carball/analysis/constants/basic_math.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/dropshot.py` & `sprocket_carball-0.8.6/carball/analysis/constants/dropshot.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/field_constants.py` & `sprocket_carball-0.8.6/carball/analysis/constants/field_constants.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/constants/playlist.py` & `sprocket_carball-0.8.6/carball/analysis/constants/playlist.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/events/boost_pad_detection/pickup_analysis.py` & `sprocket_carball-0.8.6/carball/analysis/events/boost_pad_detection/pickup_analysis.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/events/bump_detection/bump_analysis.py` & `sprocket_carball-0.8.6/carball/analysis/events/bump_detection/bump_analysis.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/events/carry_detection.py` & `sprocket_carball-0.8.6/carball/analysis/events/carry_detection.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/ball.py` & `sprocket_carball-0.8.6/carball/analysis/events/dropshot/ball.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/events/dropshot/damage.py` & `sprocket_carball-0.8.6/carball/analysis/events/dropshot/damage.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/events/event_creator.py` & `sprocket_carball-0.8.6/carball/analysis/events/event_creator.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/events/fifty_fifty/fifty_analysis.py` & `sprocket_carball-0.8.6/carball/analysis/events/fifty_fifty/fifty_analysis.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/base_hit.py` & `sprocket_carball-0.8.6/carball/analysis/events/hit_detection/base_hit.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hit_analysis.py` & `sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hit_analysis.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/Vehicle Specifications v1.39 - Hitboxes, Handling.xlsx` & `sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/Vehicle Specifications v1.39 - Hitboxes, Handling.xlsx`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/car.py` & `sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/car.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_detection/hitbox/hitbox.py` & `sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/hitbox.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/events/hit_pressure/pressure_analysis.py` & `sprocket_carball-0.8.6/carball/analysis/events/hit_pressure/pressure_analysis.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/events/kickoff_detection/kickoff_analysis.py` & `sprocket_carball-0.8.6/carball/analysis/events/kickoff_detection/kickoff_analysis.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiGame.py` & `sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiGame.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiPlayer.py` & `sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiPlayer.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiPlayerCameraSettings.py` & `sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiPlayerCameraSettings.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiPlayerLoadout.py` & `sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiPlayerLoadout.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/metadata/ApiTeam.py` & `sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiTeam.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/saltie_game/saltie_game.py` & `sprocket_carball-0.8.6/carball/analysis/saltie_game/saltie_game.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/ball_simulator.py` & `sprocket_carball-0.8.6/carball/analysis/simulator/ball_simulator.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/simulator/bounce.py` & `sprocket_carball-0.8.6/carball/analysis/simulator/bounce.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/ball_forward/distance_hit_ball_forward.py` & `sprocket_carball-0.8.6/carball/analysis/stats/ball_forward/distance_hit_ball_forward.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/boost/boost.py` & `sprocket_carball-0.8.6/carball/analysis/stats/boost/boost.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/controls/controls.py` & `sprocket_carball-0.8.6/carball/analysis/stats/controls/controls.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/demos/demos.py` & `sprocket_carball-0.8.6/carball/analysis/stats/demos/demos.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dribbles/ball_carry.py` & `sprocket_carball-0.8.6/carball/analysis/stats/dribbles/ball_carry.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/ball_phase_times.py` & `sprocket_carball-0.8.6/carball/analysis/stats/dropshot/ball_phase_times.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/damage.py` & `sprocket_carball-0.8.6/carball/analysis/stats/dropshot/damage.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/dropshot/goals.py` & `sprocket_carball-0.8.6/carball/analysis/stats/dropshot/goals.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/kickoffs/kickoff_stat.py` & `sprocket_carball-0.8.6/carball/analysis/stats/kickoffs/kickoff_stat.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/ball_distances.py` & `sprocket_carball-0.8.6/carball/analysis/stats/possession/ball_distances.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/per_possession.py` & `sprocket_carball-0.8.6/carball/analysis/stats/possession/per_possession.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/possession.py` & `sprocket_carball-0.8.6/carball/analysis/stats/possession/possession.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/possession/turnovers.py` & `sprocket_carball-0.8.6/carball/analysis/stats/possession/turnovers.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/goals.py` & `sprocket_carball-0.8.6/carball/analysis/stats/rumble/goals.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/rumble/rumble.py` & `sprocket_carball-0.8.6/carball/analysis/stats/rumble/rumble.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/stats.py` & `sprocket_carball-0.8.6/carball/analysis/stats/stats.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/stats_list.py` & `sprocket_carball-0.8.6/carball/analysis/stats/stats_list.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/stats_manager.py` & `sprocket_carball-0.8.6/carball/analysis/stats/stats_manager.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/averages.py` & `sprocket_carball-0.8.6/carball/analysis/stats/tendencies/averages.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/hit_counts.py` & `sprocket_carball-0.8.6/carball/analysis/stats/tendencies/hit_counts.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/positional_tendencies.py` & `sprocket_carball-0.8.6/carball/analysis/stats/tendencies/positional_tendencies.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/relative_position_tendencies.py` & `sprocket_carball-0.8.6/carball/analysis/stats/tendencies/relative_position_tendencies.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/speed_tendencies.py` & `sprocket_carball-0.8.6/carball/analysis/stats/tendencies/speed_tendencies.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/tendencies/team_tendencies.py` & `sprocket_carball-0.8.6/carball/analysis/stats/tendencies/team_tendencies.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/stats/utils/pandas_utils.py` & `sprocket_carball-0.8.6/carball/analysis/stats/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/numpy_manager.py` & `sprocket_carball-0.8.6/carball/analysis/utils/numpy_manager.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/pandas_manager.py` & `sprocket_carball-0.8.6/carball/analysis/utils/pandas_manager.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/analysis/utils/split_location.py` & `sprocket_carball-0.8.6/carball/analysis/utils/split_location.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/command_line.py` & `sprocket_carball-0.8.6/carball/command_line.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/controls/controls.py` & `sprocket_carball-0.8.6/carball/controls/controls.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/controls/rotations.py` & `sprocket_carball-0.8.6/carball/controls/rotations.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/decompile_replays.py` & `sprocket_carball-0.8.6/carball/decompile_replays.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/extras/per_goal_analysis.py` & `sprocket_carball-0.8.6/carball/extras/per_goal_analysis.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/game_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/game_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/camera_settings_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/metadata/camera_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/game_metadata_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/metadata/game_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/mutators_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/metadata/mutators_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/metadata/player_loadout_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/metadata/player_loadout_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/party_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/party_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/player_id_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/player_id_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/player_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/player_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/ball_stats_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/stats/ball_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/data_frame_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/stats/data_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/dropshot_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/stats/dropshot_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/events_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/stats/events_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/extra_mode_stats_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/stats/extra_mode_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/game_stats_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/stats/game_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/goal_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/stats/goal_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/kickoff_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/stats/kickoff_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/per_possession_stats_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/stats/per_possession_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/player_stats_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/stats/player_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/rumble_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/stats/rumble_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/stats_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/stats/stats_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/stats/team_stats_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/stats/team_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/generated/api/team_pb2.py` & `sprocket_carball-0.8.6/carball/generated/api/team_pb2.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/ball.py` & `sprocket_carball-0.8.6/carball/json_parser/actor/ball.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/base.py` & `sprocket_carball-0.8.6/carball/json_parser/actor/base.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/boost.py` & `sprocket_carball-0.8.6/carball/json_parser/actor/boost.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/camera.py` & `sprocket_carball-0.8.6/carball/json_parser/actor/camera.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/car.py` & `sprocket_carball-0.8.6/carball/json_parser/actor/car.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/dropshot.py` & `sprocket_carball-0.8.6/carball/json_parser/actor/dropshot.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/game_event.py` & `sprocket_carball-0.8.6/carball/json_parser/actor/game_event.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/jump.py` & `sprocket_carball-0.8.6/carball/json_parser/actor/jump.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/player.py` & `sprocket_carball-0.8.6/carball/json_parser/actor/player.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor/rumble.py` & `sprocket_carball-0.8.6/carball/json_parser/actor/rumble.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/actor_parsing.py` & `sprocket_carball-0.8.6/carball/json_parser/actor_parsing.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/bots.py` & `sprocket_carball-0.8.6/carball/json_parser/bots.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/dropshot.py` & `sprocket_carball-0.8.6/carball/json_parser/dropshot.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/frame_parser.py` & `sprocket_carball-0.8.6/carball/json_parser/frame_parser.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/game.py` & `sprocket_carball-0.8.6/carball/json_parser/game.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/game_info.py` & `sprocket_carball-0.8.6/carball/json_parser/game_info.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/goal.py` & `sprocket_carball-0.8.6/carball/json_parser/goal.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/player.py` & `sprocket_carball-0.8.6/carball/json_parser/player.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/base_checks/base_check.py` & `sprocket_carball-0.8.6/carball/json_parser/sanity_check/base_checks/base_check.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/player_attributes_check.py` & `sprocket_carball-0.8.6/carball/json_parser/sanity_check/checks/player_attributes_check.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/checks/player_data_frame_check.py` & `sprocket_carball-0.8.6/carball/json_parser/sanity_check/checks/player_data_frame_check.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/sanity_check/sanity_check.py` & `sprocket_carball-0.8.6/carball/json_parser/sanity_check/sanity_check.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/json_parser/team.py` & `sprocket_carball-0.8.6/carball/json_parser/team.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/analysis_test.py` & `sprocket_carball-0.8.6/carball/tests/analysis_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/benchmarking/benchmarking.py` & `sprocket_carball-0.8.6/carball/tests/benchmarking/benchmarking.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/docs/data_frame_docs.py` & `sprocket_carball-0.8.6/carball/tests/docs/data_frame_docs.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/export_test.py` & `sprocket_carball-0.8.6/carball/tests/export_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/game_creation_test.py` & `sprocket_carball-0.8.6/carball/tests/game_creation_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/camera_settings_test.py` & `sprocket_carball-0.8.6/carball/tests/metadata/camera_settings_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/command_line_test.py` & `sprocket_carball-0.8.6/carball/tests/metadata/command_line_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/error_test.py` & `sprocket_carball-0.8.6/carball/tests/metadata/error_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/leader_test.py` & `sprocket_carball-0.8.6/carball/tests/metadata/leader_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/metadata/offline_test.py` & `sprocket_carball-0.8.6/carball/tests/metadata/offline_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/read_pandas_test.py` & `sprocket_carball-0.8.6/carball/tests/read_pandas_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/stats/boost_test.py` & `sprocket_carball-0.8.6/carball/tests/stats/boost_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/stats/dribble_test.py` & `sprocket_carball-0.8.6/carball/tests/stats/dribble_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/stats/dropshot_test.py` & `sprocket_carball-0.8.6/carball/tests/stats/dropshot_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/stats/fifty_fifty_test.py` & `sprocket_carball-0.8.6/carball/tests/stats/fifty_fifty_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/stats/hit_test.py` & `sprocket_carball-0.8.6/carball/tests/stats/hit_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/stats/kickoff_test.py` & `sprocket_carball-0.8.6/carball/tests/stats/kickoff_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/stats/rumble_test.py` & `sprocket_carball-0.8.6/carball/tests/stats/rumble_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/stats/team_test.py` & `sprocket_carball-0.8.6/carball/tests/stats/team_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/tiles_test.py` & `sprocket_carball-0.8.6/carball/tests/tiles_test.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/carball/tests/utils.py` & `sprocket_carball-0.8.6/carball/tests/utils.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/PKG-INFO` & `sprocket_carball-0.8.6/sprocket_carball.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocket-carball
-Version: 0.8.5
+Version: 0.8.6
 Summary: Rocket League replay parsing and analysis.
 Home-page: https://github.com/SprocketBot/carball
 Author: Sprocket Dev Team
 Author-email: asaxplayinghorse@gmail.com
 License: Apache 2.0
 Keywords: rocket-league
 Description-Content-Type: text/markdown
```

### Comparing `./usr/local/lib/python3.10/dist-packages/sprocket_carball-0.8.5-py3.10.egg-info/SOURCES.txt` & `sprocket_carball-0.8.6/sprocket_carball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/utils/create_proto.py` & `sprocket_carball-0.8.6/utils/create_proto.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/utils/import_fixer.py` & `sprocket_carball-0.8.6/utils/import_fixer.py`

 * *Files identical despite different names*

