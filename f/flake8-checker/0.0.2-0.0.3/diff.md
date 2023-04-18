# Comparing `tmp/flake8-checker-0.0.2.tar.gz` & `tmp/flake8-checker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-checker-0.0.2.tar", last modified: Mon Apr 17 21:30:18 2023, max compression
+gzip compressed data, was "flake8-checker-0.0.3.tar", last modified: Tue Apr 18 04:46:41 2023, max compression
```

## Comparing `flake8-checker-0.0.2.tar` & `flake8-checker-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 harish    (1000) harish    (1000)        0 2023-04-17 21:30:18.343549 flake8-checker-0.0.2/
--rw-rw-r--   0 harish    (1000) harish    (1000)      300 2023-04-17 21:30:18.343549 flake8-checker-0.0.2/PKG-INFO
-drwxrwxr-x   0 harish    (1000) harish    (1000)        0 2023-04-17 21:30:18.343549 flake8-checker-0.0.2/flake8_checker.egg-info/
--rw-rw-r--   0 harish    (1000) harish    (1000)      300 2023-04-17 21:30:18.000000 flake8-checker-0.0.2/flake8_checker.egg-info/PKG-INFO
--rw-rw-r--   0 harish    (1000) harish    (1000)      256 2023-04-17 21:30:18.000000 flake8-checker-0.0.2/flake8_checker.egg-info/SOURCES.txt
--rw-rw-r--   0 harish    (1000) harish    (1000)        1 2023-04-17 21:30:18.000000 flake8-checker-0.0.2/flake8_checker.egg-info/dependency_links.txt
--rw-rw-r--   0 harish    (1000) harish    (1000)       75 2023-04-17 21:30:18.000000 flake8-checker-0.0.2/flake8_checker.egg-info/entry_points.txt
--rw-rw-r--   0 harish    (1000) harish    (1000)        7 2023-04-17 21:30:18.000000 flake8-checker-0.0.2/flake8_checker.egg-info/requires.txt
--rw-rw-r--   0 harish    (1000) harish    (1000)       15 2023-04-17 21:30:18.000000 flake8-checker-0.0.2/flake8_checker.egg-info/top_level.txt
--rw-rw-r--   0 harish    (1000) harish    (1000)     1191 2023-04-16 20:53:51.000000 flake8-checker-0.0.2/flake8_checker.py
--rw-rw-r--   0 harish    (1000) harish    (1000)       38 2023-04-17 21:30:18.343549 flake8-checker-0.0.2/setup.cfg
--rw-rw-r--   0 harish    (1000) harish    (1000)      504 2023-04-17 21:29:50.000000 flake8-checker-0.0.2/setup.py
+drwxrwxr-x   0 harish    (1000) harish    (1000)        0 2023-04-18 04:46:41.548959 flake8-checker-0.0.3/
+-rw-rw-r--   0 harish    (1000) harish    (1000)      289 2023-04-18 04:46:41.548959 flake8-checker-0.0.3/PKG-INFO
+drwxrwxr-x   0 harish    (1000) harish    (1000)        0 2023-04-18 04:46:41.548959 flake8-checker-0.0.3/flake8_checker.egg-info/
+-rw-rw-r--   0 harish    (1000) harish    (1000)      289 2023-04-18 04:46:41.000000 flake8-checker-0.0.3/flake8_checker.egg-info/PKG-INFO
+-rw-rw-r--   0 harish    (1000) harish    (1000)      256 2023-04-18 04:46:41.000000 flake8-checker-0.0.3/flake8_checker.egg-info/SOURCES.txt
+-rw-rw-r--   0 harish    (1000) harish    (1000)        1 2023-04-18 04:46:41.000000 flake8-checker-0.0.3/flake8_checker.egg-info/dependency_links.txt
+-rw-rw-r--   0 harish    (1000) harish    (1000)       73 2023-04-18 04:46:41.000000 flake8-checker-0.0.3/flake8_checker.egg-info/entry_points.txt
+-rw-rw-r--   0 harish    (1000) harish    (1000)        7 2023-04-18 04:46:41.000000 flake8-checker-0.0.3/flake8_checker.egg-info/requires.txt
+-rw-rw-r--   0 harish    (1000) harish    (1000)       15 2023-04-18 04:46:41.000000 flake8-checker-0.0.3/flake8_checker.egg-info/top_level.txt
+-rw-rw-r--   0 harish    (1000) harish    (1000)     1462 2023-04-18 04:46:00.000000 flake8-checker-0.0.3/flake8_checker.py
+-rw-rw-r--   0 harish    (1000) harish    (1000)       38 2023-04-18 04:46:41.548959 flake8-checker-0.0.3/setup.cfg
+-rw-rw-r--   0 harish    (1000) harish    (1000)      491 2023-04-18 04:24:56.000000 flake8-checker-0.0.3/setup.py
```

