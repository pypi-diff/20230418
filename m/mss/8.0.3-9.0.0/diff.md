# Comparing `tmp/mss-8.0.3.tar.gz` & `tmp/mss-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mss-8.0.3.tar", last modified: Fri Apr 14 22:53:22 2023, max compression
+gzip compressed data, was "mss-9.0.0.tar", last modified: Tue Apr 18 20:19:43 2023, max compression
```

## Comparing `mss-8.0.3.tar` & `mss-9.0.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.671195 mss-8.0.3/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    10881 2023-04-14 22:51:49.000000 mss-8.0.3/CHANGELOG.md
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5575 2023-04-14 22:52:22.000000 mss-8.0.3/CHANGES.md
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      668 2023-04-10 12:52:20.000000 mss-8.0.3/CONTRIBUTORS.md
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1093 2023-04-10 14:19:05.000000 mss-8.0.3/LICENSE.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      276 2023-04-14 22:47:09.000000 mss-8.0.3/MANIFEST.in
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3928 2023-04-14 22:53:22.671195 mss-8.0.3/PKG-INFO
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2109 2023-04-14 22:53:15.000000 mss-8.0.3/README.md
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       43 2023-04-11 07:35:16.000000 mss-8.0.3/dev-requirements.txt
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.663195 mss-8.0.3/docs/
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.667195 mss-8.0.3/docs/source/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8751 2023-04-09 20:16:52.000000 mss-8.0.3/docs/source/api.rst
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2417 2023-04-10 11:05:18.000000 mss-8.0.3/docs/source/conf.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      858 2023-04-10 20:36:40.000000 mss-8.0.3/docs/source/developers.rst
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.667195 mss-8.0.3/docs/source/examples/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      550 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/callback.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      729 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/custom_cls_image.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1356 2022-10-27 02:44:18.000000 mss-8.0.3/docs/source/examples/fps.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1113 2022-10-27 02:47:31.000000 mss-8.0.3/docs/source/examples/fps_multiprocessing.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      751 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/from_pil_tuple.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      240 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/linux_display_keyword.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      885 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/opencv_numpy.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      526 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/part_of_screen.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      792 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/part_of_screen_monitor_2.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      712 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/pil.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      755 2023-04-10 11:55:20.000000 mss-8.0.3/docs/source/examples/pil_pixels.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     4332 2022-10-27 01:33:30.000000 mss-8.0.3/docs/source/examples.rst
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1689 2023-04-10 19:48:35.000000 mss-8.0.3/docs/source/index.rst
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      494 2022-10-27 01:33:30.000000 mss-8.0.3/docs/source/installation.rst
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      735 2023-04-09 20:16:52.000000 mss-8.0.3/docs/source/support.rst
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2216 2023-04-09 20:16:52.000000 mss-8.0.3/docs/source/usage.rst
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3293 2023-04-09 22:30:36.000000 mss-8.0.3/docs/source/where.rst
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2427 2023-04-14 22:53:22.671195 mss-8.0.3/setup.cfg
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       39 2022-10-27 01:33:30.000000 mss-8.0.3/setup.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.663195 mss-8.0.3/src/
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.667195 mss-8.0.3/src/mss/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      940 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/__init__.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2659 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/__main__.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8565 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/base.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     7513 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/darwin.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      368 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/exception.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      911 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/factory.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    16933 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/linux.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      416 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/models.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/py.typed
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3859 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/screenshot.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1928 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/tools.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     9290 2023-04-14 22:47:09.000000 mss-8.0.3/src/mss/windows.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.667195 mss-8.0.3/src/mss.egg-info/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3928 2023-04-14 22:53:22.000000 mss-8.0.3/src/mss.egg-info/PKG-INFO
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1647 2023-04-14 22:53:22.000000 mss-8.0.3/src/mss.egg-info/SOURCES.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-14 22:53:22.000000 mss-8.0.3/src/mss.egg-info/dependency_links.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       42 2023-04-14 22:53:22.000000 mss-8.0.3/src/mss.egg-info/entry_points.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        4 2023-04-14 22:53:22.000000 mss-8.0.3/src/mss.egg-info/top_level.txt
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.671195 mss-8.0.3/src/tests/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1566 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/bench_bgra2rgb.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1327 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/bench_general.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1577 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/conftest.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:53:22.671195 mss-8.0.3/src/tests/res/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    37834 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/res/monitor-1024x768.raw.zip
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      501 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_bgra_to_rgb.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      573 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_cls_image.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      863 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_find_monitors.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1777 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_get_pixels.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5383 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_gnu_linux.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     6612 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_implementation.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1366 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_issue_220.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3530 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_leaks.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1719 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_macos.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2242 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_save.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     6674 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_setup.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2475 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_third_party.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1969 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_tools.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1866 2023-04-14 22:47:09.000000 mss-8.0.3/src/tests/test_windows.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       75 2023-04-11 07:36:50.000000 mss-8.0.3/tests-requirements.txt
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.514272 mss-9.0.0/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    11521 2023-04-18 20:18:15.000000 mss-9.0.0/CHANGELOG.md
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5769 2023-04-18 20:16:57.000000 mss-9.0.0/CHANGES.md
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      668 2023-04-10 12:52:20.000000 mss-9.0.0/CONTRIBUTORS.md
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1093 2023-04-10 14:19:05.000000 mss-9.0.0/LICENSE.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      276 2023-04-14 22:47:09.000000 mss-9.0.0/MANIFEST.in
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3928 2023-04-18 20:19:43.514272 mss-9.0.0/PKG-INFO
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2110 2023-04-14 22:55:26.000000 mss-9.0.0/README.md
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       43 2023-04-11 07:35:16.000000 mss-9.0.0/dev-requirements.txt
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.506272 mss-9.0.0/docs/
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.510272 mss-9.0.0/docs/source/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8757 2023-04-18 20:16:41.000000 mss-9.0.0/docs/source/api.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2417 2023-04-15 20:14:16.000000 mss-9.0.0/docs/source/conf.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      858 2023-04-10 20:36:40.000000 mss-9.0.0/docs/source/developers.rst
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.510272 mss-9.0.0/docs/source/examples/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      550 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/callback.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      729 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/custom_cls_image.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1356 2022-10-27 02:44:18.000000 mss-9.0.0/docs/source/examples/fps.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1113 2022-10-27 02:47:31.000000 mss-9.0.0/docs/source/examples/fps_multiprocessing.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      751 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/from_pil_tuple.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      240 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/linux_display_keyword.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      885 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/opencv_numpy.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      526 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/part_of_screen.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      792 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/part_of_screen_monitor_2.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      712 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/pil.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      755 2023-04-10 11:55:20.000000 mss-9.0.0/docs/source/examples/pil_pixels.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     4332 2022-10-27 01:33:30.000000 mss-9.0.0/docs/source/examples.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1689 2023-04-10 19:48:35.000000 mss-9.0.0/docs/source/index.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      494 2022-10-27 01:33:30.000000 mss-9.0.0/docs/source/installation.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      735 2023-04-09 20:16:52.000000 mss-9.0.0/docs/source/support.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2216 2023-04-09 20:16:52.000000 mss-9.0.0/docs/source/usage.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3293 2023-04-09 22:30:36.000000 mss-9.0.0/docs/source/where.rst
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2439 2023-04-18 20:19:43.514272 mss-9.0.0/setup.cfg
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       39 2022-10-27 01:33:30.000000 mss-9.0.0/setup.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.510272 mss-9.0.0/src/
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.510272 mss-9.0.0/src/mss/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      940 2023-04-18 20:16:57.000000 mss-9.0.0/src/mss/__init__.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2659 2023-04-14 22:47:09.000000 mss-9.0.0/src/mss/__main__.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8565 2023-04-15 20:54:55.000000 mss-9.0.0/src/mss/base.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     7430 2023-04-18 20:16:16.000000 mss-9.0.0/src/mss/darwin.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      368 2023-04-14 22:47:09.000000 mss-9.0.0/src/mss/exception.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      911 2023-04-14 22:47:09.000000 mss-9.0.0/src/mss/factory.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    16967 2023-04-18 20:16:30.000000 mss-9.0.0/src/mss/linux.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      416 2023-04-14 22:47:09.000000 mss-9.0.0/src/mss/models.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-14 22:47:09.000000 mss-9.0.0/src/mss/py.typed
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3859 2023-04-14 22:47:09.000000 mss-9.0.0/src/mss/screenshot.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1928 2023-04-15 20:55:26.000000 mss-9.0.0/src/mss/tools.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8818 2023-04-15 21:57:39.000000 mss-9.0.0/src/mss/windows.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.510272 mss-9.0.0/src/mss.egg-info/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3928 2023-04-18 20:19:43.000000 mss-9.0.0/src/mss.egg-info/PKG-INFO
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1647 2023-04-18 20:19:43.000000 mss-9.0.0/src/mss.egg-info/SOURCES.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-18 20:19:43.000000 mss-9.0.0/src/mss.egg-info/dependency_links.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       42 2023-04-18 20:19:43.000000 mss-9.0.0/src/mss.egg-info/entry_points.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        4 2023-04-18 20:19:43.000000 mss-9.0.0/src/mss.egg-info/top_level.txt
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.514272 mss-9.0.0/src/tests/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1566 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/bench_bgra2rgb.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1327 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/bench_general.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1629 2023-04-15 22:58:23.000000 mss-9.0.0/src/tests/conftest.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-18 20:19:43.514272 mss-9.0.0/src/tests/res/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    37834 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/res/monitor-1024x768.raw.zip
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      508 2023-04-15 22:57:30.000000 mss-9.0.0/src/tests/test_bgra_to_rgb.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      573 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_cls_image.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      863 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_find_monitors.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1517 2023-04-15 22:57:30.000000 mss-9.0.0/src/tests/test_get_pixels.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5439 2023-04-15 20:13:59.000000 mss-9.0.0/src/tests/test_gnu_linux.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     6612 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_implementation.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1366 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_issue_220.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3470 2023-04-15 20:13:59.000000 mss-9.0.0/src/tests/test_leaks.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1719 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_macos.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2242 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_save.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     6674 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_setup.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2475 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_third_party.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1969 2023-04-14 22:47:09.000000 mss-9.0.0/src/tests/test_tools.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2920 2023-04-15 21:55:33.000000 mss-9.0.0/src/tests/test_windows.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      101 2023-04-16 08:23:38.000000 mss-9.0.0/tests-requirements.txt
```

### Comparing `mss-8.0.3/CHANGELOG.md` & `mss-9.0.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # History
 
 See Git checking messages for full history.
 
+## 9.0.0 (2023/04/18)
+- Linux: add failure handling to `XOpenDisplay()` call (fixes #246)
+- Mac: tiny improvement in moniors finding
+- Windows: refactored how internal handles are stored (fixes #198)
+- Windows: removed side effects when leaving the context manager, resources are all freed (fixes #209)
+- CI: run tests via `xvfb-run` on GitHub Actions (#248)
+- tests: enhance `test_get_pixels.py`, and try to fix a random failure at the same time (related to #251)
+- tests: use `PyVirtualDisplay` instead of `xvfbwrapper` (#249)
+- tests: automatic rerun in case of failure (related to #251)
+- :heart: contributors: @mgorny, @CTPaHHuK-HEbA
+
 ## 8.0.3 (2023/04/15)
 - added support for Python 3.12
 - MSS: added PEP 561 compatibility
 - MSS: include more files in the sdist package (#240)
 - Linux: restore the original X error handler in `.close()` (#241)
 - Linux: fixed `XRRCrtcInfo.width`, and `XRRCrtcInfo.height`, C types
 - doc: use markdown for the README, and changelogs
```

### Comparing `mss-8.0.3/CHANGES.md` & `mss-9.0.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Technical Changes
 
+## 9.0.0 (2023-04-18)
+
+### linux.py
+- Removed `XEvent` class. Use `XErrorEvent` instead.
+
+### windows.py
+- Added `MSS.close()` method
+- Removed `MSS.bmp` attribute
+- Removed `MSS.memdc` attribute
+
 ## 8.0.3 (2023-04-15)
 
 ### linux.py
 - Added `XErrorEvent` class (old `Event` class is just an alias now, and will be removed in v9.0.0)
 
 ## 8.0.0 (2023-04-09)
 
@@ -13,16 +23,16 @@
 - Added `max_displays=32` keyword argument to `MSS.__init__()`
 - Added `with_cursor=False` keyword argument to `MSS.__init__()`
 - Added `MSS.with_cursor` attribute
 
 ### linux.py
 - Added `MSS.close()`
 - Moved `MSS.__init__()` keyword arguments handling to the base class
-- Renamed `error_handler()` function to `__error_handler()`
-- Renamed `_validate()` function to `___validate()`
+- Renamed `error_handler()` function to `_error_handler()`
+- Renamed `validate()` function to `__validate()`
 - Renamed `MSS.has_extension()` method to `_is_extension_enabled()`
 - Removed `ERROR` namespace
 - Removed `MSS.drawable` attribute
 - Removed `MSS.root` attribute
 - Removed `MSS.get_error_details()` method. Use `ScreenShotError.details` attribute instead.
 
 ## 6.1.0 (2020-10-31)
```

### Comparing `mss-8.0.3/CONTRIBUTORS.md` & `mss-9.0.0/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/LICENSE.txt` & `mss-9.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/PKG-INFO` & `mss-9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mss
-Version: 8.0.3
+Version: 9.0.0
 Summary: An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 Home-page: https://github.com/BoboTiG/python-mss
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: MIT
 Project-URL: Documentation, https://python-mss.readthedocs.io
 Project-URL: Source, https://github.com/BoboTiG/python-mss
```

### Comparing `mss-8.0.3/README.md` & `mss-9.0.0/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -47,8 +47,8 @@
 For the maintainers, here are commands to upload a new release:
 
 ```shell
 rm -rf build dist
 python -m build
 twine check dist/*
 twine upload dist/*
-```
+```
```

### Comparing `mss-8.0.3/docs/source/api.rst` & `mss-9.0.0/docs/source/api.rst`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 .. attribute:: ZPIXMAP
 
 .. class:: Display
 
     Structure that serves as the connection to the X server, and that contains all the information about that X server.
 
-.. class:: Event
+.. class:: XErrorEvent
 
     XErrorEvent to debug eventual errors.
 
 .. class:: XFixesCursorImage
 
     Cursor structure
```

### Comparing `mss-8.0.3/docs/source/conf.py` & `mss-9.0.0/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 author = "Tiger-222"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "8.0.3"
+version = "8.0.4"
 
 # The full version, including alpha/beta/rc tags.
 release = "latest"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
```

### Comparing `mss-8.0.3/docs/source/developers.rst` & `mss-9.0.0/docs/source/developers.rst`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/docs/source/examples/callback.py` & `mss-9.0.0/docs/source/examples/callback.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/docs/source/examples/custom_cls_image.py` & `mss-9.0.0/docs/source/examples/custom_cls_image.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/docs/source/examples/fps.py` & `mss-9.0.0/docs/source/examples/fps.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/docs/source/examples/fps_multiprocessing.py` & `mss-9.0.0/docs/source/examples/fps_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/docs/source/examples/from_pil_tuple.py` & `mss-9.0.0/docs/source/examples/from_pil_tuple.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/docs/source/examples/opencv_numpy.py` & `mss-9.0.0/docs/source/examples/opencv_numpy.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/docs/source/examples/part_of_screen.py` & `mss-9.0.0/docs/source/examples/part_of_screen.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/docs/source/examples/part_of_screen_monitor_2.py` & `mss-9.0.0/docs/source/examples/part_of_screen_monitor_2.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/docs/source/examples/pil.py` & `mss-9.0.0/docs/source/examples/pil.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/docs/source/examples/pil_pixels.py` & `mss-9.0.0/docs/source/examples/pil_pixels.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/docs/source/examples.rst` & `mss-9.0.0/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/docs/source/index.rst` & `mss-9.0.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/docs/source/support.rst` & `mss-9.0.0/docs/source/support.rst`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/docs/source/usage.rst` & `mss-9.0.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/docs/source/where.rst` & `mss-9.0.0/docs/source/where.rst`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/setup.cfg` & `mss-9.0.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mss
-version = 8.0.3
+version = 9.0.0
 author = Mickaël 'Tiger-222' Schoentgen
 author_email = contact@tiger-222.fr
 description = An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BoboTiG/python-mss
 home_page = https://pypi.org/project/mss/
@@ -88,12 +88,13 @@
 addopts = 
 	--showlocals
 	--strict-markers
 	-r fE
 	-v
 	--cov=mss
 	--cov-report=term-missing
+	--reruns 5
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mss-8.0.3/src/mss/__init__.py` & `mss-9.0.0/src/mss/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 You can always get the latest version of this module at:
     https://github.com/BoboTiG/python-mss
 If that URL should fail, try contacting the author.
 """
 from .exception import ScreenShotError
 from .factory import mss
 
-__version__ = "8.0.3"
+__version__ = "9.0.0"
 __author__ = "Mickaël 'Tiger-222' Schoentgen"
 __copyright__ = """
 Copyright (c) 2013-2023, Mickaël 'Tiger-222' Schoentgen
 
 Permission to use, copy, modify, and distribute this software and its
 documentation for any purpose and without fee or royalty is hereby
 granted, provided that the above copyright notice appear in all copies
```

### Comparing `mss-8.0.3/src/mss/__main__.py` & `mss-9.0.0/src/mss/__main__.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/mss/base.py` & `mss-9.0.0/src/mss/base.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/mss/darwin.py` & `mss-9.0.0/src/mss/darwin.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,15 +99,14 @@
     def _init_library(self) -> None:
         """Load the CoreGraphics library."""
         version = float(".".join(mac_ver()[0].split(".")[:2]))
         if version < 10.16:
             coregraphics = ctypes.util.find_library("CoreGraphics")
         else:
             # macOS Big Sur and newer
-            # pylint: disable=line-too-long
             coregraphics = "/System/Library/Frameworks/CoreGraphics.framework/Versions/Current/CoreGraphics"
 
         if not coregraphics:
             raise ScreenShotError("No CoreGraphics library found.")
         self.core = ctypes.cdll.LoadLibrary(coregraphics)
 
     def _set_cfunctions(self) -> None:
@@ -130,22 +129,21 @@
         all_monitors = CGRect()
         self._monitors.append({})
 
         # Each monitor
         display_count = c_uint32(0)
         active_displays = (c_uint32 * self.max_displays)()
         core.CGGetActiveDisplayList(self.max_displays, active_displays, ctypes.byref(display_count))
-        rotations = {0.0: "normal", 90.0: "right", -90.0: "left"}
         for idx in range(display_count.value):
             display = active_displays[idx]
             rect = core.CGDisplayBounds(display)
             rect = core.CGRectStandardize(rect)
             width, height = rect.size.width, rect.size.height
-            rot = core.CGDisplayRotation(display)
-            if rotations[rot] in ["left", "right"]:
+            if core.CGDisplayRotation(display) in {90.0, -90.0}:
+                # {0.0: "normal", 90.0: "right", -90.0: "left"}
                 width, height = height, width
             self._monitors.append(
                 {
                     "left": int_(rect.origin.x),
                     "top": int_(rect.origin.y),
                     "width": int_(width),
                     "height": int_(height),
```

### Comparing `mss-8.0.3/src/mss/factory.py` & `mss-9.0.0/src/mss/factory.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/mss/linux.py` & `mss-9.0.0/src/mss/linux.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,18 +61,14 @@
         ("error_code", c_ubyte),  # error code of failed request
         ("request_code", c_ubyte),  # major op-code of failed request
         ("minor_code", c_ubyte),  # minor op-code of failed request
         ("resourceid", c_void_p),  # resource ID
     ]
 
 
-# TODO: remove in v9.0.0
-Event = XErrorEvent
-
-
 class XFixesCursorImage(Structure):
     """
     Cursor structure.
     /usr/include/X11/extensions/Xfixes.h
     https://github.com/freedesktop/xorg-libXfixes/blob/libXfixes-6.0.0/include/X11/extensions/Xfixes.h#L96
     """
 
@@ -219,15 +215,15 @@
         "type": evt.type,
     }
 
     return 0
 
 
 def _validate(retval: int, func: Any, args: Tuple[Any, Any], /) -> Tuple[Any, Any]:
-    """Validate the returned value of a Xlib or XRANDR function."""
+    """Validate the returned value of a C function call."""
 
     thread = current_thread()
     if retval != 0 and thread not in _ERROR:
         return args
 
     details = _ERROR.pop(thread, {})
     raise ScreenShotError(f"{func.__name__}() failed", details=details)
@@ -313,37 +309,39 @@
 
         self._set_cfunctions()
 
         # Install the error handler to prevent interpreter crashes: any error will raise a ScreenShotError exception
         self._handles.original_error_handler = self.xlib.XSetErrorHandler(_error_handler)
 
         self._handles.display = self.xlib.XOpenDisplay(display)
+        if not self._handles.display:
+            raise ScreenShotError(f"Unable to open display: {display!r}.")
 
         if not self._is_extension_enabled("RANDR"):
             raise ScreenShotError("Xrandr not enabled.")
 
         self._handles.root = self.xlib.XDefaultRootWindow(self._handles.display)
 
         # Fix for XRRGetScreenResources and XGetImage:
         #     expected LP_Display instance instead of LP_XWindowAttributes
         self._handles.drawable = cast(self._handles.root, POINTER(Display))
 
     def close(self) -> None:
         # Remove our error handler
-        if self._handles.original_error_handler is not None:
+        if self._handles.original_error_handler:
             # It's required when exiting MSS to prevent letting `_error_handler()` as default handler.
             # Doing so would crash when using Tk/Tkinter, see issue #220.
             # Interesting technical stuff can be found here:
             #     https://core.tcl-lang.org/tk/file?name=generic/tkError.c&ci=a527ef995862cb50
             #     https://github.com/tcltk/tk/blob/b9cdafd83fe77499ff47fa373ce037aff3ae286a/generic/tkError.c
             self.xlib.XSetErrorHandler(self._handles.original_error_handler)
             self._handles.original_error_handler = None
 
         # Clean-up
-        if self._handles.display is not None:
+        if self._handles.display:
             self.xlib.XCloseDisplay(self._handles.display)
             self._handles.display = None
             self._handles.drawable = None
             self._handles.root = None
 
         # Also empty the error dict
         _ERROR.clear()
```

### Comparing `mss-8.0.3/src/mss/screenshot.py` & `mss-9.0.0/src/mss/screenshot.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/mss/tools.py` & `mss-9.0.0/src/mss/tools.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/mss/windows.py` & `mss-9.0.0/src/mss/windows.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 This is part of the MSS Python's module.
 Source: https://github.com/BoboTiG/python-mss
 """
 import ctypes
 import sys
-import threading
-from ctypes import POINTER, WINFUNCTYPE, Structure, c_void_p
+from ctypes import POINTER, WINFUNCTYPE, Structure, c_int, c_void_p
 from ctypes.wintypes import (
     BOOL,
     DOUBLE,
     DWORD,
     HBITMAP,
     HDC,
     HGDIOBJ,
@@ -18,15 +17,16 @@
     LONG,
     LPARAM,
     LPRECT,
     RECT,
     UINT,
     WORD,
 )
-from typing import Any, Dict, Optional
+from threading import local
+from typing import Any, Optional
 
 from .base import MSSBase
 from .exception import ScreenShotError
 from .models import CFunctions, Monitor
 from .screenshot import ScreenShot
 
 __all__ = ("MSS",)
@@ -74,61 +74,70 @@
 # Available attr: gdi32, user32.
 #
 # Note: keep it sorted by cfunction.
 CFUNCTIONS: CFunctions = {
     "BitBlt": ("gdi32", [HDC, INT, INT, INT, INT, HDC, INT, INT, DWORD], BOOL),
     "CreateCompatibleBitmap": ("gdi32", [HDC, INT, INT], HBITMAP),
     "CreateCompatibleDC": ("gdi32", [HDC], HDC),
+    "DeleteDC": ("gdi32", [HDC], HDC),
     "DeleteObject": ("gdi32", [HGDIOBJ], INT),
     "EnumDisplayMonitors": ("user32", [HDC, c_void_p, MONITORNUMPROC, LPARAM], BOOL),
     "GetDeviceCaps": ("gdi32", [HWND, INT], INT),
     "GetDIBits": ("gdi32", [HDC, HBITMAP, UINT, UINT, c_void_p, POINTER(BITMAPINFO), UINT], BOOL),
     "GetSystemMetrics": ("user32", [INT], INT),
     "GetWindowDC": ("user32", [HWND], HDC),
+    "ReleaseDC": ("user32", [HWND, HDC], c_int),
     "SelectObject": ("gdi32", [HDC, HGDIOBJ], HGDIOBJ),
 }
 
 
 class MSS(MSSBase):
     """Multiple ScreenShots implementation for Microsoft Windows."""
 
-    __slots__ = {"_bbox", "_bmi", "_data", "gdi32", "user32"}
-
-    # Class attributes instanced one time to prevent resource leaks.
-    bmp = None
-    memdc = None
-
-    # A dict to maintain *srcdc* values created by multiple threads.
-    _srcdc_dict: Dict[threading.Thread, int] = {}
+    __slots__ = {"gdi32", "user32", "_handles"}
 
     def __init__(self, /, **kwargs: Any) -> None:
         """Windows initialisations."""
 
         super().__init__(**kwargs)
 
         self.user32 = ctypes.WinDLL("user32")
         self.gdi32 = ctypes.WinDLL("gdi32")
         self._set_cfunctions()
         self._set_dpi_awareness()
 
-        self._bbox = {"height": 0, "width": 0}
-        self._data: ctypes.Array[ctypes.c_char] = ctypes.create_string_buffer(0)
-
-        srcdc = self._get_srcdc()
-        if not MSS.memdc:
-            MSS.memdc = self.gdi32.CreateCompatibleDC(srcdc)
+        # Available thread-specific variables
+        self._handles = local()
+        self._handles.region_width_height = (0, 0)
+        self._handles.bmp = None
+        self._handles.srcdc = self.user32.GetWindowDC(0)
+        self._handles.memdc = self.gdi32.CreateCompatibleDC(self._handles.srcdc)
 
         bmi = BITMAPINFO()
         bmi.bmiHeader.biSize = ctypes.sizeof(BITMAPINFOHEADER)
         bmi.bmiHeader.biPlanes = 1  # Always 1
         bmi.bmiHeader.biBitCount = 32  # See grab.__doc__ [2]
         bmi.bmiHeader.biCompression = 0  # 0 = BI_RGB (no compression)
         bmi.bmiHeader.biClrUsed = 0  # See grab.__doc__ [3]
         bmi.bmiHeader.biClrImportant = 0  # See grab.__doc__ [3]
-        self._bmi = bmi
+        self._handles.bmi = bmi
+
+    def close(self) -> None:
+        # Clean-up
+        if self._handles.bmp:
+            self.gdi32.DeleteObject(self._handles.bmp)
+            self._handles.bmp = None
+
+        if self._handles.memdc:
+            self.gdi32.DeleteDC(self._handles.memdc)
+            self._handles.memdc = None
+
+        if self._handles.srcdc:
+            self.user32.ReleaseDC(0, self._handles.srcdc)
+            self._handles.srcdc = None
 
     def _set_cfunctions(self) -> None:
         """Set all ctypes functions and attach them to attributes."""
 
         cfactory = self._cfactory
         attrs = {
             "gdi32": self.gdi32,
@@ -145,34 +154,17 @@
             # Windows 8.1+
             # Here 2 = PROCESS_PER_MONITOR_DPI_AWARE, which means:
             #     per monitor DPI aware. This app checks for the DPI when it is
             #     created and adjusts the scale factor whenever the DPI changes.
             #     These applications are not automatically scaled by the system.
             ctypes.windll.shcore.SetProcessDpiAwareness(2)
         elif (6, 0) <= version < (6, 3):
-            # Windows Vista, 7, 8 and Server 2012
+            # Windows Vista, 7, 8, and Server 2012
             self.user32.SetProcessDPIAware()
 
-    def _get_srcdc(self) -> int:
-        """
-        Retrieve a thread-safe HDC from GetWindowDC().
-        In multithreading, if the thread that creates *srcdc* is dead, *srcdc* will
-        no longer be valid to grab the screen. The *srcdc* attribute is replaced
-        with *_srcdc_dict* to maintain the *srcdc* values in multithreading.
-        Since the current thread and main thread are always alive, reuse their *srcdc* value first.
-        """
-        cur_thread, main_thread = threading.current_thread(), threading.main_thread()
-        current_srcdc = MSS._srcdc_dict.get(cur_thread) or MSS._srcdc_dict.get(main_thread)
-        if current_srcdc:
-            srcdc = current_srcdc
-        else:
-            srcdc = self.user32.GetWindowDC(0)
-            MSS._srcdc_dict[cur_thread] = srcdc
-        return srcdc
-
     def _monitors_impl(self) -> None:
         """Get positions of monitors. It will populate self._monitors."""
 
         int_ = int
         user32 = self.user32
         get_system_metrics = user32.GetSystemMetrics
 
@@ -236,40 +228,31 @@
 
         When biClrUsed and biClrImportant are set to zero, there
         is "no" color table, so we can read the pixels of the bitmap
         retrieved by gdi32.GetDIBits() as a sequence of RGB values.
         Thanks to http://stackoverflow.com/a/3688682
         """
 
-        srcdc, memdc = self._get_srcdc(), MSS.memdc
+        srcdc, memdc = self._handles.srcdc, self._handles.memdc
+        gdi = self.gdi32
         width, height = monitor["width"], monitor["height"]
 
-        if (self._bbox["height"], self._bbox["width"]) != (height, width):
-            self._bbox = monitor
-            self._bmi.bmiHeader.biWidth = width
-            self._bmi.bmiHeader.biHeight = -height  # Why minus? [1]
-            self._data = ctypes.create_string_buffer(width * height * 4)  # [2]
-            if MSS.bmp:
-                self.gdi32.DeleteObject(MSS.bmp)
-            MSS.bmp = self.gdi32.CreateCompatibleBitmap(srcdc, width, height)
-            self.gdi32.SelectObject(memdc, MSS.bmp)
-
-        self.gdi32.BitBlt(
-            memdc,
-            0,
-            0,
-            width,
-            height,
-            srcdc,
-            monitor["left"],
-            monitor["top"],
-            SRCCOPY | CAPTUREBLT,
-        )
-        bits = self.gdi32.GetDIBits(memdc, MSS.bmp, 0, height, self._data, self._bmi, DIB_RGB_COLORS)
+        if self._handles.region_width_height != (width, height):
+            self._handles.region_width_height = (width, height)
+            self._handles.bmi.bmiHeader.biWidth = width
+            self._handles.bmi.bmiHeader.biHeight = -height  # Why minus? [1]
+            self._handles.data = ctypes.create_string_buffer(width * height * 4)  # [2]
+            if self._handles.bmp:
+                gdi.DeleteObject(self._handles.bmp)
+            self._handles.bmp = gdi.CreateCompatibleBitmap(srcdc, width, height)
+            gdi.SelectObject(memdc, self._handles.bmp)
+
+        gdi.BitBlt(memdc, 0, 0, width, height, srcdc, monitor["left"], monitor["top"], SRCCOPY | CAPTUREBLT)
+        bits = gdi.GetDIBits(memdc, self._handles.bmp, 0, height, self._handles.data, self._handles.bmi, DIB_RGB_COLORS)
         if bits != height:
             raise ScreenShotError("gdi32.GetDIBits() failed.")
 
-        return self.cls_image(bytearray(self._data), monitor)
+        return self.cls_image(bytearray(self._handles.data), monitor)
 
     def _cursor_impl(self) -> Optional[ScreenShot]:
         """Retrieve all cursor data. Pixels have to be RGB."""
         return None
```

### Comparing `mss-8.0.3/src/mss.egg-info/PKG-INFO` & `mss-9.0.0/src/mss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mss
-Version: 8.0.3
+Version: 9.0.0
 Summary: An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 Home-page: https://github.com/BoboTiG/python-mss
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: MIT
 Project-URL: Documentation, https://python-mss.readthedocs.io
 Project-URL: Source, https://github.com/BoboTiG/python-mss
```

### Comparing `mss-8.0.3/src/mss.egg-info/SOURCES.txt` & `mss-9.0.0/src/mss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/tests/bench_bgra2rgb.py` & `mss-9.0.0/src/tests/bench_bgra2rgb.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/tests/bench_general.py` & `mss-9.0.0/src/tests/bench_general.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/tests/conftest.py` & `mss-9.0.0/src/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This is part of the MSS Python's module.
 Source: https://github.com/BoboTiG/python-mss
 """
 import glob
 import os
+import platform
 from hashlib import md5
 from pathlib import Path
 from zipfile import ZipFile
 
 import pytest
 
 from mss import mss
@@ -51,13 +52,17 @@
     assert md5(data).hexdigest() == "125696266e2a8f5240f6bc17e4df98c6"
     return data
 
 
 @pytest.fixture(scope="session")
 def pixel_ratio() -> int:
     """Get the pixel, used to adapt test checks."""
+
+    if platform.system().lower() != "darwin":
+        return 1
+
     # Grab a 1x1 screenshot
     region = {"top": 0, "left": 0, "width": 1, "height": 1}
 
-    with mss(display=os.getenv("DISPLAY")) as sct:
-        # On macOS with Retina display, the width will be 2 instead of 1
+    with mss() as sct:
+        # On macOS with Retina display, the width can be 2 instead of 1
         return sct.grab(region).size[0]
```

### Comparing `mss-8.0.3/src/tests/res/monitor-1024x768.raw.zip` & `mss-9.0.0/src/tests/res/monitor-1024x768.raw.zip`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/tests/test_cls_image.py` & `mss-9.0.0/src/tests/test_cls_image.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/tests/test_find_monitors.py` & `mss-9.0.0/src/tests/test_find_monitors.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/tests/test_get_pixels.py` & `mss-9.0.0/src/tests/test_get_pixels.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 This is part of the MSS Python's module.
 Source: https://github.com/BoboTiG/python-mss
 """
+
+import itertools
 import os
 
 import pytest
 
 from mss import mss
 from mss.base import ScreenShot
 from mss.exception import ScreenShotError
@@ -17,39 +19,31 @@
             image = sct.grab(mon)
             assert isinstance(image, ScreenShot)
             assert isinstance(image.raw, bytearray)
             assert isinstance(image.rgb, bytes)
 
 
 def test_grab_part_of_screen(pixel_ratio):
-    monitor = {"top": 160, "left": 160, "width": 160, "height": 160}
-    with mss(display=os.getenv("DISPLAY")) as sct:
-        image = sct.grab(monitor)
-    assert isinstance(image, ScreenShot)
-    assert isinstance(image.raw, bytearray)
-    assert isinstance(image.rgb, bytes)
-    assert image.top == 160
-    assert image.left == 160
-    assert image.width == 160 * pixel_ratio
-    assert image.height == 160 * pixel_ratio
-
-
-def test_grab_part_of_screen_rounded(pixel_ratio):
-    monitor = {"top": 160, "left": 160, "width": 161, "height": 159}
     with mss(display=os.getenv("DISPLAY")) as sct:
-        image = sct.grab(monitor)
-    assert isinstance(image, ScreenShot)
-    assert isinstance(image.raw, bytearray)
-    assert isinstance(image.rgb, bytes)
-    assert image.top == 160
-    assert image.left == 160
-    assert image.width == 161 * pixel_ratio
-    assert image.height == 159 * pixel_ratio
-
+        for width, height in itertools.product(range(1, 42), range(1, 42)):
+            monitor = {"top": 160, "left": 160, "width": width, "height": height}
+            image = sct.grab(monitor)
+
+            assert image.top == 160
+            assert image.left == 160
+            assert image.width == width * pixel_ratio
+            assert image.height == height * pixel_ratio
+
+
+def test_get_pixel(raw: bytes):
+    image = ScreenShot.from_size(bytearray(raw), 1024, 768)
+    assert image.width == 1024
+    assert image.height == 768
+    assert len(image.pixels) == 768
+    assert len(image.pixels[0]) == 1024
+
+    assert image.pixel(0, 0) == (135, 152, 192)
+    assert image.pixel(image.width // 2, image.height // 2) == (0, 0, 0)
+    assert image.pixel(image.width - 1, image.height - 1) == (135, 152, 192)
 
-def test_grab_individual_pixels():
-    monitor = {"top": 160, "left": 160, "width": 222, "height": 42}
-    with mss(display=os.getenv("DISPLAY")) as sct:
-        image = sct.grab(monitor)
-    assert isinstance(image.pixel(0, 0), tuple)
     with pytest.raises(ScreenShotError):
         image.pixel(image.width + 1, 12)
```

### Comparing `mss-8.0.3/src/tests/test_gnu_linux.py` & `mss-9.0.0/src/tests/test_gnu_linux.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,31 +8,27 @@
 import pytest
 
 import mss
 import mss.linux
 from mss.base import MSSBase
 from mss.exception import ScreenShotError
 
-xvfbwrapper = pytest.importorskip("xvfbwrapper")
+pyvirtualdisplay = pytest.importorskip("pyvirtualdisplay")
 
 PYPY = platform.python_implementation() == "PyPy"
 
 WIDTH = 200
 HEIGHT = 200
 DEPTH = 24
 
 
 @pytest.fixture
 def display() -> str:
-    vdisplay = xvfbwrapper.Xvfb(width=WIDTH, height=HEIGHT, colordepth=DEPTH)
-    vdisplay.start()
-    try:
-        yield f":{vdisplay.new_display}"
-    finally:
-        vdisplay.stop()
+    with pyvirtualdisplay.Display(size=(WIDTH, HEIGHT), color_depth=DEPTH) as vdisplay:
+        yield vdisplay.new_display_var
 
 
 @pytest.mark.skipif(PYPY, reason="Failure on PyPy")
 def test_factory_systems(monkeypatch):
     """
     Here, we are testing all systems.
 
@@ -68,14 +64,19 @@
         pass
 
     # Bad `display` (missing ":" in front of the number)
     with pytest.raises(ScreenShotError):
         with mss.mss(display="0"):
             pass
 
+    # Invalid `display` that is not trivially distinguishable.
+    with pytest.raises(ScreenShotError):
+        with mss.mss(display=":INVALID"):
+            pass
+
     # No `DISPLAY` in envars
     monkeypatch.delenv("DISPLAY")
     with pytest.raises(ScreenShotError):
         with mss.mss():
             pass
 
 
@@ -105,22 +106,18 @@
 def test_xrandr_extension_exists_but_is_not_enabled(display: str):
     with pytest.raises(ScreenShotError):
         with mss.mss(display=display):
             pass
 
 
 def test_unsupported_depth():
-    vdisplay = xvfbwrapper.Xvfb(width=WIDTH, height=HEIGHT, colordepth=8)
-    vdisplay.start()
-    try:
+    with pyvirtualdisplay.Display(size=(WIDTH, HEIGHT), color_depth=8) as vdisplay:
         with pytest.raises(ScreenShotError):
-            with mss.mss(display=f":{vdisplay.new_display}") as sct:
+            with mss.mss(display=vdisplay.new_display_var) as sct:
                 sct.grab(sct.monitors[1])
-    finally:
-        vdisplay.stop()
 
 
 def test_region_out_of_monitor_bounds(display: str):
     monitor = {"left": -30, "top": 0, "width": WIDTH, "height": HEIGHT}
 
     assert not mss.linux._ERROR
```

### Comparing `mss-8.0.3/src/tests/test_implementation.py` & `mss-9.0.0/src/tests/test_implementation.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/tests/test_issue_220.py` & `mss-9.0.0/src/tests/test_issue_220.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/tests/test_leaks.py` & `mss-9.0.0/src/tests/test_leaks.py`

 * *Files 9% similar despite different names*

```diff
@@ -90,27 +90,23 @@
         sct.grab(bounding_box_test)
         bounding_box_score = {"top": 110, "left": 110, "width": 100, "height": 100}
         sct.grab(bounding_box_score)
 
 
 def regression_issue_210():
     """Regression test for issue #210: multiple X servers."""
-    xvfbwrapper = pytest.importorskip("xvfbwrapper")
+    pyvirtualdisplay = pytest.importorskip("pyvirtualdisplay")
 
-    vdisplay = xvfbwrapper.Xvfb(width=1920, height=1080, colordepth=24)
-    vdisplay.start()
-    with mss():
-        pass
-    vdisplay.stop()
-
-    vdisplay = xvfbwrapper.Xvfb(width=1920, height=1080, colordepth=24)
-    vdisplay.start()
-    with mss():
-        pass
-    vdisplay.stop()
+    with pyvirtualdisplay.Display(size=(1920, 1080), color_depth=24):
+        with mss():
+            pass
+
+    with pyvirtualdisplay.Display(size=(1920, 1080), color_depth=24):
+        with mss():
+            pass
 
 
 @pytest.mark.skipif(OS == "darwin", reason="No possible leak on macOS.")
 @pytest.mark.parametrize(
     "func",
     (
         # bound_instance_without_cm,
```

### Comparing `mss-8.0.3/src/tests/test_macos.py` & `mss-9.0.0/src/tests/test_macos.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/tests/test_save.py` & `mss-9.0.0/src/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/tests/test_setup.py` & `mss-9.0.0/src/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/tests/test_third_party.py` & `mss-9.0.0/src/tests/test_third_party.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/tests/test_tools.py` & `mss-9.0.0/src/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.3/src/tests/test_windows.py` & `mss-9.0.0/src/tests/test_windows.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,49 +20,79 @@
         monkeypatch.setattr(sct.gdi32, "GetDIBits", lambda *args: 0)
         with pytest.raises(ScreenShotError):
             sct.shot()
 
 
 def test_region_caching():
     """The region to grab is cached, ensure this is well-done."""
-    from mss.windows import MSS
-
     with mss.mss() as sct:
-        # Reset the current BMP
-        if MSS.bmp:
-            sct.gdi32.DeleteObject(MSS.bmp)
-            MSS.bmp = None
-
         # Grab the area 1
         region1 = {"top": 0, "left": 0, "width": 200, "height": 200}
         sct.grab(region1)
-        bmp1 = id(MSS.bmp)
+        bmp1 = id(sct._handles.bmp)
 
         # Grab the area 2, the cached BMP is used
         # Same sizes but different positions
         region2 = {"top": 200, "left": 200, "width": 200, "height": 200}
         sct.grab(region2)
-        bmp2 = id(MSS.bmp)
+        bmp2 = id(sct._handles.bmp)
         assert bmp1 == bmp2
 
         # Grab the area 2 again, the cached BMP is used
         sct.grab(region2)
-        assert bmp2 == id(MSS.bmp)
+        assert bmp2 == id(sct._handles.bmp)
+
+
+def test_region_not_caching():
+    """The region to grab is not bad cached previous grab."""
+    grab1 = mss.mss()
+    grab2 = mss.mss()
+
+    region1 = {"top": 0, "left": 0, "width": 100, "height": 100}
+    region2 = {"top": 0, "left": 0, "width": 50, "height": 1}
+    grab1.grab(region1)
+    bmp1 = id(grab1._handles.bmp)
+    grab2.grab(region2)
+    bmp2 = id(grab2._handles.bmp)
+    assert bmp1 != bmp2
+
+    # Grab the area 1, is not bad cached BMP previous grab the area 2
+    grab1.grab(region1)
+    bmp1 = id(grab1._handles.bmp)
+    assert bmp1 != bmp2
 
 
 def run_child_thread(loops):
     for _ in range(loops):
-        with mss.mss() as sct:
+        with mss.mss() as sct:  # New sct for every loop
             sct.grab(sct.monitors[1])
 
 
 def test_thread_safety():
     """Thread safety test for issue #150.
     The following code will throw a ScreenShotError exception if thread-safety is not guaranted.
     """
     # Let thread 1 finished ahead of thread 2
     thread1 = threading.Thread(target=run_child_thread, args=(30,))
     thread2 = threading.Thread(target=run_child_thread, args=(50,))
     thread1.start()
     thread2.start()
     thread1.join()
     thread2.join()
+
+
+def run_child_thread_bbox(loops, bbox):
+    with mss.mss() as sct:  # One sct for all loops
+        for _ in range(loops):
+            sct.grab(bbox)
+
+
+def test_thread_safety_regions():
+    """Thread safety test for different regions
+    The following code will throw a ScreenShotError exception if thread-safety is not guaranted.
+    """
+    thread1 = threading.Thread(target=run_child_thread_bbox, args=(100, (0, 0, 100, 100)))
+    thread2 = threading.Thread(target=run_child_thread_bbox, args=(100, (0, 0, 50, 1)))
+    thread1.start()
+    thread2.start()
+    thread1.join()
+    thread2.join()
```

