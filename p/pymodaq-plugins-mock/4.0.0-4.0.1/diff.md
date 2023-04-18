# Comparing `tmp/pymodaq_plugins_mock-4.0.0.tar.gz` & `tmp/pymodaq_plugins_mock-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_mock-4.0.0.tar", last modified: Mon Jan 30 14:26:15 2023, max compression
+gzip compressed data, was "pymodaq_plugins_mock-4.0.1.tar", last modified: Tue Apr 18 13:34:02 2023, max compression
```

## Comparing `pymodaq_plugins_mock-4.0.0.tar` & `pymodaq_plugins_mock-4.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:26:15.556288 pymodaq_plugins_mock-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-01-30 14:26:15.556288 pymodaq_plugins_mock-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 14:26:15.556288 pymodaq_plugins_mock-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:26:15.552288 pymodaq_plugins_mock-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:26:15.556288 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:26:15.556288 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:26:15.556288 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:26:15.556288 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:26:15.556288 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:26:15.556288 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:26:15.556288 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:26:15.556288 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/hardware/
--rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/hardware/camera_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/hardware/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:26:15.556288 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 14:26:03.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 14:26:15.556288 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-01-30 14:26:15.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-01-30 14:26:15.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 14:26:15.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-30 14:26:15.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-30 14:26:15.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-30 14:26:15.000000 pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.621826 pymodaq_plugins_mock-4.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.621826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/camera_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:33:52.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:34:02.625826 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-18 13:34:02.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-18 13:34:02.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:34:02.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 13:34:02.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 13:34:02.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 13:34:02.000000 pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_mock-4.0.0/LICENSE` & `pymodaq_plugins_mock-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.0/PKG-INFO` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pymodaq_plugins_mock
-Version: 4.0.0
+Name: pymodaq-plugins-mock
+Version: 4.0.1
 Summary: Set of base PyMoDAQ plugins including Mock ones for development
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_mock
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: CECILL B
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,15 +29,16 @@
    :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://github.com/PyMoDAQ/pymodaq_plugins/workflows/Upload%20Python%20Package/badge.svg
     :target: https://github.com/PyMoDAQ/pymodaq_plugins
 
 Plugins initially developed with PyMoDAQ. Includes Mock plugins that are plugins of virtual instruments dedicated
-to code testing for new functionalities or development.
+to code testing for new functionalities or development. From version 4.0.0 onwards, these plugins will only work with
+pymodaq > 4.0.0
 
 
 Authors
 =======
 
 * Sebastien J. Weber
```

### Comparing `pymodaq_plugins_mock-4.0.0/README.rst` & `pymodaq_plugins_mock-4.0.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,16 @@
    :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://github.com/PyMoDAQ/pymodaq_plugins/workflows/Upload%20Python%20Package/badge.svg
     :target: https://github.com/PyMoDAQ/pymodaq_plugins
 
 Plugins initially developed with PyMoDAQ. Includes Mock plugins that are plugins of virtual instruments dedicated
-to code testing for new functionalities or development.
+to code testing for new functionalities or development. From version 4.0.0 onwards, these plugins will only work with
+pymodaq > 4.0.0
 
 
 Authors
 =======
 
 * Sebastien J. Weber
```

### Comparing `pymodaq_plugins_mock-4.0.0/setup.py` & `pymodaq_plugins_mock-4.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_Mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, main  # base class
 from pymodaq.control_modules.move_utility_classes import comon_parameters_fun  # common set of parameters for all actuators
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo  # object used to send info back to the main thread
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo  # object used to send info back to the main thread
 from easydict import EasyDict as edict  # type of dict
 
 
 class DAQ_Move_Mock(DAQ_Move_base):
     """
         Wrapper object to access the Mock fonctionnalities, similar wrapper for all controllers.
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockCamera.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pymodaq.control_modules.move_utility_classes import DAQ_Move_base, main  # base class
 from pymodaq.control_modules.move_utility_classes import comon_parameters_fun  # common set of parameters for all actuators
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo  # object used to send info back to the main thread
-from easydict import EasyDict as edict  # type of dict
 
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo  # object used to send info back to the main thread
+from easydict import EasyDict as edict  # type of dict
 from pymodaq_plugins_mock.hardware.camera_wrapper import Camera
 
+
 class DAQ_Move_MockCamera(DAQ_Move_base):
     """
         Wrapper object to access the Mock fonctionnalities, similar wrapper for all controllers.
 
         =============== ==============
         **Attributes**    **Type**
         *params*          dictionnary
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_move_plugins/daq_move_MockTau.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_Mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from qtpy import QtWidgets
 
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, DataFromPlugins
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.data import DataFromPlugins
 import numpy as np
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, comon_parameters, main
 
-from pymodaq.daq_utils.math_utils import gauss1D
+from pymodaq.utils.math_utils import gauss1D
 
 
 class DAQ_0DViewer_Mock(DAQ_Viewer_base):
     params = comon_parameters + [
         {'title': 'Wait time (ms)', 'name': 'wait_time', 'type': 'int', 'value': 100, 'default': 100, 'min': 0},
         {'title': 'Separated viewers', 'name': 'sep_viewers', 'type': 'bool', 'value': False},
         {'title': 'Show in LCD', 'name': 'lcd', 'type': 'bool', 'value': False},
@@ -88,15 +89,15 @@
 
         self.set_Mock_data()
         self.emit_status(ThreadCommand('update_main_settings', [['wait_time'],
                                                                 self.settings.child('wait_time').value(), 'value']))
 
         # initialize viewers with the future type of data
         self.data_grabed_signal.emit(
-            [DataFromPlugins(name='Mock1', data=[np.array(0)], dim='Data0D', labels=['Mock1', 'label2'])])
+            [DataFromPlugins(name='Mock1', data=[np.array([0])], dim='Data0D', labels=['Mock1', 'label2'])])
 
         initialized = True
         info = 'RAS'
         return info, initialized
 
     def close(self):
         """
@@ -125,24 +126,24 @@
         for ind, data in enumerate(self.data_mock):
             data = np.roll(data, self.ind_data)
             if Naverage > 1:
                 data_tot.append(np.array([np.mean(data[0:Naverage - 1])]))
             else:
                 data_tot.append(np.array([data[0]]))
 
-        if self.settings.child(('sep_viewers')).value():
+        if self.settings.child('sep_viewers').value():
             dat = [DataFromPlugins(name=f'Mock_{ind:03}', data=[data], dim='Data0D',
                                    labels=[f'mock data {ind:03}']) for ind, data in enumerate(data_tot)]
             self.data_grabed_signal.emit(dat)
 
         else:
-            self.data_grabed_signal.emit([DataFromPlugins(name='Mock1', data=data_tot,
+            self.data_grabed_signal.emit([DataFromPlugins(name='Mock0D', data=data_tot,
                                                           dim='Data0D', labels=['dat0', 'data1'])])
         self.ind_data += 1
-        if self.settings.child('lcd').value():
+        if self.settings['lcd']:
             if not self.lcd_init:
                 self.emit_status(ThreadCommand('init_lcd', [dict(labels=['dat0', 'data1'], Nvals=2, digits=6)]))
                 QtWidgets.QApplication.processEvents()
                 self.lcd_init = True
 
             self.emit_status(ThreadCommand('lcd', [data_tot]))
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_MockAdaptive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from qtpy import QtWidgets
 from qtpy.QtCore import Signal, QThread, Slot
-from pymodaq.daq_utils import daq_utils as utils
+from pymodaq.utils import daq_utils as utils
+from pymodaq.utils.data import DataFromPlugins
 import numpy as np
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base
 from easydict import EasyDict as edict
 from collections import OrderedDict
-from pymodaq.daq_utils.daq_utils import gauss1D
+from pymodaq.utils.daq_utils import gauss1D
 from pymodaq.control_modules.viewer_utility_classes import comon_parameters
-from pymodaq.daq_utils.scanner import ScanParameters
+from pymodaq.utils.scanner import ScanParameters
 from PIL import Image
 from pathlib import Path
 
 here = Path(__file__).parent
 # %%
 with Image.open(str(here.parent.parent.joinpath('hardware', 'CNRS_degrade.png'))) as im:
     im = im.convert("L")
@@ -196,15 +197,15 @@
             if fun_type == 'Gaussians':
                 data = random_hypergaussians1D(np.roll(x_axis1D, -self.ind_data)[0], coeff)
             else:
                 data = diverging1D(np.roll(x_axis1D, -self.ind_data)[0], coeff)
 
         data = np.array([data + self.settings['noise'] * np.random.rand()])
 
-        self.data_grabed_signal.emit([utils.DataFromPlugins(name='MockAdaptive', data=[data],
+        self.data_grabed_signal.emit([DataFromPlugins(name='MockAdaptive', data=[data],
                                                             dim='Data0D', )])
         self.ind_data += 1
 
     def stop(self):
         """
             not implemented.
         """
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from qtpy.QtCore import Signal
 from easydict import EasyDict as edict
 from collections import OrderedDict
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_TCP_server
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, DataFromPlugins
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.data import DataFromPlugins, Axis
 
 
-class DAQ_0DViewer_TCPServer(DAQ_Viewer_TCP_server):
+class DAQ_1DViewer_TCPServer(DAQ_Viewer_TCP_server):
     """
         ================= ==============================
         **Attributes**      **Type**
         *command_server*    instance of Signal
         *x_axis*            1D numpy array
         *y_axis*            1D numpy array
         *data*              double precision float array
@@ -24,19 +25,18 @@
     # params = DAQ_TCP_server.params
 
     command_server = Signal(list)
 
     # params=DAQ_TCP_server.params
     def __init__(self, parent=None, params_state=None):
         super().__init__(parent, params_state,
-                         grabber_type='0D')  # initialize base class with commom attributes and methods
+                         grabber_type='1D')  # initialize base class with commom attributes and methods
 
         self.x_axis = None
         self.y_axis = None
         self.data = None
 
     def data_ready(self, data):
         """
             Send the grabed data signal.
         """
-
-        self.data_grabed_signal.emit([DataFromPlugins(name='TCPServer', data=data, dim='Data0D')])
+        self.data_grabed_signal.emit([DataFromPlugins(name='TCP Server', data=data, dim='Data1D')])
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from qtpy.QtCore import QThread
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, main
 import numpy as np
 from easydict import EasyDict as edict
 from collections import OrderedDict
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo
-from pymodaq.daq_utils.daq_utils import gauss1D
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.daq_utils import gauss1D
 from pymodaq.control_modules.viewer_utility_classes import comon_parameters
 from pymodaq_plugins_mock.daq_viewer_plugins.plugins_1D.daq_1Dviewer_Mock_spectro import DAQ_1DViewer_Mock_spectro
 
 
 class DAQ_1DViewer_Mock(DAQ_1DViewer_Mock_spectro):
     """
     Derived class from DAQ_1DViewer_Mock_spectro
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_Mock_spectro.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from qtpy.QtCore import QThread
 from qtpy import QtWidgets
-from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base
+from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, main
 import numpy as np
 from easydict import EasyDict as edict
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, DataFromPlugins, Axis
-from pymodaq.daq_utils.math_utils import gauss1D, linspace_step
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.data import DataFromPlugins, Axis
+from pymodaq.utils.math_utils import gauss1D, linspace_step
 from pymodaq.control_modules.viewer_utility_classes import comon_parameters
-from pymodaq.daq_utils.parameter.utils import iter_children
+from pymodaq.utils.parameter.utils import iter_children
 
 
 class DAQ_1DViewer_Mock_spectro(DAQ_Viewer_base):
     """
     1D viewer plugin simulating a photon spectrometer controlling the laser source, the exposure and the calibration axis
     Produces one data signal with two hypergaussians whose parameters are fully controllable or
     produces 2 data signals, each beeing a fully controllable hypergaussian
@@ -55,37 +56,35 @@
     ]
     hardware_averaging = False
 
     def __init__(self, parent=None,
                  params_state=None):  # init_params is a list of tuple where each tuple contains info on a 1D channel (Ntps,amplitude, width, position and noise)
         super().__init__(parent, params_state)
 
-        self.x_axis = Axis(label='photon wavelength', units='nm')
+        self.x_axis: Axis = None
         self.ind_data = 0
+        self._update_x_axis = True
 
     def commit_settings(self, param):
         """
             Setting the mock data
 
             ============== ========= =================
             **Parameters**  **Type**  **Description**
             *param*         none      not used
             ============== ========= =================
 
             See Also
             --------
             set_Mock_data
         """
-        if param.name() in iter_children(self.settings.child(('x_axis')), []):
+        if param.name() in iter_children(self.settings.child('x_axis'), []):
             if param.name() == 'x0':
                 self.get_spectro_wl()
-
             self.set_x_axis()
-            self.emit_x_axis()
-
         else:
             self.set_Mock_data()
 
     def set_Mock_data(self):
         """
             For each parameter of the settings tree :
                 * compute linspace numpy distribution with local parameters values
@@ -95,115 +94,117 @@
             Returns
             -------
             list
                 The computed data_mock list.
         """
         ind = -1
         self.data_mock = []
-        data = np.zeros(self.x_axis['data'].shape)
-        exposure_factor = self.settings.child('exposure_ms').value() / \
+        data = np.zeros((self.x_axis.size, ))
+        exposure_factor = self.settings['exposure_ms'] / \
             self.settings.child('exposure_ms').opts['default']
 
         for param in self.settings.children():  #
             if 'Mock' in param.name():
                 ind += 1
 
                 data_tmp = exposure_factor * \
-                    param.child('Amp').value() * gauss1D(self.x_axis['data'], param.child('x0').value(),
-                                                           param.child('dx').value(),
-                                                           param.child('n').value())
+                    param['Amp'] * gauss1D(self.x_axis.get_data(), param.child('x0').value(),
+                                           param.child('dx').value(),
+                                           param.child('n').value())
                 if ind == 0:
-                    data_tmp = data_tmp * np.sin(self.x_axis['data'] / 4) ** 2
-                data_tmp += param.child('amp_noise').value() * np.random.rand((len(self.x_axis['data'])))
-                data_tmp = self.settings.child('exposure_ms').value() /\
-                    1000 * np.roll(data_tmp, self.ind_data * self.settings.child('rolling').value())
-                if self.settings.child('multi').value():
+                    data_tmp = data_tmp * np.sin(self.x_axis.get_data() / 4) ** 2
+                data_tmp += param['amp_noise'] * np.random.rand((self.x_axis.size))
+                data_tmp = self.settings['exposure_ms'] /\
+                    1000 * np.roll(data_tmp, self.ind_data * self.settings['rolling'])
+                if self.settings['multi']:
                     self.data_mock.append(data_tmp)
                 else:
                     data += data_tmp
-        if not self.settings.child('multi').value():
+        if not self.settings['multi']:
             self.data_mock.append(data)
         self.ind_data += 1
         return self.data_mock
 
     def set_x_axis(self):
-        Npts = self.settings.child('x_axis', 'Npts').value()
-        x0 = self.settings.child('x_axis', 'x0').value()
-        dx = self.settings.child('x_axis', 'dx').value()
-        self.x_axis['data'] = linspace_step(x0 - (Npts - 1) * dx / 2, x0 + (Npts - 1) * dx / 2, dx)
-        self.emit_x_axis()
+        Npts = self.settings['x_axis', 'Npts']
+        x0 = self.settings['x_axis', 'x0']
+        dx = self.settings['x_axis', 'dx']
+        self.x_axis = Axis(label='photon wavelength', units='nm',
+                           data=linspace_step(x0 - (Npts - 1) * dx / 2, x0 + (Npts - 1) * dx / 2, dx),
+                           index=0)
+        self._update_x_axis = True
 
     def set_spectro_wl(self, spectro_wl):
         """
         Method related to spectrometer module, mandatory
         Parameters
         ----------
         spectro_wl: set the "grating" position
 
         """
         self.settings.child('x_axis', 'x0').setValue(spectro_wl)
         QtWidgets.QApplication.processEvents()
-        self.emit_status(ThreadCommand('spectro_wl', [self.settings.child('x_axis', 'x0').value()]))
+        self.emit_status(ThreadCommand('spectro_wl', [self.settings['x_axis', 'x0']]))
         self.set_x_axis()
 
     def get_spectro_wl(self):
         """
         Method related to spectrometer module, mandatory
         Get the "grating" position
         """
-        self.emit_status(ThreadCommand('spectro_wl', [self.settings.child('x_axis', 'x0').value()]))
+        self.emit_status(ThreadCommand('spectro_wl', [self.settings['x_axis', 'x0']]))
 
     def get_laser_wl(self):
         """
         Method related to spectrometer module, mandatory if laser can be set
         Get the "laser" position
         """
-        self.emit_status(ThreadCommand('laser_wl', [self.settings.child(("laser_wl")).value()]))
+        self.emit_status(ThreadCommand('laser_wl', [self.settings["laser_wl"]]))
 
     def set_laser_wl(self, laser_wl):
         """
         Method related to spectrometer module, mandatory if laser can be set
         Set the "laser" position
         """
         self.settings.child("laser_wl").setValue(laser_wl)
         QtWidgets.QApplication.processEvents()
-        self.emit_status(ThreadCommand('laser_wl', [self.settings.child(('laser_wl')).value()]))
+        self.emit_status(ThreadCommand('laser_wl', [self.settings['laser_wl']]))
 
     def get_exposure_ms(self):
-        self.emit_status(ThreadCommand('exposure_ms', [self.settings.child(('exposure_ms')).value()]))
+        self.emit_status(ThreadCommand('exposure_ms', [self.settings['exposure_ms']]))
 
     def set_exposure_ms(self, exposure):
         self.settings.child("exposure_ms").setValue(exposure)
         QtWidgets.QApplication.processEvents()
-        self.emit_status(ThreadCommand('exposure_ms', [self.settings.child(('exposure_ms')).value()]))
+        self.emit_status(ThreadCommand('exposure_ms', [self.settings['exposure_ms']]))
 
     def ini_detector(self, controller=None):
         """
             Initialisation procedure of the detector updating the status dictionnary.
 
             See Also
             --------
             set_Mock_data, daq_utils.ThreadCommand
         """
         self.status.update(edict(initialized=False, info="", x_axis=None, y_axis=None, controller=None))
         try:
 
-            if self.settings.child('controller_status').value() == "Slave":
+            if self.settings['controller_status'] == "Slave":
                 if controller is None:
                     raise Exception('no controller has been defined externally while this detector is a slave one')
                 else:
                     self.controller = controller
             else:
                 self.controller = "Mock controller"
             self.set_x_axis()
             self.set_Mock_data()
 
             # initialize viewers with the future type of data
             self.data_grabed_signal_temp.emit([DataFromPlugins(name='Mock1', data=self.data_mock, dim='Data1D',
-                                                               x_axis=self.x_axis, labels=['Mock1', 'label2']), ])
+                                                               axes=[self.x_axis], labels=['Mock1', 'label2']), ])
 
             self.status.initialized = True
             self.status.controller = self.controller
             self.status.x_axis = self.x_axis
             return self.status
 
         except Exception as e:
@@ -246,15 +247,23 @@
             QThread.msleep(self.settings.child('exposure_ms').value())
 
             for ind, data in enumerate(data_tmp):
                 data_tot[ind] += data
 
         data_tot = [data / Naverage for data in data_tot]
         QThread.msleep(self.settings.child('exposure_ms').value())
-        self.data_grabed_signal.emit([DataFromPlugins(name='Mock1', data=data_tot, dim='Data1D')])
+        if not self._update_x_axis:
+            self.data_grabed_signal.emit([DataFromPlugins(name='Mock1D', data=data_tot, dim='Data1D',)])
+        else:
+            self.data_grabed_signal.emit([DataFromPlugins(name='Mock1D', data=data_tot, dim='Data1D',
+                                                          axes=[self.x_axis])])
+            self._update_x_axis = False
 
     def stop(self):
         """
             not implemented.
         """
 
         return ""
+
+if __name__ == '__main__':
+    main(__file__)
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_1D/daq_1Dviewer_TCPServer.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_0D/daq_0Dviewer_TCPServer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from qtpy.QtCore import Signal
 from easydict import EasyDict as edict
 from collections import OrderedDict
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_TCP_server
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, DataFromPlugins, Axis
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.data import DataFromPlugins
 
 
-class DAQ_1DViewer_TCPServer(DAQ_Viewer_TCP_server):
+class DAQ_0DViewer_TCPServer(DAQ_Viewer_TCP_server):
     """
         ================= ==============================
         **Attributes**      **Type**
         *command_server*    instance of Signal
         *x_axis*            1D numpy array
         *y_axis*            1D numpy array
         *data*              double precision float array
@@ -24,18 +25,19 @@
     # params = DAQ_TCP_server.params
 
     command_server = Signal(list)
 
     # params=DAQ_TCP_server.params
     def __init__(self, parent=None, params_state=None):
         super().__init__(parent, params_state,
-                         grabber_type='1D')  # initialize base class with commom attributes and methods
+                         grabber_type='0D')  # initialize base class with commom attributes and methods
 
         self.x_axis = None
         self.y_axis = None
         self.data = None
 
     def data_ready(self, data):
         """
             Send the grabed data signal.
         """
-        self.data_grabed_signal.emit([DataFromPlugins(name='TCP Server', data=data, dim='Data1D')])
+
+        self.data_grabed_signal.emit([DataFromPlugins(name='TCPServer', data=data, dim='Data0D')])
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_Mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,24 @@
 from qtpy.QtCore import QThread, Slot, QRectF
 from qtpy import QtWidgets
 import numpy as np
-import pymodaq.daq_utils.math_utils as mutils
+import pymodaq.utils.math_utils as mutils
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, main, comon_parameters
-from easydict import EasyDict as edict
-from collections import OrderedDict
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, DataFromPlugins, Axis
-from pymodaq.daq_utils.array_manipulation import crop_array_to_axis, crop_vector_to_axis
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.data import DataFromPlugins, Axis
+from pymodaq.utils.array_manipulation import crop_array_to_axis
 
 
 class DAQ_2DViewer_Mock(DAQ_Viewer_base):
-    """
-        =============== ==================
-        **Attributes**   **Type**
-        *params*         dictionnary list
-        *x_axis*         1D numpy array
-        *y_axis*         1D numpy array
-        =============== ==================
-
-        See Also
-        --------
-        utility_classes.DAQ_Viewer_base
-    """
+    """Virtual instrument generating 2D data"""
 
     params = comon_parameters + [
         {'title': 'Nimages colors:', 'name': 'Nimagescolor', 'type': 'int', 'value': 1, 'default': 1, 'min': 0,
          'max': 3},
-        {'title': 'Nimages pannels:', 'name': 'Nimagespannel', 'type': 'int', 'value': 1, 'default': 0, 'min': 0},
+        {'title': 'Nimages pannels:', 'name': 'Nimagespannel', 'type': 'int', 'value': 2, 'default': 0, 'min': 0},
         {'title': 'Use ROISelect', 'name': 'use_roi_select', 'type': 'bool', 'value': False},
         {'title': 'Threshold', 'name': 'threshold', 'type': 'int', 'value': 1, 'min': 0},
         {'title': 'rolling', 'name': 'rolling', 'type': 'int', 'value': 1, 'min': 0},
         {'title': 'Nx', 'name': 'Nx', 'type': 'int', 'value': 100, 'default': 100, 'min': 1},
         {'title': 'Ny', 'name': 'Ny', 'type': 'int', 'value': 200, 'default': 200, 'min': 1},
         {'title': 'Amp', 'name': 'Amp', 'type': 'int', 'value': 20, 'default': 20, 'min': 1},
         {'title': 'x0', 'name': 'x0', 'type': 'slide', 'value': 50, 'default': 50, 'min': 0},
@@ -103,15 +91,15 @@
                     np.random.rand(len(y_axis), len(x_axis))
 
         for indy in range(data_mock.shape[0]):
             data_mock[indy, :] = data_mock[indy, :] * np.sin(x_axis / 4) ** 2
         data_mock = np.roll(data_mock, self.ind_data * self.settings.child('rolling').value(), axis=1)
 
         if self.settings['use_roi_select']:
-            x_axis, y_axis, data = \
+            _, _, data = \
                 crop_array_to_axis(x_axis, y_axis, data_mock,
                                    (self._ROI['position'][0], self._ROI['position'][0] + self._ROI['size'][0],
                                     self._ROI['position'][1], self._ROI['position'][1] + self._ROI['size'][1]))
 
 
             try:
                 self.image[self._ROI['position'][1]:self._ROI['position'][1] + self._ROI['size'][1]+1,
@@ -122,14 +110,16 @@
         else:
 
             self.image = data_mock
 
         self.ind_data += 1
 
         QThread.msleep(100)
+        self.x_axis = Axis(label='the x axis', data=x_axis, index=1)
+        self.y_axis = Axis(label='the y axis', data=y_axis, index=0)
 
         return self.image
 
     def ini_detector(self, controller=None):
         self.ini_detector_init(controller, "Mock controller")
 
         self.x_axis = self.get_xaxis()
@@ -198,15 +188,16 @@
         data_tmp = data_tmp / Naverage
 
         data_tmp = data_tmp * (data_tmp >= self.settings['threshold']) * (init is False)
         for ind in range(self.settings['Nimagespannel']):
             datatmptmp = []
             for indbis in range(self.settings['Nimagescolor']):
                 datatmptmp.append(data_tmp)
-            data.append(DataFromPlugins(name='Mock2D_{:d}'.format(ind), data=datatmptmp, dim='Data2D'))
+            data.append(DataFromPlugins(name='Mock2D_{:d}'.format(ind), data=datatmptmp, dim='Data2D',
+                                        axes=[self.y_axis, self.x_axis]))
         # data.append(OrderedDict(name='Mock2D_1D',data=[np.mean(data_tmp,axis=0)], type='Data1D'))
         return data
 
     def stop(self):
         """
             not implemented.
         """
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_MockCamera.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from qtpy.QtCore import QThread, Slot, QRectF
 from qtpy import QtWidgets
 import numpy as np
-import pymodaq.daq_utils.math_utils as mylib
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, main, comon_parameters
-from easydict import EasyDict as edict
-from collections import OrderedDict
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, DataFromPlugins, Axis
-from pymodaq.daq_utils.parameter import Parameter
-from pymodaq.daq_utils.parameter.utils import iter_children
-from pymodaq.daq_utils.array_manipulation import crop_array_to_axis, crop_vector_to_axis
+
+from pymodaq.utils.daq_utils import ThreadCommand
+from pymodaq.utils.data import DataFromPlugins, Axis
+from pymodaq.utils.parameter import Parameter
+from pymodaq.utils.parameter.utils import iter_children
+
 
 from pymodaq_plugins_mock.hardware.camera_wrapper import Camera
 
+
 class DAQ_2DViewer_MockCamera(DAQ_Viewer_base):
 
     params = comon_parameters + [
         {'title': 'Wait time (ms)', 'name': 'wait_time', 'type': 'int', 'value': 100, 'default': 100, 'min': 0},
         {'title': 'Nimages colors:', 'name': 'Nimagescolor', 'type': 'int', 'value': 1, 'default': 1, 'min': 0,
          'max': 3},
         {'title': 'Nimages pannels:', 'name': 'Nimagespannel', 'type': 'int', 'value': 1, 'default': 0, 'min': 0},
@@ -45,36 +45,37 @@
     def ini_attributes(self):
         self.controller: Camera = None
 
         self.x_axis = None
         self.y_axis = None
         self.live = False
         self.ind_commit = 0
+        self._update_axes = True
 
     def commit_settings(self, param: Parameter):
         """
         """
         if param.name() in iter_children(self.settings.child('current_values'), []):
             self.controller.set_value(axis=param.name(), value=param.value())
 
         if param.name() in iter_children(self.settings.child('cam_settings'), []):
             if hasattr(self.controller, param.name()):
                 setattr(self.controller, param.name(), param.value())
             self.controller.base_Mock_data()
-            self.x_axis = Axis(data=self.controller.x_axis)
-            self.y_axis = Axis(data=self.controller.y_axis)
+            self.x_axis = Axis(data=self.controller.x_axis, label='pixel', index=1)
+            self.y_axis = Axis(data=self.controller.y_axis, label='pixel', index=0)
 
     def ini_detector(self, controller=None):
         self.ini_detector_init(controller, Camera())
         self.emit_status(ThreadCommand('update_main_settings',
                                        [['wait_time'], self.settings['wait_time'], 'value']))
 
         self.controller.base_Mock_data()
-        self.x_axis = Axis(data=self.controller.x_axis)
-        self.y_axis = Axis(data=self.controller.y_axis)
+        self.x_axis = Axis(data=self.controller.x_axis, label='pixel', index=1)
+        self.y_axis = Axis(data=self.controller.y_axis, label='pixel', index=0)
 
         #apply presets to wrapper
         for settings in self.settings.child('cam_settings').children():
             if hasattr(self.controller, settings.name()):
                 setattr(self.controller, settings.name(), settings.value())
 
         # initialize viewers with the future type of data but with 0value data
@@ -158,18 +159,21 @@
         data_tmp = data_tmp / Naverage
 
         data_tmp = data_tmp * (data_tmp >= self.settings['threshold']) * (init is False)
         for ind in range(self.settings['Nimagespannel']):
             datatmptmp = []
             for indbis in range(self.settings['Nimagescolor']):
                 datatmptmp.append(data_tmp)
-            data.append(DataFromPlugins(name='Mock2D_{:d}'.format(ind), data=datatmptmp, dim='Data2D',
-                                        x_axis=self.x_axis,
-                                        y_axis=self.y_axis))
-        # data.append(OrderedDict(name='Mock2D_1D',data=[np.mean(data_tmp,axis=0)], type='Data1D'))
+            if self._update_axes:
+                data.append(DataFromPlugins(name='Mock2D_{:d}'.format(ind), data=datatmptmp, dim='Data2D',
+                                            axes=[self.x_axis, self.y_axis]))
+            else:
+                data.append(DataFromPlugins(name='Mock2D_{:d}'.format(ind), data=datatmptmp, dim='Data2D'))
+        if self._update_axes:
+            self._update_axes = False
         return data
 
     def stop(self):
         """
             not implemented.
         """
         self.live = False
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_2D/daq_2Dviewer_TCPServer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from qtpy.QtCore import Signal, Slot
-from easydict import EasyDict as edict
-from collections import OrderedDict
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_TCP_server
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, DataFromPlugins, Axis
+from pymodaq.utils.data import DataFromPlugins, Axis
 
 
 class DAQ_2DViewer_TCPServer(DAQ_Viewer_TCP_server):
     """
         ================= ==============================
         **Attributes**      **Type**
         *command_server*    instance of Signal
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/daq_viewer_plugins/plugins_ND/daq_NDviewer_Mock.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from qtpy.QtCore import QThread
 from qtpy import QtWidgets
 import numpy as np
-import pymodaq.daq_utils.daq_utils as utils
+import pymodaq.utils.daq_utils as utils
 from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base
 from easydict import EasyDict as edict
 from collections import OrderedDict
-from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, Axis, DataFromPlugins, NavAxis
+from pymodaq.utils.daq_utils import ThreadCommand, getLineInfo
+from pymodaq.utils.data import Axis, DataFromPlugins, NavAxis
 from pymodaq.control_modules.viewer_utility_classes import comon_parameters
 
 
 class DAQ_NDViewer_Mock(DAQ_Viewer_base):
     """
         =============== ==================
         **Attributes**   **Type**
@@ -94,81 +95,47 @@
                           self.settings.child('spatial_settings', 'Nx').value(),
                           self.settings.child('temp_settings', 'Nt').value()))
 
         self.time_axis = np.linspace(0, self.settings.child('temp_settings', 'Nt').value(),
                                      self.settings.child('temp_settings', 'Nt').value(),
                                      endpoint=False)
 
-        if self.settings.child('ROIselect', 'use_ROI').value():
-            self.x_axis = np.linspace(self.settings.child('ROIselect', 'x0').value(),
-                                      self.settings.child('ROIselect', 'x0').value() + self.settings.child('ROIselect',
-                                                                                                           'width').value(),
-                                      self.settings.child('ROIselect', 'width').value(), endpoint=False)
-            self.y_axis = np.linspace(self.settings.child('ROIselect', 'y0').value(),
-                                      self.settings.child('ROIselect', 'y0').value() + self.settings.child('ROIselect',
-                                                                                                           'height').value(),
-                                      self.settings.child('ROIselect', 'height').value(), endpoint=False)
-
-            data_mock = self.settings.child('spatial_settings', 'amp').value() * (
-                utils.gauss2D(self.x_axis, self.settings.child('spatial_settings', 'x0').value(),
-                              self.settings.child('spatial_settings', 'dx').value(),
-                              self.y_axis, self.settings.child('spatial_settings', 'y0').value(),
-                              self.settings.child('spatial_settings', 'dy').value(),
-                              self.settings.child('spatial_settings', 'n').value())) + self.settings.child(
-                ('amp_noise')).value() * np.random.rand(len(self.y_axis), len(self.x_axis))
-
-            for indy in range(data_mock.shape[0]):
-                data_mock[indy, :] = data_mock[indy, :] * np.sin(
-                    self.x_axis / self.settings.child('spatial_settings', 'lambda').value()) ** 2
-            data_mock = np.roll(data_mock, self.ind_data * self.settings.child('rolling').value(), axis=1)
-
-            try:
-                self.image[
-                    self.settings.child('ROIselect', 'y0').value():
-                    self.settings.child('ROIselect', 'y0').value() + self.settings.child('ROIselect', 'height').value(),
-                    self.settings.child('ROIselect', 'x0').value():
-                    self.settings.child('ROIselect', 'x0').value() + self.settings.child('ROIselect', 'width').value()] \
-                    = data_mock
-
-            except Exception as e:
-                self.emit_status(ThreadCommand('Update_Status', [getLineInfo() + str(e), 'log']))
-        else:
-            self.x_axis = np.linspace(0, self.settings.child('spatial_settings', 'Nx').value(),
-                                      self.settings.child('spatial_settings', 'Nx').value(),
-                                      endpoint=False)
-            self.y_axis = np.linspace(0, self.settings.child('spatial_settings', 'Ny').value(),
-                                      self.settings.child('spatial_settings', 'Ny').value(),
-                                      endpoint=False)
-
-            data_mock = self.settings.child('spatial_settings', 'amp').value() * (
-                utils.gauss2D(self.x_axis, self.settings.child('spatial_settings', 'x0').value(),
-                              self.settings.child('spatial_settings', 'dx').value(),
-                              self.y_axis, self.settings.child('spatial_settings', 'y0').value(),
-                              self.settings.child('spatial_settings', 'dy').value(),
-                              self.settings.child('spatial_settings', 'n').value())) + \
-                self.settings.child(('amp_noise')).value() * \
-                np.random.rand(len(self.y_axis), len(self.x_axis))
-
-            for indy in range(data_mock.shape[0]):
-                data_mock[indy, :] = data_mock[indy, :] * np.sin(
-                    self.x_axis / self.settings.child('spatial_settings', 'lambda').value()) ** 2
-
-            ind = 0
-            for indy in range(data_mock.shape[0]):
-                for indx in range(data_mock.shape[1]):
-                    image[indy, indx, :] = data_mock[indy, indx] * \
-                        utils.gauss1D(self.time_axis, self.settings.child('temp_settings', 't0').value(),
-                                      self.settings.child('temp_settings', 'dt').value(),
-                                      self.settings.child('temp_settings', 'n').value()) * \
-                        np.sin(np.roll(self.time_axis, ind) / 4) ** 2
-                    ind += 1
+        self.x_axis = np.linspace(0, self.settings.child('spatial_settings', 'Nx').value(),
+                                  self.settings.child('spatial_settings', 'Nx').value(),
+                                  endpoint=False)
+        self.y_axis = np.linspace(0, self.settings.child('spatial_settings', 'Ny').value(),
+                                  self.settings.child('spatial_settings', 'Ny').value(),
+                                  endpoint=False)
+
+        data_mock = self.settings.child('spatial_settings', 'amp').value() * (
+            utils.gauss2D(self.x_axis, self.settings.child('spatial_settings', 'x0').value(),
+                          self.settings.child('spatial_settings', 'dx').value(),
+                          self.y_axis, self.settings.child('spatial_settings', 'y0').value(),
+                          self.settings.child('spatial_settings', 'dy').value(),
+                          self.settings.child('spatial_settings', 'n').value())) + \
+            self.settings.child(('amp_noise')).value() * \
+            np.random.rand(len(self.y_axis), len(self.x_axis))
+
+        for indy in range(data_mock.shape[0]):
+            data_mock[indy, :] = data_mock[indy, :] * np.sin(
+                self.x_axis / self.settings.child('spatial_settings', 'lambda').value()) ** 2
+
+        ind = 0
+        for indy in range(data_mock.shape[0]):
+            for indx in range(data_mock.shape[1]):
+                image[indy, indx, :] = data_mock[indy, indx] * \
+                    utils.gauss1D(self.time_axis, self.settings.child('temp_settings', 't0').value(),
+                                  self.settings.child('temp_settings', 'dt').value(),
+                                  self.settings.child('temp_settings', 'n').value()) * \
+                    np.sin(np.roll(self.time_axis, ind) / 4) ** 2
+                ind += 1
 
-            image = np.roll(image, self.ind_data * self.settings.child(('rolling')).value(), axis=1)
+        image = np.roll(image, self.ind_data * self.settings.child(('rolling')).value(), axis=1)
 
-            self.image = image
+        self.image = image
 
         self.ind_data += 1
 
         QThread.msleep(100)
 
         return self.image
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/CNRS_degrade.png`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/hardware/camera_wrapper.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/camera_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Created the 24/10/2022
 
 @author: Sebastien Weber
 """
 import numpy as np
-import pymodaq.daq_utils.math_utils as mylib
+import pymodaq.utils.math_utils as mutils
 
 
 class Camera:
     Nx = 256
     Ny = 256
     amp = 20
     x0 = 128
@@ -35,15 +35,15 @@
         if axis == 'Theta':
             self.base_Mock_data()
 
     def base_Mock_data(self):
         self.x_axis = np.linspace(0, self.Nx, self.Nx, endpoint=False)
         self.y_axis = np.linspace(0, self.Ny, self.Ny, endpoint=False)
         data_mock = self.amp * (
-            mylib.gauss2D(self.x_axis, self.x0, self.dx,
+            mutils.gauss2D(self.x_axis, self.x0, self.dx,
                           self.y_axis, self.y0, self.dy,
                           self.n,
                           angle=self._current_value['Theta']))
 
         for indy in range(data_mock.shape[0]):
             if self.fringes:
                 data_mock[indy, :] = data_mock[indy, :] * np.sin(self.x_axis / 4) ** 2
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/hardware/wrapper.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/hardware/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Demo Wrapper to illustrate the plugin developpement. This Mock wrapper will emulate communication with an instrument
 """
 
 from time import perf_counter, sleep
 import math
 from numpy import random
 
+ports = ['COM1', 'COM2']
+
 
 class ActuatorWrapper:
     units = 'mm'
 
     def __init__(self):
         self._com_port = ''
         self._current_value = 0
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock/models/PIDModelBeamSteering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pymodaq.pid.utils import PIDModelGeneric, OutputToActuator, InputFromDetector, main
+from pymodaq.extensions.pid.utils import PIDModelGeneric, OutputToActuator, InputFromDetector, main
 from scipy.ndimage import center_of_mass
 
 
 class PIDModelBeamSteering(PIDModelGeneric):
     limits = dict(max=dict(state=False, value=100),
                   min=dict(state=False, value=-100),)
     konstants = dict(kp=0.1, ki=0.000, kd=0.0000)
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock.egg-info/PKG-INFO` & `pymodaq_plugins_mock-4.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pymodaq-plugins-mock
-Version: 4.0.0
+Name: pymodaq_plugins_mock
+Version: 4.0.1
 Summary: Set of base PyMoDAQ plugins including Mock ones for development
 Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_mock
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: CECILL B
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,15 +29,16 @@
    :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://github.com/PyMoDAQ/pymodaq_plugins/workflows/Upload%20Python%20Package/badge.svg
     :target: https://github.com/PyMoDAQ/pymodaq_plugins
 
 Plugins initially developed with PyMoDAQ. Includes Mock plugins that are plugins of virtual instruments dedicated
-to code testing for new functionalities or development.
+to code testing for new functionalities or development. From version 4.0.0 onwards, these plugins will only work with
+pymodaq > 4.0.0
 
 
 Authors
 =======
 
 * Sebastien J. Weber
```

### Comparing `pymodaq_plugins_mock-4.0.0/src/pymodaq_plugins_mock.egg-info/SOURCES.txt` & `pymodaq_plugins_mock-4.0.1/src/pymodaq_plugins_mock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

