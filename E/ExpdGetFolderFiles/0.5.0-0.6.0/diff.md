# Comparing `tmp/ExpdGetFolderFiles-0.5.0.tar.gz` & `tmp/ExpdGetFolderFiles-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ExpdGetFolderFiles-0.5.0.tar", last modified: Fri Apr  7 09:04:48 2023, max compression
+gzip compressed data, was "dist\ExpdGetFolderFiles-0.6.0.tar", last modified: Tue Apr 18 05:33:33 2023, max compression
```

## Comparing `ExpdGetFolderFiles-0.5.0.tar` & `ExpdGetFolderFiles-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 09:04:48.000000 ExpdGetFolderFiles-0.5.0/
--rw-rw-rw-   0        0        0      262 2023-04-07 09:04:48.000000 ExpdGetFolderFiles-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-04-07 09:02:30.000000 ExpdGetFolderFiles-0.5.0/README.md
--rw-rw-rw-   0        0        0      115 2023-04-07 09:04:48.000000 ExpdGetFolderFiles-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      376 2023-04-07 09:03:58.000000 ExpdGetFolderFiles-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:04:48.000000 ExpdGetFolderFiles-0.5.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 09:04:48.000000 ExpdGetFolderFiles-0.5.0/src/ExpdGetFolderFiles/
--rw-rw-rw-   0        0        0      665 2023-04-07 08:42:55.000000 ExpdGetFolderFiles-0.5.0/src/ExpdGetFolderFiles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:04:48.000000 ExpdGetFolderFiles-0.5.0/src/ExpdGetFolderFiles.egg-info/
--rw-rw-rw-   0        0        0      262 2023-04-07 09:04:47.000000 ExpdGetFolderFiles-0.5.0/src/ExpdGetFolderFiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-07 09:04:47.000000 ExpdGetFolderFiles-0.5.0/src/ExpdGetFolderFiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 09:04:47.000000 ExpdGetFolderFiles-0.5.0/src/ExpdGetFolderFiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-07 09:04:47.000000 ExpdGetFolderFiles-0.5.0/src/ExpdGetFolderFiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-07 09:04:47.000000 ExpdGetFolderFiles-0.5.0/src/ExpdGetFolderFiles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 05:33:33.000000 ExpdGetFolderFiles-0.6.0/
+-rw-rw-rw-   0        0        0      262 2023-04-18 05:33:33.000000 ExpdGetFolderFiles-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-04-07 09:12:49.000000 ExpdGetFolderFiles-0.6.0/README.md
+-rw-rw-rw-   0        0        0      115 2023-04-18 05:33:33.000000 ExpdGetFolderFiles-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      376 2023-04-18 05:25:17.000000 ExpdGetFolderFiles-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:33:33.000000 ExpdGetFolderFiles-0.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 05:33:33.000000 ExpdGetFolderFiles-0.6.0/src/ExpdGetFolderFiles/
+-rw-rw-rw-   0        0        0      858 2023-04-18 05:33:14.000000 ExpdGetFolderFiles-0.6.0/src/ExpdGetFolderFiles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:33:33.000000 ExpdGetFolderFiles-0.6.0/src/ExpdGetFolderFiles.egg-info/
+-rw-rw-rw-   0        0        0      262 2023-04-18 05:33:33.000000 ExpdGetFolderFiles-0.6.0/src/ExpdGetFolderFiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-18 05:33:33.000000 ExpdGetFolderFiles-0.6.0/src/ExpdGetFolderFiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:33:33.000000 ExpdGetFolderFiles-0.6.0/src/ExpdGetFolderFiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 05:33:33.000000 ExpdGetFolderFiles-0.6.0/src/ExpdGetFolderFiles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-18 05:33:33.000000 ExpdGetFolderFiles-0.6.0/src/ExpdGetFolderFiles.egg-info/top_level.txt
```

