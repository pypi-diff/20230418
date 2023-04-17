# Comparing `tmp/netin-1.0.5.1.tar.gz` & `tmp/netin-1.0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netin-1.0.5.1.tar", last modified: Mon Apr 17 10:13:08 2023, max compression
+gzip compressed data, was "netin-1.0.5.2.tar", last modified: Mon Apr 17 13:05:46 2023, max compression
```

## Comparing `netin-1.0.5.1.tar` & `netin-1.0.5.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.793910 netin-1.0.5.1/
--rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.1/LICENSE
--rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.1/MANIFEST.in
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3705 2023-04-17 10:13:08.793910 netin-1.0.5.1/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2433 2023-04-16 07:53:42.000000 netin-1.0.5.1/README.rst
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.789910 netin-1.0.5.1/examples/
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.789910 netin-1.0.5.1/examples/directed/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.1/examples/directed/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.1/examples/directed/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.1/examples/directed/dpah.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.789910 netin-1.0.5.1/examples/undirected/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.1/examples/undirected/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.1/examples/undirected/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.1/examples/undirected/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.1/examples/undirected/patch.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.789910 netin-1.0.5.1/netin/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      353 2023-04-17 10:09:56.000000 netin-1.0.5.1/netin/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.789910 netin-1.0.5.1/netin/algorithms/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-06 13:44:46.000000 netin-1.0.5.1/netin/algorithms/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.793910 netin-1.0.5.1/netin/generators/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-14 21:19:23.000000 netin-1.0.5.1/netin/generators/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4078 2023-04-15 01:01:03.000000 netin-1.0.5.1/netin/generators/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     9214 2023-04-15 22:08:19.000000 netin-1.0.5.1/netin/generators/directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2385 2023-04-14 21:16:14.000000 netin-1.0.5.1/netin/generators/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3448 2023-04-15 21:55:31.000000 netin-1.0.5.1/netin/generators/dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    13362 2023-04-15 21:45:47.000000 netin-1.0.5.1/netin/generators/graph.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6332 2023-04-15 18:01:34.000000 netin-1.0.5.1/netin/generators/h.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1948 2023-04-14 21:16:41.000000 netin-1.0.5.1/netin/generators/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4363 2023-04-16 07:05:49.000000 netin-1.0.5.1/netin/generators/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3587 2023-04-14 21:16:55.000000 netin-1.0.5.1/netin/generators/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3951 2023-04-15 22:08:18.000000 netin-1.0.5.1/netin/generators/patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6339 2023-04-14 23:53:00.000000 netin-1.0.5.1/netin/generators/tc.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.793910 netin-1.0.5.1/netin/generators/tests/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.1/netin/generators/tests/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.1/netin/generators/tests/test_directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.1/netin/generators/tests/test_dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.1/netin/generators/tests/test_patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.1/netin/generators/tests/test_undirected.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     7000 2023-04-15 22:08:18.000000 netin-1.0.5.1/netin/generators/undirected.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.793910 netin-1.0.5.1/netin/stats/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      288 2023-04-15 18:06:03.000000 netin-1.0.5.1/netin/stats/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1854 2023-04-15 19:33:04.000000 netin-1.0.5.1/netin/stats/distributions.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2753 2023-04-15 22:08:18.000000 netin-1.0.5.1/netin/stats/ranking.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.793910 netin-1.0.5.1/netin/utils/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.1/netin/utils/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1075 2023-04-15 18:01:34.000000 netin-1.0.5.1/netin/utils/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1221 2023-04-13 15:18:30.000000 netin-1.0.5.1/netin/utils/validator.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.793910 netin-1.0.5.1/netin/viz/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      426 2023-04-15 18:04:47.000000 netin-1.0.5.1/netin/viz/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      466 2023-04-17 10:09:00.000000 netin-1.0.5.1/netin/viz/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    15383 2023-04-17 10:09:00.000000 netin-1.0.5.1/netin/viz/handlers.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.789910 netin-1.0.5.1/netin.egg-info/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3705 2023-04-17 10:13:08.000000 netin-1.0.5.1/netin.egg-info/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1237 2023-04-17 10:13:08.000000 netin-1.0.5.1/netin.egg-info/SOURCES.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-17 10:13:08.000000 netin-1.0.5.1/netin.egg-info/dependency_links.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.1/netin.egg-info/not-zip-safe
--rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-17 10:13:08.000000 netin-1.0.5.1/netin.egg-info/requires.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-17 10:13:08.000000 netin-1.0.5.1/netin.egg-info/top_level.txt
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 10:13:08.793910 netin-1.0.5.1/requirements/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.1/requirements/default.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.1/requirements/test.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-17 10:13:08.793910 netin-1.0.5.1/setup.cfg
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4247 2023-04-16 07:47:09.000000 netin-1.0.5.1/setup.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 13:05:46.136791 netin-1.0.5.2/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.5.2/LICENSE
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.5.2/MANIFEST.in
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3705 2023-04-17 13:05:46.136791 netin-1.0.5.2/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2433 2023-04-16 07:53:42.000000 netin-1.0.5.2/README.rst
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 13:05:46.132791 netin-1.0.5.2/examples/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 13:05:46.132791 netin-1.0.5.2/examples/directed/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.5.2/examples/directed/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.5.2/examples/directed/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.5.2/examples/directed/dpah.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 13:05:46.132791 netin-1.0.5.2/examples/undirected/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.5.2/examples/undirected/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.5.2/examples/undirected/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.5.2/examples/undirected/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.5.2/examples/undirected/patch.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 13:05:46.132791 netin-1.0.5.2/netin/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      353 2023-04-17 13:05:12.000000 netin-1.0.5.2/netin/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 13:05:46.136791 netin-1.0.5.2/netin/algorithms/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-06 13:44:46.000000 netin-1.0.5.2/netin/algorithms/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 13:05:46.136791 netin-1.0.5.2/netin/generators/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-14 21:19:23.000000 netin-1.0.5.2/netin/generators/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4078 2023-04-15 01:01:03.000000 netin-1.0.5.2/netin/generators/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     9214 2023-04-15 22:08:19.000000 netin-1.0.5.2/netin/generators/directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2385 2023-04-14 21:16:14.000000 netin-1.0.5.2/netin/generators/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3448 2023-04-15 21:55:31.000000 netin-1.0.5.2/netin/generators/dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    13362 2023-04-15 21:45:47.000000 netin-1.0.5.2/netin/generators/graph.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6332 2023-04-15 18:01:34.000000 netin-1.0.5.2/netin/generators/h.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1948 2023-04-14 21:16:41.000000 netin-1.0.5.2/netin/generators/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4363 2023-04-16 07:05:49.000000 netin-1.0.5.2/netin/generators/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3587 2023-04-14 21:16:55.000000 netin-1.0.5.2/netin/generators/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3951 2023-04-15 22:08:18.000000 netin-1.0.5.2/netin/generators/patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6339 2023-04-14 23:53:00.000000 netin-1.0.5.2/netin/generators/tc.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 13:05:46.136791 netin-1.0.5.2/netin/generators/tests/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.5.2/netin/generators/tests/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.5.2/netin/generators/tests/test_directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.5.2/netin/generators/tests/test_dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.5.2/netin/generators/tests/test_patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.5.2/netin/generators/tests/test_undirected.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     7000 2023-04-15 22:08:18.000000 netin-1.0.5.2/netin/generators/undirected.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 13:05:46.136791 netin-1.0.5.2/netin/stats/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      288 2023-04-15 18:06:03.000000 netin-1.0.5.2/netin/stats/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1854 2023-04-15 19:33:04.000000 netin-1.0.5.2/netin/stats/distributions.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2753 2023-04-15 22:08:18.000000 netin-1.0.5.2/netin/stats/ranking.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 13:05:46.136791 netin-1.0.5.2/netin/utils/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.5.2/netin/utils/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1075 2023-04-15 18:01:34.000000 netin-1.0.5.2/netin/utils/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1221 2023-04-13 15:18:30.000000 netin-1.0.5.2/netin/utils/validator.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 13:05:46.136791 netin-1.0.5.2/netin/viz/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      425 2023-04-17 12:53:55.000000 netin-1.0.5.2/netin/viz/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      466 2023-04-17 10:09:00.000000 netin-1.0.5.2/netin/viz/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    15777 2023-04-17 12:55:53.000000 netin-1.0.5.2/netin/viz/handlers.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 13:05:46.136791 netin-1.0.5.2/netin.egg-info/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3705 2023-04-17 13:05:46.000000 netin-1.0.5.2/netin.egg-info/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1237 2023-04-17 13:05:46.000000 netin-1.0.5.2/netin.egg-info/SOURCES.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-17 13:05:46.000000 netin-1.0.5.2/netin.egg-info/dependency_links.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.5.2/netin.egg-info/not-zip-safe
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-17 13:05:46.000000 netin-1.0.5.2/netin.egg-info/requires.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-17 13:05:46.000000 netin-1.0.5.2/netin.egg-info/top_level.txt
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-17 13:05:46.136791 netin-1.0.5.2/requirements/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.5.2/requirements/default.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.5.2/requirements/test.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-17 13:05:46.136791 netin-1.0.5.2/setup.cfg
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4247 2023-04-16 07:47:09.000000 netin-1.0.5.2/setup.py
```

### Comparing `netin-1.0.5.1/LICENSE` & `netin-1.0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/PKG-INFO` & `netin-1.0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.1
+Version: 1.0.5.2
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.1/README.rst` & `netin-1.0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/dh.py` & `netin-1.0.5.2/netin/generators/dh.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/directed.py` & `netin-1.0.5.2/netin/generators/directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/dpa.py` & `netin-1.0.5.2/netin/generators/dpa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/dpah.py` & `netin-1.0.5.2/netin/generators/dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/graph.py` & `netin-1.0.5.2/netin/generators/graph.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/h.py` & `netin-1.0.5.2/netin/generators/h.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/pa.py` & `netin-1.0.5.2/netin/generators/pa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/pah.py` & `netin-1.0.5.2/netin/generators/pah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/patc.py` & `netin-1.0.5.2/netin/generators/patc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/patch.py` & `netin-1.0.5.2/netin/generators/patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/tc.py` & `netin-1.0.5.2/netin/generators/tc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/tests/test_directed.py` & `netin-1.0.5.2/netin/generators/tests/test_directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/tests/test_dpah.py` & `netin-1.0.5.2/netin/generators/tests/test_dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/tests/test_patch.py` & `netin-1.0.5.2/netin/generators/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/tests/test_undirected.py` & `netin-1.0.5.2/netin/generators/tests/test_undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/generators/undirected.py` & `netin-1.0.5.2/netin/generators/undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/stats/distributions.py` & `netin-1.0.5.2/netin/stats/distributions.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/stats/ranking.py` & `netin-1.0.5.2/netin/stats/ranking.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/utils/constants.py` & `netin-1.0.5.2/netin/utils/constants.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/utils/validator.py` & `netin-1.0.5.2/netin/utils/validator.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/netin/viz/handlers.py` & `netin-1.0.5.2/netin/viz/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,16 @@
     maj_patch = mpatches.Patch(color=COLOR_MAJORITY, label='majority')
     min_patch = mpatches.Patch(color=COLOR_MINORITY, label='minority')
     bbox = kwargs.get('bbox', (1.04, 1))
     loc = kwargs.get('loc', "upper left")
     fig.legend(handles=[maj_patch, min_patch], bbox_to_anchor=bbox, loc=loc)
 
 
-def plot_graphs(iter_graph: Set[Graph], share_pos=False, fn=None, **kwargs):
+def plot_graph(data: Union[Graph, Set[Graph]], share_pos=False, fn=None, **kwargs):
+    iter_graph = [data] if isinstance(data, Graph) else data
     nc = kwargs.pop('nc', None)
     nc, nr = _get_grid_info(len(iter_graph), nc=nc)
     cell_size = kwargs.get('cell_size', DEFAULT_CELL_SIZE)
 
     fig, axes = plt.subplots(nr, nc, figsize=(nc * cell_size, nr * cell_size), sharex=False, sharey=False)
     node_size = kwargs.get('node_size', 1)
     node_shape = kwargs.get('node_shape', 'o')
@@ -90,16 +91,20 @@
     edge_style = kwargs.get('edge_style', 'solid')
     edge_arrows = kwargs.get('edge_arrows', True)
     arrow_style = kwargs.get('arrow_style', '-|>')
     arrow_size = kwargs.get('arrow_size', 2)
 
     pos = None
     same_n = len(set([g.number_of_nodes() for g in iter_graph])) == 1
-    for c, g in enumerate(iter_graph):
-        ax = axes[c]
+    for cell, g in enumerate(iter_graph):
+        row = cell // nc
+        col = cell % nc
+
+        ax = axes if nr == nc == 1 else axes[cell] if nr == 1 else axes[row, col]
+
         pos = nx.spring_layout(g) if pos is None or not share_pos or not same_n else pos
 
         # nodes
         maj = g.graph['class_values'][g.graph['class_labels'].index("M")]
         nodes, node_colors = zip(
             *[(node, COLOR_MAJORITY if data[g.graph['class_attribute']] == maj else COLOR_MINORITY)
               for node, data in g.nodes(data=True)])
@@ -126,36 +131,41 @@
                       get_x_y_from_df_fnc: callable, fn=None, **kwargs):
     iter_data = [data] if type(data) == pd.DataFrame else data
     nc = kwargs.pop('nc', None)
     nc, nr = _get_grid_info(len(iter_data), nc=nc)
     cell_size = kwargs.pop('cell_size', DEFAULT_CELL_SIZE)
     iter_column = [col_name] * (nc * nr) if type(col_name) == str else col_name
 
+    # whole plot
     scatter = kwargs.pop('scatter', False)
-    hue = kwargs.pop('hue', None)
     sharex = kwargs.pop('sharex', False)
     sharey = kwargs.pop('sharey', False)
     xy_fnc_name = get_x_y_from_df_fnc.__name__
     ylabel = xy_fnc_name.replace("get_", '').upper()
     ylabel = kwargs.pop('ylabel', ylabel)
     xlabel = kwargs.pop('xlabel', None)
     xlim = kwargs.pop('xlim', None)
     ylim = kwargs.pop('ylim', None)
     common_norm = kwargs.pop('common_norm', False)
     log_scale = kwargs.pop('log_scale', (False, False))
-    class_label_legend = kwargs.pop('class_label_legend', True)
     hline_fnc = kwargs.pop('hline_fnc', None)
     vline_fnc = kwargs.pop('vline_fnc', None)
+    wspace = kwargs.pop('wspace', None)
+    hspace = kwargs.pop('hspace', None)
     suptitle = kwargs.pop('suptitle', None)
+
+    # subplots
     cuts = kwargs.pop('cuts', None)
     gini_fnc = kwargs.pop('gini_fnc', None)
     me_fnc = kwargs.pop('me_fnc', None)
     beta = kwargs.pop('beta', None)
-    wspace = kwargs.pop('wspace', None)
-    hspace = kwargs.pop('hspace', None)
+
+    # outter legend
+    hue = kwargs.pop('hue', None)
+    class_label_legend = kwargs.pop('class_label_legend', True)
 
     w, h = cell_size if type(cell_size) == tuple else (cell_size, cell_size)
     fig, axes = plt.subplots(nr, nc, figsize=(nc * w, nr * h), sharex=sharex, sharey=sharey)
 
     for cell, df in enumerate(iter_data):
         row = cell // nc
         col = cell % nc
@@ -353,14 +363,15 @@
     sharey = kwargs.pop('sharey', False)
     log_scale = kwargs.pop('log_scale', (False, False))
     xlabel = kwargs.pop('xlabel', None)
     ylabel = kwargs.pop('ylabel', "p(X≥x)" if kind == "ccdf" else "p(X<x)" if kind == 'cdf' else "p(X=x)" if kind == 'pdf' else None)
     verbose = kwargs.pop('verbose', False)
     wspace = kwargs.pop('wspace', None)
     hspace = kwargs.pop('hspace', None)
+    suptitle = kwargs.pop('suptitle', None)
 
     # outer legend
     hue = kwargs.pop('hue', None)
     bbox = kwargs.pop('bbox', (1.0, 0.9))
 
     # inner legend
     fontsize = kwargs.pop('fontsize', None)
@@ -408,12 +419,18 @@
         if xlabel is None:
             ax.set_xlabel(_col_name)
         elif (sharex and row == nr - 1) or (not sharex):
             ax.set_xlabel(xlabel)
 
         ax.set_title(df.name)
 
-    # legend
-    if hue:
+    # suptitle
+    if suptitle is not None:
+        fig.suptitle(suptitle)
+
+    # legend (min, maj)
+    if hue and bbox:
         kwargs['bbox'] = bbox
         _add_class_legend(fig, **kwargs)
+
+    # save plot
     _save_plot(fig, fn, wspace=wspace, hspace=hspace, **kwargs)
```

### Comparing `netin-1.0.5.1/netin.egg-info/PKG-INFO` & `netin-1.0.5.2/netin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.5.1
+Version: 1.0.5.2
 Summary: Python package to study inequalities in social networks
 Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin-dev@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.5.1/netin.egg-info/SOURCES.txt` & `netin-1.0.5.2/netin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netin-1.0.5.1/setup.py` & `netin-1.0.5.2/setup.py`

 * *Files identical despite different names*

