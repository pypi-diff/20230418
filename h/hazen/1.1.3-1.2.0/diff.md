# Comparing `tmp/hazen-1.1.3.tar.gz` & `tmp/hazen-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazen-1.1.3.tar", last modified: Tue Feb 28 15:29:04 2023, max compression
+gzip compressed data, was "hazen-1.2.0.tar", last modified: Tue Apr 18 13:39:05 2023, max compression
```

## Comparing `hazen-1.1.3.tar` & `hazen-1.2.0.tar`

### file list

```diff
@@ -1,61 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:29:04.493920 hazen-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-28 15:28:53.000000 hazen-1.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-28 15:28:53.000000 hazen-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-02-28 15:29:04.493920 hazen-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-02-28 15:28:53.000000 hazen-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:29:04.485921 hazen-1.1.3/hazen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-02-28 15:29:04.000000 hazen-1.1.3/hazen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-02-28 15:29:04.000000 hazen-1.1.3/hazen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 15:29:04.000000 hazen-1.1.3/hazen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-28 15:29:04.000000 hazen-1.1.3/hazen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-28 15:29:04.000000 hazen-1.1.3/hazen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-28 15:29:04.000000 hazen-1.1.3/hazen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:29:04.489920 hazen-1.1.3/hazenlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/HazenTask.py
--rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:29:04.485921 hazen-1.1.3/hazenlib/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:29:04.489920 hazen-1.1.3/hazenlib/data/relaxometry/
--rw-r--r--   0 runner    (1001) docker     (123)   157178 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/data/relaxometry/Plate4_T1_signed
--rw-r--r--   0 runner    (1001) docker     (123)   168984 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/data/relaxometry/Plate4_T2
--rw-r--r--   0 runner    (1001) docker     (123)   157180 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/data/relaxometry/Plate5_T1_signed
--rw-r--r--   0 runner    (1001) docker     (123)   168984 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/data/relaxometry/Plate5_T2
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    47189 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/relaxometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:29:04.489920 hazen-1.1.3/hazenlib/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/tasks/acr_geometric_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/tasks/acr_ghosting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/tasks/acr_slice_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/tasks/acr_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/tasks/acr_uniformity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/tasks/ghosting.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/tasks/relaxometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/tasks/slice_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    35489 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/tasks/slice_width.py
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/tasks/snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/tasks/snr_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/tasks/spatial_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/tasks/uniformity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-02-28 15:28:53.000000 hazen-1.1.3/hazenlib/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-28 15:28:53.000000 hazen-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-02-28 15:29:04.493920 hazen-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:29:04.493920 hazen-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/test_acr_geometric_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/test_acr_ghosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/test_acr_slice_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/test_acr_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/test_acr_uniformity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/test_ghosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/test_hazenlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    31794 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/test_relaxometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/test_slice_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/test_slice_width.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/test_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/test_snr_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    39305 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/test_spatial_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-02-28 15:28:53.000000 hazen-1.1.3/tests/test_uniformity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:05.439765 hazen-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-18 13:38:53.000000 hazen-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-18 13:38:53.000000 hazen-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-04-18 13:39:05.439765 hazen-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-18 13:38:53.000000 hazen-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:05.435765 hazen-1.2.0/hazen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-04-18 13:39:05.000000 hazen-1.2.0/hazen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-18 13:39:05.000000 hazen-1.2.0/hazen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:39:05.000000 hazen-1.2.0/hazen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 13:39:05.000000 hazen-1.2.0/hazen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 13:39:05.000000 hazen-1.2.0/hazen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 13:39:05.000000 hazen-1.2.0/hazen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:05.435765 hazen-1.2.0/hazenlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/HazenTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:05.431765 hazen-1.2.0/hazenlib/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:05.435765 hazen-1.2.0/hazenlib/data/relaxometry/
+-rw-r--r--   0 runner    (1001) docker     (123)   157178 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/data/relaxometry/Plate4_T1_signed
+-rw-r--r--   0 runner    (1001) docker     (123)   168984 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/data/relaxometry/Plate4_T2
+-rw-r--r--   0 runner    (1001) docker     (123)   157180 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/data/relaxometry/Plate5_T1_signed
+-rw-r--r--   0 runner    (1001) docker     (123)   168984 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/data/relaxometry/Plate5_T2
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47189 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/relaxometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:05.439765 hazen-1.2.0/hazenlib/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/acr_geometric_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/acr_ghosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/acr_slice_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/acr_slice_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/acr_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/acr_spatial_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/acr_uniformity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/ghosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/relaxometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/slice_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35489 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/slice_width.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/snr_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/spatial_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/uniformity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 13:38:54.000000 hazen-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-18 13:39:05.443765 hazen-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:05.439765 hazen-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_acr_geometric_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_acr_ghosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_acr_slice_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_acr_slice_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_acr_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_acr_spatial_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_acr_uniformity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_ghosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_hazenlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31794 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_relaxometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_slice_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_slice_width.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_snr_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39521 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_spatial_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_uniformity.py
```

### Comparing `hazen-1.1.3/PKG-INFO` & `hazen-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hazen
-Version: 1.1.3
+Version: 1.2.0
 Summary: An automatic MRI QA tool
 Home-page: https://bitbucket.org/gsttmri/hazen
 Author: Shuaib, Haris
 Author-email: mohammad_haris.shuaib@kcl.ac.uk
 Requires-Python: <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -45,15 +45,15 @@
 - Slice position and width
 - Uniformity
 - Ghosting
 - MR Relaxometry
 
 Some example outputs from hazen:
 
-| hazen snr                        | hazen ghosting                |
+| hazen acr_ghosting                        | hazen ghosting                |
 |----------------------------------|-------------------------------|
 | ![](docs/assets/SNR.png) | ![](docs/assets/ghosting.png) |
 
 ---
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hazen Version: 1.1.3 Summary: An automatic MRI QA
+Metadata-Version: 2.1 Name: hazen Version: 1.2.0 Summary: An automatic MRI QA
 tool Home-page: https://bitbucket.org/gsttmri/hazen Author: Shuaib, Haris
 Author-email: mohammad_haris.shuaib@kcl.ac.uk Requires-Python: <3.11
 Description-Content-Type: text/markdown License-File: LICENSE.txt
                                [Ibn Al-Haytham]
                               ****** hazen ******
           Quality assurance framework for Magnetic Resonance Imaging
                              Explore_the_docs_Â»
@@ -14,29 +14,29 @@
                     raw/hazen_pytest-coverage-comment.json]
      Please STAR this repo to receive updates about new versions of hazen!
 --- ## Overview hazen is a software framework for performing automated analysis
 of magnetic resonance imaging (MRI) Quality Assurance data. It provides
 automatic quantitative analysis for the following measurements of MRI phantom
 data: - Signal-to-noise ratio (SNR) - Spatial resolution - Slice position and
 width - Uniformity - Ghosting - MR Relaxometry Some example outputs from hazen:
-| hazen snr | hazen ghosting | |----------------------------------|------------
--------------------| | ![](docs/assets/SNR.png) | ![](docs/assets/ghosting.png)
-| --- ## Installation ### pip Hazen can be installed using pip on python 3.9 or
-higher, it is recommended to use a virtual environment ```bash python3 -m venv
-hazen-venv source hazen-venv/bin/activate pip install hazen ``` #### Docker The
-Docker version of hazen as it is easy to get up-and-running and is linked to
-the most stable release. Refer to the [Docker installation instructions](https:
-//docs.docker.com/engine/install) to install Docker on your host computer. For
-ease of use, it is recommended to copy the `hazen-app` script to a location
-accessible on the path such as `/usr/local/bin`. This will allow you to run
-hazen from any location on your computer. Then, to use Docker hazen, simply run
-the `hazen-app` script appended with the function you want to use (e.g.:
-`snr`). In Terminal: ```bash cd hazen cp ./hazen-app /usr/local/bin # run hazen
-with CLI arguments hazen-app snr tests/data/snr/Siemens/ latest: Pulling from
-gsttmriphysics/hazen Digest: sha256:
+| hazen acr_ghosting | hazen ghosting | |----------------------------------|---
+----------------------------| | ![](docs/assets/SNR.png) | ![](docs/assets/
+ghosting.png) | --- ## Installation ### pip Hazen can be installed using pip on
+python 3.9 or higher, it is recommended to use a virtual environment ```bash
+python3 -m venv hazen-venv source hazen-venv/bin/activate pip install hazen ```
+#### Docker The Docker version of hazen as it is easy to get up-and-running and
+is linked to the most stable release. Refer to the [Docker installation
+instructions](https://docs.docker.com/engine/install) to install Docker on your
+host computer. For ease of use, it is recommended to copy the `hazen-app`
+script to a location accessible on the path such as `/usr/local/bin`. This will
+allow you to run hazen from any location on your computer. Then, to use Docker
+hazen, simply run the `hazen-app` script appended with the function you want to
+use (e.g.: `snr`). In Terminal: ```bash cd hazen cp ./hazen-app /usr/local/bin
+# run hazen with CLI arguments hazen-app snr tests/data/snr/Siemens/ latest:
+Pulling from gsttmriphysics/hazen Digest: sha256:
 18603e40b45f3af4bf45f07559a08a7833af92a6efe21cb7306f758e8eeab24a Status: Image
 is up to date for gsttmriphysics/hazen:latest docker.io/gsttmriphysics/hazen:
 latest
 { 'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
 191.16,
 'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
 195.58,
```

### Comparing `hazen-1.1.3/README.md` & `hazen-1.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 - Slice position and width
 - Uniformity
 - Ghosting
 - MR Relaxometry
 
 Some example outputs from hazen:
 
-| hazen snr                        | hazen ghosting                |
+| hazen acr_ghosting                        | hazen ghosting                |
 |----------------------------------|-------------------------------|
 | ![](docs/assets/SNR.png) | ![](docs/assets/ghosting.png) |
 
 ---
 
 ## Installation
```

#### html2text {}

```diff
@@ -11,29 +11,29 @@
                     raw/hazen_pytest-coverage-comment.json]
      Please STAR this repo to receive updates about new versions of hazen!
 --- ## Overview hazen is a software framework for performing automated analysis
 of magnetic resonance imaging (MRI) Quality Assurance data. It provides
 automatic quantitative analysis for the following measurements of MRI phantom
 data: - Signal-to-noise ratio (SNR) - Spatial resolution - Slice position and
 width - Uniformity - Ghosting - MR Relaxometry Some example outputs from hazen:
-| hazen snr | hazen ghosting | |----------------------------------|------------
--------------------| | ![](docs/assets/SNR.png) | ![](docs/assets/ghosting.png)
-| --- ## Installation ### pip Hazen can be installed using pip on python 3.9 or
-higher, it is recommended to use a virtual environment ```bash python3 -m venv
-hazen-venv source hazen-venv/bin/activate pip install hazen ``` #### Docker The
-Docker version of hazen as it is easy to get up-and-running and is linked to
-the most stable release. Refer to the [Docker installation instructions](https:
-//docs.docker.com/engine/install) to install Docker on your host computer. For
-ease of use, it is recommended to copy the `hazen-app` script to a location
-accessible on the path such as `/usr/local/bin`. This will allow you to run
-hazen from any location on your computer. Then, to use Docker hazen, simply run
-the `hazen-app` script appended with the function you want to use (e.g.:
-`snr`). In Terminal: ```bash cd hazen cp ./hazen-app /usr/local/bin # run hazen
-with CLI arguments hazen-app snr tests/data/snr/Siemens/ latest: Pulling from
-gsttmriphysics/hazen Digest: sha256:
+| hazen acr_ghosting | hazen ghosting | |----------------------------------|---
+----------------------------| | ![](docs/assets/SNR.png) | ![](docs/assets/
+ghosting.png) | --- ## Installation ### pip Hazen can be installed using pip on
+python 3.9 or higher, it is recommended to use a virtual environment ```bash
+python3 -m venv hazen-venv source hazen-venv/bin/activate pip install hazen ```
+#### Docker The Docker version of hazen as it is easy to get up-and-running and
+is linked to the most stable release. Refer to the [Docker installation
+instructions](https://docs.docker.com/engine/install) to install Docker on your
+host computer. For ease of use, it is recommended to copy the `hazen-app`
+script to a location accessible on the path such as `/usr/local/bin`. This will
+allow you to run hazen from any location on your computer. Then, to use Docker
+hazen, simply run the `hazen-app` script appended with the function you want to
+use (e.g.: `snr`). In Terminal: ```bash cd hazen cp ./hazen-app /usr/local/bin
+# run hazen with CLI arguments hazen-app snr tests/data/snr/Siemens/ latest:
+Pulling from gsttmriphysics/hazen Digest: sha256:
 18603e40b45f3af4bf45f07559a08a7833af92a6efe21cb7306f758e8eeab24a Status: Image
 is up to date for gsttmriphysics/hazen:latest docker.io/gsttmriphysics/hazen:
 latest
 { 'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
 191.16,
 'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
 195.58,
```

### Comparing `hazen-1.1.3/hazen.egg-info/PKG-INFO` & `hazen-1.2.0/hazen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hazen
-Version: 1.1.3
+Version: 1.2.0
 Summary: An automatic MRI QA tool
 Home-page: https://bitbucket.org/gsttmri/hazen
 Author: Shuaib, Haris
 Author-email: mohammad_haris.shuaib@kcl.ac.uk
 Requires-Python: <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -45,15 +45,15 @@
 - Slice position and width
 - Uniformity
 - Ghosting
 - MR Relaxometry
 
 Some example outputs from hazen:
 
-| hazen snr                        | hazen ghosting                |
+| hazen acr_ghosting                        | hazen ghosting                |
 |----------------------------------|-------------------------------|
 | ![](docs/assets/SNR.png) | ![](docs/assets/ghosting.png) |
 
 ---
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hazen Version: 1.1.3 Summary: An automatic MRI QA
+Metadata-Version: 2.1 Name: hazen Version: 1.2.0 Summary: An automatic MRI QA
 tool Home-page: https://bitbucket.org/gsttmri/hazen Author: Shuaib, Haris
 Author-email: mohammad_haris.shuaib@kcl.ac.uk Requires-Python: <3.11
 Description-Content-Type: text/markdown License-File: LICENSE.txt
                                [Ibn Al-Haytham]
                               ****** hazen ******
           Quality assurance framework for Magnetic Resonance Imaging
                              Explore_the_docs_Â»
@@ -14,29 +14,29 @@
                     raw/hazen_pytest-coverage-comment.json]
      Please STAR this repo to receive updates about new versions of hazen!
 --- ## Overview hazen is a software framework for performing automated analysis
 of magnetic resonance imaging (MRI) Quality Assurance data. It provides
 automatic quantitative analysis for the following measurements of MRI phantom
 data: - Signal-to-noise ratio (SNR) - Spatial resolution - Slice position and
 width - Uniformity - Ghosting - MR Relaxometry Some example outputs from hazen:
-| hazen snr | hazen ghosting | |----------------------------------|------------
--------------------| | ![](docs/assets/SNR.png) | ![](docs/assets/ghosting.png)
-| --- ## Installation ### pip Hazen can be installed using pip on python 3.9 or
-higher, it is recommended to use a virtual environment ```bash python3 -m venv
-hazen-venv source hazen-venv/bin/activate pip install hazen ``` #### Docker The
-Docker version of hazen as it is easy to get up-and-running and is linked to
-the most stable release. Refer to the [Docker installation instructions](https:
-//docs.docker.com/engine/install) to install Docker on your host computer. For
-ease of use, it is recommended to copy the `hazen-app` script to a location
-accessible on the path such as `/usr/local/bin`. This will allow you to run
-hazen from any location on your computer. Then, to use Docker hazen, simply run
-the `hazen-app` script appended with the function you want to use (e.g.:
-`snr`). In Terminal: ```bash cd hazen cp ./hazen-app /usr/local/bin # run hazen
-with CLI arguments hazen-app snr tests/data/snr/Siemens/ latest: Pulling from
-gsttmriphysics/hazen Digest: sha256:
+| hazen acr_ghosting | hazen ghosting | |----------------------------------|---
+----------------------------| | ![](docs/assets/SNR.png) | ![](docs/assets/
+ghosting.png) | --- ## Installation ### pip Hazen can be installed using pip on
+python 3.9 or higher, it is recommended to use a virtual environment ```bash
+python3 -m venv hazen-venv source hazen-venv/bin/activate pip install hazen ```
+#### Docker The Docker version of hazen as it is easy to get up-and-running and
+is linked to the most stable release. Refer to the [Docker installation
+instructions](https://docs.docker.com/engine/install) to install Docker on your
+host computer. For ease of use, it is recommended to copy the `hazen-app`
+script to a location accessible on the path such as `/usr/local/bin`. This will
+allow you to run hazen from any location on your computer. Then, to use Docker
+hazen, simply run the `hazen-app` script appended with the function you want to
+use (e.g.: `snr`). In Terminal: ```bash cd hazen cp ./hazen-app /usr/local/bin
+# run hazen with CLI arguments hazen-app snr tests/data/snr/Siemens/ latest:
+Pulling from gsttmriphysics/hazen Digest: sha256:
 18603e40b45f3af4bf45f07559a08a7833af92a6efe21cb7306f758e8eeab24a Status: Image
 is up to date for gsttmriphysics/hazen:latest docker.io/gsttmriphysics/hazen:
 latest
 { 'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
 191.16,
 'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
 195.58,
```

### Comparing `hazen-1.1.3/hazen.egg-info/SOURCES.txt` & `hazen-1.2.0/hazen.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,29 +21,33 @@
 hazenlib/data/relaxometry/Plate4_T2
 hazenlib/data/relaxometry/Plate5_T1_signed
 hazenlib/data/relaxometry/Plate5_T2
 hazenlib/tasks/__init__.py
 hazenlib/tasks/acr_geometric_accuracy.py
 hazenlib/tasks/acr_ghosting.py
 hazenlib/tasks/acr_slice_position.py
+hazenlib/tasks/acr_slice_thickness.py
 hazenlib/tasks/acr_snr.py
+hazenlib/tasks/acr_spatial_resolution.py
 hazenlib/tasks/acr_uniformity.py
 hazenlib/tasks/ghosting.py
 hazenlib/tasks/relaxometry.py
 hazenlib/tasks/slice_position.py
 hazenlib/tasks/slice_width.py
 hazenlib/tasks/snr.py
 hazenlib/tasks/snr_map.py
 hazenlib/tasks/spatial_resolution.py
 hazenlib/tasks/uniformity.py
 tests/__init__.py
 tests/test_acr_geometric_accuracy.py
 tests/test_acr_ghosting.py
 tests/test_acr_slice_position.py
+tests/test_acr_slice_thickness.py
 tests/test_acr_snr.py
+tests/test_acr_spatial_resolution.py
 tests/test_acr_uniformity.py
 tests/test_ghosting.py
 tests/test_hazenlib.py
 tests/test_relaxometry.py
 tests/test_slice_position.py
 tests/test_slice_width.py
 tests/test_snr.py
```

### Comparing `hazen-1.1.3/hazenlib/HazenTask.py` & `hazen-1.2.0/hazenlib/HazenTask.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/__init__.py` & `hazen-1.2.0/hazenlib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     hazen --version
 Options:
 Report is an optional argument needed if you want to get a plot of your results.
 'Calc_t1', 'calc_t', 'plate_number=<n>', 'show_template_fit', 'show_relax_fits', 'show_rois', 'verbose' are optional arguments for the relaxometry function.
 'Measured_slice_width' is an optional argument for the SNR function.
 'Log' is an optional argument that allows users to set the severity of the logs.
     <task>    snr | slice_position | slice_width | spatial_resolution | uniformity | ghosting | relaxometry | snr_map |
-    acr_ghosting | acr_uniformity |
+    acr_ghosting | acr_uniformity | acr_spatial_resolution | acr_slice_thickness | acr_snr | acr_slice_position | acr_geometric_accuracy
     <folder>
     --report
 
 """
 import importlib
 import inspect
 import logging
```

### Comparing `hazen-1.1.3/hazenlib/data/relaxometry/Plate4_T1_signed` & `hazen-1.2.0/hazenlib/data/relaxometry/Plate4_T1_signed`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/data/relaxometry/Plate4_T2` & `hazen-1.2.0/hazenlib/data/relaxometry/Plate4_T2`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/data/relaxometry/Plate5_T1_signed` & `hazen-1.2.0/hazenlib/data/relaxometry/Plate5_T1_signed`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/data/relaxometry/Plate5_T2` & `hazen-1.2.0/hazenlib/data/relaxometry/Plate5_T2`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/exceptions.py` & `hazen-1.2.0/hazenlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/logger.py` & `hazen-1.2.0/hazenlib/logger.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/relaxometry.py` & `hazen-1.2.0/hazenlib/relaxometry.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/shapes.py` & `hazen-1.2.0/hazenlib/shapes.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/tasks/acr_geometric_accuracy.py` & `hazen-1.2.0/hazenlib/tasks/acr_geometric_accuracy.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/tasks/acr_ghosting.py` & `hazen-1.2.0/hazenlib/tasks/acr_ghosting.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/tasks/acr_slice_position.py` & `hazen-1.2.0/hazenlib/tasks/acr_slice_position.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         mean_y_profile = np.mean(invest_y, 1)  # mean of vertical projections of phantom
         abs_diff_y_profile = np.abs(np.diff(mean_y_profile))  # absolute first derivative of mean
 
         y_peaks = find_n_peaks(abs_diff_y_profile, 2)  # find two highest peaks
         y_locs = w_point + y_peaks - 1  # y coordinates of these peaks in image coordinate system(before diff operation)
 
         if y_locs[1] - y_locs[0] < 5 / res[1]:
-            y = n_point + round(10 / res[1])  # if peaks too close together, use phantom geometry
+            y = [n_point + round(10 / res[1])]  # if peaks too close together, use phantom geometry
         else:
             y = np.round(np.min(y_locs) + 0.25 * np.abs(np.diff(y_locs)))  # define y coordinate
 
         dist_to_y = np.abs(n_point - y[0]) * res[1]  # distance to y from top of phantom
         y_pts = np.append(y, np.round(y[0] + (47 - dist_to_y) / res[1])).astype(int)  # place 2nd y point 47mm from top of phantom
 
         return x_pts, y_pts
@@ -188,27 +188,25 @@
         # take line profiles in range of interest
         static_line_L = interp_line_prof_L[peaks[0]:peaks[1]]
         static_line_R = interp_line_prof_R[peaks[0]:peaks[1]]
 
         lag = np.linspace(-50, 50, 101, dtype=int)  # create array of lag values
         err = np.zeros(len(lag))  # initialise array of errors
 
-        for k in range(len(lag)):
-            temp_lag = lag[k]  # set a shift value
-            difference = static_line_R - np.roll(static_line_L, temp_lag)  # difference of L and circularly shifted R
+        for k, lag_val in enumerate(lag):
+            difference = static_line_R - np.roll(static_line_L, lag_val)  # difference of L and circularly shifted R
             # set wrapped values to nan
-            if temp_lag > 0:
-                difference[:temp_lag] = np.nan
+            if lag_val > 0:
+                difference[:lag_val] = np.nan
             else:
-                difference[temp_lag:] = np.nan
+                difference[lag_val:] = np.nan
 
-            if np.isnan(difference).all():
-                err[k] = 1e10  # filler value to suppress warning when trying to calculate mean of array filled with NaN
-            else:
-                err[k] = np.nanmean(difference)  # calculate mean difference ignoring nan values
+            # filler value to suppress warning when trying to calculate mean of array filled with NaN otherwise
+            # calculate difference
+            err[k] = 1e10 if np.isnan(difference).all() else np.nanmean(difference)
 
         temp = np.argwhere(err == np.min(err[err > 0]))[0]  # find minimum non-zero error
         shift = -lag[temp][0] if pos == 1 else lag[temp][0]  # find shift corresponding to above error
 
         dL = np.round(pos * np.abs(shift) * (1 / interp_factor) * res[1], 2)  # calculate bar length difference
 
         if self.report:
```

### Comparing `hazen-1.1.3/hazenlib/tasks/acr_snr.py` & `hazen-1.2.0/hazenlib/tasks/acr_snr.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/tasks/acr_uniformity.py` & `hazen-1.2.0/hazenlib/tasks/acr_uniformity.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/tasks/ghosting.py` & `hazen-1.2.0/hazenlib/tasks/ghosting.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/tasks/slice_position.py` & `hazen-1.2.0/hazenlib/tasks/slice_position.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/tasks/slice_width.py` & `hazen-1.2.0/hazenlib/tasks/slice_width.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/tasks/snr.py` & `hazen-1.2.0/hazenlib/tasks/snr.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/tasks/snr_map.py` & `hazen-1.2.0/hazenlib/tasks/snr_map.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/tasks/spatial_resolution.py` & `hazen-1.2.0/hazenlib/tasks/spatial_resolution.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/hazenlib/tasks/uniformity.py` & `hazen-1.2.0/hazenlib/tasks/uniformity.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     def run(self) -> dict:
         results = {}
 
         for dcm in self.data:
             try:
                 result = self.get_fractional_uniformity(dcm)
             except Exception as e:
-                print(f"Could not calculate the uniformity for {self.key(dcm)} because of : {e}")
+                print(f"Could test not calculate the uniformity for {self.key(dcm)} because of : {e}")
                 traceback.print_exc(file=sys.stdout)
                 continue
 
             results[self.key(dcm)] = result
 
         results['reports'] = {'images': self.report_files}
```

### Comparing `hazen-1.1.3/hazenlib/tools.py` & `hazen-1.2.0/hazenlib/tools.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/setup.cfg` & `hazen-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/tests/test_acr_geometric_accuracy.py` & `hazen-1.2.0/tests/test_acr_geometric_accuracy.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,19 +24,28 @@
     def test_object_centre(self):
         data = self.dcm.pixel_array
         assert self.acr_geometric_accuracy_task.centroid_com(data)[1] == self.centre
 
     def test_geo_accuracy_slice1(self):
         slice1_vals = np.array(self.acr_geometric_accuracy_task.get_geometric_accuracy_slice1(self.dcm))
         slice1_vals = np.round(slice1_vals, 2)
+
+        print("\ntest_geo_accuracy.py::TestGeoAccuracy::test_geo_accuracy_slice1")
+        print("new_release:", slice1_vals)
+        print("fixed value:", self.L1)
+
         assert (slice1_vals == self.L1).all() == True
 
     def test_geo_accuracy_slice5(self):
         slice5_vals = np.array(self.acr_geometric_accuracy_task.get_geometric_accuracy_slice5(self.dcm2))
         slice5_vals = np.round(slice5_vals, 2)
+
+        print("\ntest_geo_accuracy.py::TestGeoAccuracy::test_geo_accuracy_slice1")
+        print("new_release:", slice5_vals)
+        print("fixed value:", self.L5)
         assert (slice5_vals == self.L5).all() == True
 
     def test_rotate_point(self):
         rotated_point = np.array(self.acr_geometric_accuracy_task.rotate_point((0, 0), (30, 70), 150))
         rotated_point = np.round(rotated_point, 2)
         print(rotated_point)
         assert (rotated_point == self.test_point).all() == True
```

### Comparing `hazen-1.1.3/tests/test_acr_ghosting.py` & `hazen-1.2.0/tests/test_acr_ghosting.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,15 +17,21 @@
                                              report_dir=pathlib.PurePath.joinpath(TEST_REPORT_DIR))
         self.dcm = pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens', '6.dcm'))
 
     def test_object_centre(self):
         assert self.acr_ghosting_task.centroid_com(self.dcm.pixel_array)[1] == self.centre
 
     def test_ghosting(self):
-        assert round(self.acr_ghosting_task.get_signal_ghosting(self.dcm), 3) == self.psg
+        ghosting_val = round(self.acr_ghosting_task.get_signal_ghosting(self.dcm), 3)
+
+        print("\ntest_ghosting.py::TestGhosting::test_ghosting")
+        print("new_release_value:", ghosting_val)
+        print("fixed_value:", self.psg)
+
+        assert ghosting_val == self.psg
 
 
 class TestACRGhostingGE(unittest.TestCase):
     ACR_GHOSTING_DATA = pathlib.Path(TEST_DATA_DIR / 'acr')
     centre = [253, 256]
     psg = 0.487
```

### Comparing `hazen-1.1.3/tests/test_acr_slice_position.py` & `hazen-1.2.0/tests/test_acr_slice_position.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,16 +38,23 @@
         assert (self.acr_slice_position_task.find_wedges(self.dcm_11.pixel_array, mask, res)[0] ==
                 self.x_pts[1]).all() == True
 
         assert (self.acr_slice_position_task.find_wedges(self.dcm_11.pixel_array, mask, res)[1] ==
                 self.y_pts[1]).all() == True
 
     def test_slice_position(self):
-        assert round(self.acr_slice_position_task.get_slice_position(self.dcm_1), 2) == self.dL[0]
-        assert round(self.acr_slice_position_task.get_slice_position(self.dcm_11), 2) == self.dL[1]
+        slice_position_val_1 = round(self.acr_slice_position_task.get_slice_position(self.dcm_1), 2)
+        slice_position_val_11 = round(self.acr_slice_position_task.get_slice_position(self.dcm_11), 2)
+
+        print("\ntest_slice_position.py::TestSlicePosition::test_slice_position")
+        print("new_release_value:", slice_position_val_1)
+        print("fixed_value:", self.dL[0])
+
+        assert slice_position_val_1 == self.dL[0]
+        assert slice_position_val_11 == self.dL[1]
 
 
 class TestACRSlicePositionGE(unittest.TestCase):
     ACR_SLICE_POSITION_DATA = pathlib.Path(TEST_DATA_DIR / 'acr')
     centre = [253, 257]
     x_pts = [(246, 257), (246, 257)]
     y_pts = [(82, 163), (85, 165)]
```

### Comparing `hazen-1.1.3/tests/test_acr_snr.py` & `hazen-1.2.0/tests/test_acr_snr.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,21 @@
 
     def test_snr_by_smoothing(self):
         snr, _ = self.acr_snr_task.snr_by_smoothing(self.dcm)
         assert round(snr, 2) == self.snr
 
     def test_snr_by_subtraction(self):
         snr, _ = self.acr_snr_task.snr_by_subtraction(self.dcm, self.dcm2)
-        assert round(snr, 2) == self.sub_snr
+        rounded_snr = round(snr, 2)
+
+        print("\ntest_snr_by_subtraction.py::TestSnrBySubtraction::test_snr_by_subtraction")
+        print("new_release_value:", rounded_snr)
+        print("fixed_value:", self.sub_snr)
+
+        assert rounded_snr == self.sub_snr
 
 
 class TestACRSNRGE(unittest.TestCase):
     ACR_SNR_DATA = pathlib.Path(TEST_DATA_DIR / 'acr')
     centre = [253, 256]
     norm_factor = 57.12810400630368
     snr = 39.97
```

### Comparing `hazen-1.1.3/tests/test_acr_uniformity.py` & `hazen-1.2.0/tests/test_acr_uniformity.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,21 @@
 
     def test_circular_mask(self):
         test_circle = self.acr_uniformity_task.circular_mask([128, 128], 1, [256, 256]).astype(int)
         assert (self.array == test_circle).all() == True
 
     def test_uniformity(self):
         results = self.acr_uniformity_task.get_integral_uniformity(self.dcm)
-        assert round(results, 2) == self.piu
+        rounded_results = round(results, 2)
+
+        print("\ntest_uniformity.py::TestUniformity::test_uniformity")
+        print("new_release_values:", rounded_results)
+        print("fixed_values:", self.piu)
+
+        assert rounded_results == self.piu
 
 
 # class TestACRUniformityPhilips(unittest.TestCase):
 #
 class TestACRUniformityGE(unittest.TestCase):
     ACR_UNIFORMITY_DATA = pathlib.Path(TEST_DATA_DIR / 'acr')
     centre = [253, 256]
```

### Comparing `hazen-1.1.3/tests/test_ghosting.py` & `hazen-1.2.0/tests/test_ghosting.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,15 +69,21 @@
         assert self.ghosting.get_eligible_area(self.SIGNAL_BOUNDING_BOX, self.dcm) == self.ELIGIBLE_GHOST_AREA
 
     def test_get_ghost_slice(self):
         assert list(self.ghosting.get_ghost_slice(self.SIGNAL_BOUNDING_BOX, self.dcm)[0]) == list(self.GHOST_SLICE[0])
         assert list(self.ghosting.get_ghost_slice(self.SIGNAL_BOUNDING_BOX, self.dcm)[1]) == list(self.GHOST_SLICE[1])
 
     def test_get_ghosting(self):
-        assert self.ghosting.get_ghosting(self.dcm) == self.GHOSTING
+        ghosting_val = self.ghosting.get_ghosting(self.dcm)
+
+        print("\ntest_get_ghosting.py::TestGetGhosting::test_get_ghosting")
+        print("new_release_value:", ghosting_val)
+        print("fixed_value:", self.GHOSTING)
+
+        assert ghosting_val == self.GHOSTING
 
 
 class TestCOLPEGhosting(TestGhosting):
     SIGNAL_BOUNDING_BOX = (164, 208, 166, 209)
     SIGNAL_CENTRE = [186, 187]
     BACKGROUND_ROIS = [(64, 187), (64, 140), (64, 93), (64, 46)]
     PADDING_FROM_BOX = 30
```

### Comparing `hazen-1.1.3/tests/test_hazenlib.py` & `hazen-1.2.0/tests/test_hazenlib.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,17 +160,16 @@
     maxDiff = None
 
     def setUp(self):
         self.file = str(TEST_DATA_DIR / 'resolution' / 'philips' / 'IM-0004-0002.dcm')
         self.dcm = pydicom.read_file(self.file)
 
     def test1_logger(self):
-        sys.argv = ["hazen", "spatial_resolution", ".\\tests\\data\\resolution\\RESOLUTION\\", "--log", "warning"]
-
-        sys.argv = [item.replace("\\", "/") for item in sys.argv]
+        path = str(TEST_DATA_DIR / 'resolution' / 'RESOLUTION')
+        sys.argv = ["hazen", "spatial_resolution", path, "--log", "warning"]
 
         hazenlib.main()
 
         logging = hazenlib.logging
 
         self.assertEqual(logging.root.level, logging.WARNING)
 
@@ -203,18 +202,16 @@
                  'snr_smoothing_normalised_SNR_SNR_SAG_MEAS2_24_1': 7591.33,
                  'snr_smoothing_measured_SNR_SNR_SAG_MEAS1_23_1': 179.94,
                  'snr_smoothing_normalised_SNR_SNR_SAG_MEAS1_23_1': 7426.54}
 
         self.assertDictEqual(output_dict['SNR_SNR_SAG_MEAS1_23_1'], dict1)
 
     def test_relaxometry(self):
-        sys.argv = ["hazen", "relaxometry", ".\\tests\\data\\relaxometry\\T1\\site3_ge\\plate4\\", "--plate_number",
-                    "4", "--calc_t1"]
-
-        sys.argv = [item.replace("\\", "/") for item in sys.argv]
+        path = str(TEST_DATA_DIR / 'relaxometry' / 'T1' / 'site3_ge' / 'plate4')
+        sys.argv = ["hazen", "relaxometry", path, "--plate_number", "4", "--calc_t1"]
 
         output = hazenlib.main()
         output_dict = ast.literal_eval(output)
 
         dict1 = {'Spin Echo_32_2_P4_t1': {'rms_frac_time_difference': 0.13499936644959437}}
         self.assertAlmostEqual(dict1['Spin Echo_32_2_P4_t1']['rms_frac_time_difference'],
                                output_dict['Spin Echo_32_2_P4_t1']['rms_frac_time_difference'], 4)
```

### Comparing `hazen-1.1.3/tests/test_relaxometry.py` & `hazen-1.2.0/tests/test_relaxometry.py`

 * *Files identical despite different names*

### Comparing `hazen-1.1.3/tests/test_slice_position.py` & `hazen-1.2.0/tests/test_slice_position.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,17 +41,22 @@
         # plt.scatter([lx, rx], [ly, ry], 3, c='green')
         # plt.savefig('test_get_rods_coords.png')
 
         assert (lx, ly, rx, ry) == self.ROD_COORDS
 
     def test_slice_position(self):
         results = self.hazen_slice_position.run()
+        key = self.hazen_slice_position.key(self.hazen_slice_position.data[0])
+        slice_positions = results[key]['slice_positions']
 
-        assert results[self.hazen_slice_position.key(self.hazen_slice_position.data[0])][
-                   'slice_positions'] == self.SLICE_POSITION_OUTPUT
+        print("\ntest_slice_position.py::TestSlicePosition::test_slice_position")
+        print("new_release_value:", slice_positions)
+        print("fixed_value", self.SLICE_POSITION_OUTPUT)
+
+        assert slice_positions == self.SLICE_POSITION_OUTPUT
 
 
 # now test on canon data
 class CanonTestSlicePosition(TestSlicePosition):
     SLICE_POS = pathlib.Path(TEST_DATA_DIR / 'slicepos')
     ROD_COORDS = (123.0, 77.5, 130.88888888888889, 171.66666666666666)
     SLICE_POSITION_OUTPUT = ['1.49', '1.35', '1.29', '1.12', '0.928', '0.885', '0.729', '0.557', '0.531', '0.635',
```

### Comparing `hazen-1.1.3/tests/test_slice_width.py` & `hazen-1.2.0/tests/test_slice_width.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,20 +232,22 @@
             assert abs(value - matlab_trapezoid_fit_coefficients[idx]) <= 5
 
         for idx, value in enumerate(matlab_baseline_fit_coefficients):
             assert abs(value - matlab_baseline_fit_coefficients[idx]) <= 5
 
     def test_slice_width(self):
         results = self.slice_width.run()
-        self.slice_width.key(self.slice_width.data[0])
-        # key = f"{self.slice_width.data[0].SeriesDescription}_{self.slice_width.data[0].SeriesNumber}_{self.slice_width.data[0].InstanceNumber}"
-        # print("slice width")
-        # print(results[key]['slice_width_mm'])
-        # assert abs(results[key]['slice_width_mm'] - self.SW_MATLAB) < 0.1
-        assert abs(results[self.slice_width.key(self.slice_width.data[0])]['slice_width_mm'] - self.SW_MATLAB) < 0.1
+        key = self.slice_width.key(self.slice_width.data[0])
+        slice_width_mm = results[key]['slice_width_mm']
+
+        print("\ntest_slice_width.py::TestSliceWidth::test_slice_width")
+        print("new_release_value:", slice_width_mm)
+        print("fixed_value:", self.SW_MATLAB)
+
+        assert abs(slice_width_mm - self.SW_MATLAB) < 0.1
 
 
 class Test512Matrix(TestSliceWidth):
     SLICE_WIDTH_DATA = pathlib.Path(TEST_DATA_DIR / 'slicewidth')
 
     """
     Notes
```

### Comparing `hazen-1.1.3/tests/test_snr.py` & `hazen-1.2.0/tests/test_snr.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,11 +146,14 @@
                        report_dir=pathlib.PurePath.joinpath(TEST_REPORT_DIR))
 
     def test_get_object_centre(self):
         assert self.snr.get_object_centre(self.snr.data[0]) == self.OBJECT_CENTRE
 
     def test_image_snr(self):
         val = self.snr.run()
+        print("\ntest_snr.py::TestSnrThreshold::test_image_snr")
+        print("set values:", val)
+        print("new_release_values", self.snr.run())
         self.assertTrue(self.LOWER_SMOOTHED_SNR <= val[self.snr.key(self.snr.data[0])][
             f"snr_smoothing_normalised_{self.snr.key(self.snr.data[0])}"] <= self.UPPER_SMOOTHED_SNR)
         self.assertTrue(self.LOWER_SUBTRACT_SNR <= val[self.snr.key(self.snr.data[0])][
             f"snr_subtraction_normalised_{self.snr.key(self.snr.data[0])}"] <= self.UPPER_SUBTRACT_SNR)
```

### Comparing `hazen-1.1.3/tests/test_snr_map.py` & `hazen-1.2.0/tests/test_snr_map.py`

 * *Files 21% similar despite different names*

```diff
@@ -45,16 +45,21 @@
         assert self.snr_map.mask.sum() == 29444
 
     def test_calc_snr(self):
         np.testing.assert_approx_equal(
             self.snr_map.snr, 192.8818801790859)
 
     def test_calc_snr_map(self):
-        np.testing.assert_almost_equal(
-            self.snr_map.snr_map.cumsum().sum(), 128077116718.40483)
+        snr_map_cumsum = self.snr_map.snr_map.cumsum().sum()
+
+        print("\ntest_calc_snr_map.py::TestCalcSnrMap::test_calc_snr_map")
+        print("new_release_value:", snr_map_cumsum)
+        print("fixed_value:", 128077116718.40483)
+
+        np.testing.assert_almost_equal(snr_map_cumsum, 128077116718.40483)
 
     def test_plot_detailed(self):
         # Just check a valid figure handle is returned
         fig = self.snr_map.plot_detailed()
         assert isinstance(fig, matplotlib.figure.Figure)
 
     def test_plot_summary(self):
```

### Comparing `hazen-1.1.3/tests/test_spatial_resolution.py` & `hazen-1.2.0/tests/test_spatial_resolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,17 +411,24 @@
         assert a == b
 
     def test_mtf(self):
         assert self.mtf[0] == abs(np.fft.fft(self.lsf))[0]
 
     def test_calculate_mtf(self):
         res = self.hazen_spatial_resolution.calculate_mtf(self.hazen_spatial_resolution.data[0])
-        assert res['frequency_encoding_direction'] == pytest.approx(self.MTF_FE)
-        assert res['phase_encoding_direction'] == pytest.approx(self.MTF_PE)
+        fe_res = res['frequency_encoding_direction']
+        pe_res = res['phase_encoding_direction']
 
+        print("\ntest_calculate_mtf.py::TestCalculateMtf::test_calculate_mtf")
+        print("new_release_value:", fe_res)
+        print("fixed_value:", self.MTF_FE)
+
+
+        assert fe_res == pytest.approx(self.MTF_FE)
+        assert pe_res == pytest.approx(self.MTF_PE)
 
 class TestPhilipsResolution(TestSpatialResolution):
     RESOLUTION_DATA = pathlib.Path(TEST_DATA_DIR / 'resolution')
     # dicom = pydicom.read_file(str(RESOLUTION_DATA / 'philips' / "IM-0004-0002.dcm"))
     files = get_dicom_files(os.path.join(TEST_DATA_DIR, 'resolution', 'philips'))
     TEST_SQUARE = [[293, 203], [215, 218], [230, 297], [308, 282]]
     CIRCLE = [[[257, 245, 199]]]
```

### Comparing `hazen-1.1.3/tests/test_tools.py` & `hazen-1.2.0/tests/test_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,9 +106,7 @@
     def test_is_dicom_no(self):
         result = hazen_tools.is_dicom_file(self.false_dicom_path)
         self.assertFalse(result)
 
 
 if __name__ == "__main__":
     unittest.main()
-
-
```

### Comparing `hazen-1.1.3/tests/test_uniformity.py` & `hazen-1.2.0/tests/test_uniformity.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,18 +13,26 @@
 
     def setUp(self):
         self.uniformity_task = Uniformity(data_paths=[os.path.join(self.UNIFORMITY_DATA, 'axial_oil.IMA')],
                                           report_dir=pathlib.PurePath.joinpath(TEST_REPORT_DIR))
 
     def test_uniformity(self):
         results = self.uniformity_task.run()
-        assert results[self.uniformity_task.key(self.uniformity_task.data[0])]['horizontal'][
-                   'IPEM'] == self.IPEM_HORIZONTAL
-        assert results[self.uniformity_task.key(self.uniformity_task.data[0])]['vertical']['IPEM'] == self.IPEM_VERTICAL
+        key = self.uniformity_task.key(self.uniformity_task.data[0])
+        horizontal_ipem = results[key]['horizontal']['IPEM']
+        vertical_ipem = results[key]['vertical']['IPEM']
 
+        print("\ntest_uniformity.py::TestUniformity::test_uniformity")
+
+        print("new_release_value:", vertical_ipem)
+
+        print("fixed_value:", self.IPEM_VERTICAL)
+
+        assert horizontal_ipem == self.IPEM_HORIZONTAL
+        assert vertical_ipem == self.IPEM_VERTICAL
 
 class TestSagUniformity(TestUniformity):
     IPEM_HORIZONTAL = 0.46875
     IPEM_VERTICAL = 0.5125
 
     def setUp(self):
         self.uniformity_task = Uniformity(data_paths=[os.path.join(self.UNIFORMITY_DATA, 'sag.dcm')],
```

