# Comparing `tmp/az_basics-0.0.1.tar.gz` & `tmp/az_basics-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "az_basics-0.0.1.tar", max compression
+gzip compressed data, was "az_basics-0.0.2.tar", max compression
```

## Comparing `az_basics-0.0.1.tar` & `az_basics-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       50 2023-04-18 12:34:37.931466 az_basics-0.0.1/az_basics/__init__.py
--rw-r--r--   0        0        0      108 2023-04-18 12:27:26.192839 az_basics-0.0.1/az_basics/toy.py
--rw-r--r--   0        0        0      482 2023-04-18 12:55:08.714101 az_basics-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       45 2023-04-18 13:32:09.541025 az_basics-0.0.1/README.md
--rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 az_basics-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-04-18 12:34:37.931466 az_basics-0.0.2/az_basics/__init__.py
+-rw-r--r--   0        0        0      108 2023-04-18 12:27:26.192839 az_basics-0.0.2/az_basics/toy.py
+-rw-r--r--   0        0        0      482 2023-04-18 14:20:08.599334 az_basics-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-04-18 13:32:09.541025 az_basics-0.0.2/README.md
+-rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 az_basics-0.0.2/PKG-INFO
```

