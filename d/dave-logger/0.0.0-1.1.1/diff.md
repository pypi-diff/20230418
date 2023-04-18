# Comparing `tmp/dave-logger-0.0.0.tar.gz` & `tmp/dave-logger-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dave-logger-0.0.0.tar", last modified: Tue Apr 18 18:10:30 2023, max compression
+gzip compressed data, was "dave-logger-1.1.1.tar", last modified: Tue Apr 18 18:13:15 2023, max compression
```

## Comparing `dave-logger-0.0.0.tar` & `dave-logger-1.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 velicanu   (501) staff       (20)        0 2023-04-18 18:10:30.020647 dave-logger-0.0.0/
--rw-r--r--   0 velicanu   (501) staff       (20)      136 2023-04-18 18:10:30.020216 dave-logger-0.0.0/PKG-INFO
--rw-r--r--   0 velicanu   (501) staff       (20)      257 2022-12-20 15:23:53.000000 dave-logger-0.0.0/README.md
-drwxr-xr-x   0 velicanu   (501) staff       (20)        0 2023-04-18 18:10:30.019365 dave-logger-0.0.0/dave_logger.egg-info/
--rw-r--r--   0 velicanu   (501) staff       (20)      136 2023-04-18 18:10:29.000000 dave-logger-0.0.0/dave_logger.egg-info/PKG-INFO
--rw-r--r--   0 velicanu   (501) staff       (20)      158 2023-04-18 18:10:29.000000 dave-logger-0.0.0/dave_logger.egg-info/SOURCES.txt
--rw-r--r--   0 velicanu   (501) staff       (20)        1 2023-04-18 18:10:29.000000 dave-logger-0.0.0/dave_logger.egg-info/dependency_links.txt
--rw-r--r--   0 velicanu   (501) staff       (20)        1 2023-04-18 18:10:29.000000 dave-logger-0.0.0/dave_logger.egg-info/top_level.txt
--rw-r--r--   0 velicanu   (501) staff       (20)       38 2023-04-18 18:10:30.020769 dave-logger-0.0.0/setup.cfg
--rw-r--r--   0 velicanu   (501) staff       (20)      281 2023-04-18 18:09:53.000000 dave-logger-0.0.0/setup.py
+drwxr-xr-x   0 velicanu   (501) staff       (20)        0 2023-04-18 18:13:15.563889 dave-logger-1.1.1/
+-rw-r--r--   0 velicanu   (501) staff       (20)      136 2023-04-18 18:13:15.563534 dave-logger-1.1.1/PKG-INFO
+-rw-r--r--   0 velicanu   (501) staff       (20)      257 2022-12-20 15:23:53.000000 dave-logger-1.1.1/README.md
+drwxr-xr-x   0 velicanu   (501) staff       (20)        0 2023-04-18 18:13:15.562839 dave-logger-1.1.1/dave_logger.egg-info/
+-rw-r--r--   0 velicanu   (501) staff       (20)      136 2023-04-18 18:13:15.000000 dave-logger-1.1.1/dave_logger.egg-info/PKG-INFO
+-rw-r--r--   0 velicanu   (501) staff       (20)      158 2023-04-18 18:13:15.000000 dave-logger-1.1.1/dave_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 velicanu   (501) staff       (20)        1 2023-04-18 18:13:15.000000 dave-logger-1.1.1/dave_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 velicanu   (501) staff       (20)        1 2023-04-18 18:13:15.000000 dave-logger-1.1.1/dave_logger.egg-info/top_level.txt
+-rw-r--r--   0 velicanu   (501) staff       (20)       38 2023-04-18 18:13:15.564026 dave-logger-1.1.1/setup.cfg
+-rw-r--r--   0 velicanu   (501) staff       (20)      281 2023-04-18 18:13:06.000000 dave-logger-1.1.1/setup.py
```

