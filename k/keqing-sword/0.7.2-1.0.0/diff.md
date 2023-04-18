# Comparing `tmp/keqing_sword-0.7.2.tar.gz` & `tmp/keqing_sword-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keqing_sword-0.7.2.tar", max compression
+gzip compressed data, was "keqing_sword-1.0.0.tar", max compression
```

## Comparing `keqing_sword-0.7.2.tar` & `keqing_sword-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-04-17 07:01:30.054163 keqing_sword-0.7.2/LICENSE
--rw-r--r--   0        0        0     3764 2023-04-17 07:01:30.054163 keqing_sword-0.7.2/README.md
--rw-r--r--   0        0        0      704 2023-04-17 07:03:03.466672 keqing_sword-0.7.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/__init__.py
--rw-r--r--   0        0        0       89 2023-04-17 07:02:45.882558 keqing_sword-0.7.2/src/kqs/global_const.py
--rw-r--r--   0        0        0     1689 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_diff.py
--rw-r--r--   0        0        0     2211 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_getosm.py
--rw-r--r--   0        0        0     1071 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_getosm.py.LICENSE
--rw-r--r--   0        0        0      137 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_getosm.py.METADATA
--rw-r--r--   0        0        0      514 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_network.py
--rw-r--r--   0        0        0     1130 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_parse.py
--rw-r--r--   0        0        0     1686 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_query.py
--rw-r--r--   0        0        0       10 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_stream_read.py
--rw-r--r--   0        0        0        0 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/method_stream_write.py
--rw-r--r--   0        0        0     3093 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/model_basic.py
--rw-r--r--   0        0        0     1789 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/type_constraint.py
--rw-r--r--   0        0        0      498 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/type_data.py
--rw-r--r--   0        0        0     5417 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/type_element.py
--rw-r--r--   0        0        0    14429 2023-04-17 07:01:30.058164 keqing_sword-0.7.2/src/kqs/waifu.py
--rw-r--r--   0        0        0     4396 1970-01-01 00:00:00.000000 keqing_sword-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-18 12:19:28.364059 keqing_sword-1.0.0/LICENSE
+-rw-r--r--   0        0        0      580 2023-04-18 17:06:40.963391 keqing_sword-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      169 2023-04-18 17:02:49.466344 keqing_sword-1.0.0/README.md
+-rw-r--r--   0        0        0      254 2023-04-18 17:00:06.375765 keqing_sword-1.0.0/src/keqing/__init__.py
+-rw-r--r--   0        0        0      254 2023-04-18 17:00:06.375765 keqing_sword-1.0.0/src/keqing/__main__.py
+-rw-r--r--   0        0        0     1199 1970-01-01 00:00:00.000000 keqing_sword-1.0.0/PKG-INFO
```

