# Comparing `tmp/waffle_hub-0.1.7.tar.gz` & `tmp/waffle_hub-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_hub-0.1.7.tar", last modified: Wed Apr 12 07:56:56 2023, max compression
+gzip compressed data, was "waffle_hub-0.1.8.tar", last modified: Mon Apr 17 23:08:26 2023, max compression
```

## Comparing `waffle_hub-0.1.7.tar` & `waffle_hub-0.1.8.tar`

### file list

```diff
@@ -1,51 +1,68 @@
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-03-20 23:40:26.000000 waffle_hub-0.1.7/LICENSE
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-03-20 23:40:26.000000 waffle_hub-0.1.7/MANIFEST.in
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1966 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      885 2023-04-03 23:38:22.000000 waffle_hub-0.1.7/README.md
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      213 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/requirements.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/setup.cfg
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2643 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/setup.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/tests/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     6878 2023-04-12 07:56:27.000000 waffle_hub-0.1.7/tests/test_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2500 2023-04-12 07:56:27.000000 waffle_hub-0.1.7/waffle_hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/experimental/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/experimental/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/experimental/serve.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/hub/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       63 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/configs/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/configs/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2573 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1793 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     8318 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/tx_model_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/hub/adapter/ultralytics/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/ultralytics/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10931 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    21793 2023-04-12 07:56:27.000000 waffle_hub-0.1.7/waffle_hub/hub/base_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/hub/model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/hub/model/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     6340 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/hub/model/wrapper.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1247 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/run.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/schema/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/schema/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      614 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/schema/base_schema.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1257 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/schema/configs.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1170 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/schema/data.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub/utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.7/waffle_hub/utils/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5480 2023-04-12 07:56:27.000000 waffle_hub-0.1.7/waffle_hub/utils/callback.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3385 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/utils/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2239 2023-04-10 11:39:56.000000 waffle_hub-0.1.7/waffle_hub/utils/draw.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-12 07:56:56.175392 waffle_hub-0.1.7/waffle_hub.egg-info/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1966 2023-04-12 07:56:56.000000 waffle_hub-0.1.7/waffle_hub.egg-info/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1119 2023-04-12 07:56:56.000000 waffle_hub-0.1.7/waffle_hub.egg-info/SOURCES.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-04-12 07:56:56.000000 waffle_hub-0.1.7/waffle_hub.egg-info/dependency_links.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-04-12 07:56:56.000000 waffle_hub-0.1.7/waffle_hub.egg-info/entry_points.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      172 2023-04-12 07:56:56.000000 waffle_hub-0.1.7/waffle_hub.egg-info/requires.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-04-12 07:56:56.000000 waffle_hub-0.1.7/waffle_hub.egg-info/top_level.txt
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-03-20 23:40:26.000000 waffle_hub-0.1.8/LICENSE
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-03-20 23:40:26.000000 waffle_hub-0.1.8/MANIFEST.in
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1966 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      885 2023-04-03 23:38:22.000000 waffle_hub-0.1.8/README.md
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      213 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/requirements.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/setup.cfg
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2643 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/setup.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/tests/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3721 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/tests/test_dataset.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7085 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/tests/test_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3844 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/dataset/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/dataset/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/dataset/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      102 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/dataset/adapter/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2715 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/dataset/adapter/coco.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4566 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/dataset/adapter/yolo.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    20015 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/dataset/dataset.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/experimental/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/waffle_hub/experimental/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/experimental/auto_label/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-13 02:15:00.000000 waffle_hub-0.1.8/waffle_hub/experimental/auto_label/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7920 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/experimental/auto_label/grounding_dino.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/waffle_hub/experimental/serve.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/hub/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       63 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/configs/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/configs/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2573 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1793 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     8318 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/tx_model_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/hub/adapter/ultralytics/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/ultralytics/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10931 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    23011 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/hub/base_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/hub/model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/hub/model/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     6296 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/hub/model/wrapper.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1247 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/run.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/schema/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      806 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/base_schema.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1257 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/waffle_hub/schema/configs.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      785 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/data.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/schema/fields/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/fields/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    13649 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/fields/annotation.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1341 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/fields/base_field.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     6827 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/fields/category.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2581 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/schema/fields/image.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub/utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-10 11:40:54.000000 waffle_hub-0.1.8/waffle_hub/utils/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     5480 2023-04-12 07:56:27.000000 waffle_hub-0.1.8/waffle_hub/utils/callback.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3385 2023-04-10 11:39:56.000000 waffle_hub-0.1.8/waffle_hub/utils/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2330 2023-04-17 23:02:39.000000 waffle_hub-0.1.8/waffle_hub/utils/draw.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 23:08:26.810531 waffle_hub-0.1.8/waffle_hub.egg-info/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1966 2023-04-17 23:08:26.000000 waffle_hub-0.1.8/waffle_hub.egg-info/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1597 2023-04-17 23:08:26.000000 waffle_hub-0.1.8/waffle_hub.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-04-17 23:08:26.000000 waffle_hub-0.1.8/waffle_hub.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-04-17 23:08:26.000000 waffle_hub-0.1.8/waffle_hub.egg-info/entry_points.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      172 2023-04-17 23:08:26.000000 waffle_hub-0.1.8/waffle_hub.egg-info/requires.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-04-17 23:08:26.000000 waffle_hub-0.1.8/waffle_hub.egg-info/top_level.txt
```

### Comparing `waffle_hub-0.1.7/LICENSE` & `waffle_hub-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.7/PKG-INFO` & `waffle_hub-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle_hub
-Version: 0.1.7
+Version: 0.1.8
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle_hub Version: 0.1.7 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle_hub Version: 0.1.8 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.1.7/README.md` & `waffle_hub-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.7/setup.py` & `waffle_hub-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.7/tests/test_hub.py` & `waffle_hub-0.1.8/tests/test_hub.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,64 @@
 import time
 from pathlib import Path
 
 import pytest
 import torch
-from waffle_utils.dataset import Dataset
-from waffle_utils.file import io, network
 
+from waffle_hub import TaskType
+from waffle_hub.dataset import Dataset
 from waffle_hub.hub.adapter.ultralytics import UltralyticsHub
 from waffle_hub.utils.callback import (
     ExportCallback,
     InferenceCallback,
     TrainCallback,
 )
 
 
 @pytest.fixture
-def dummy_dataset(tmpdir: Path):
-    url = "https://raw.githubusercontent.com/snuailab/assets/main/waffle/sample_dataset/mnist.zip"
+def object_detection_dataset(coco_path: Path, tmpdir: Path):
+    dataset: Dataset = Dataset.from_coco(
+        name="od",
+        task=TaskType.OBJECT_DETECTION,
+        coco_file=coco_path / "coco.json",
+        coco_root_dir=coco_path / "images",
+        root_dir=tmpdir,
+    )
+    dataset.split(0.8)
 
-    dummy_zip_file = tmpdir / "mnist.zip"
-    dummy_extract_dir = tmpdir / "extract"
-    dummy_coco_root_dir = tmpdir / "extract/images"
-    dummy_coco_file = tmpdir / "extract/coco.json"
+    return dataset
 
-    network.get_file_from_url(url, dummy_zip_file, create_directory=True)
-    io.unzip(dummy_zip_file, dummy_extract_dir, create_directory=True)
 
-    ds = Dataset.from_coco(
-        "mnist", dummy_coco_file, Path(dummy_coco_root_dir), root_dir=tmpdir
+@pytest.fixture
+def classification_dataset(coco_path: Path, tmpdir: Path):
+    dataset: Dataset = Dataset.from_coco(
+        name="cls",
+        task=TaskType.CLASSIFICATION,
+        coco_file=coco_path / "coco.json",
+        coco_root_dir=coco_path / "images",
+        root_dir=tmpdir,
     )
-    ds.split(0.8)
-    return ds
+    dataset.split(0.8)
 
+    return dataset
 
-def test_ultralytics_object_detection(tmpdir: Path, dummy_dataset: Dataset):
 
-    export_dir = dummy_dataset.export("yolo_detection")
+def test_ultralytics_object_detection(
+    object_detection_dataset: Dataset, tmpdir: Path
+):
 
-    name = "test_det"
+    export_dir = object_detection_dataset.export("yolo")
 
+    name = "test_det"
     hub = UltralyticsHub.new(
         name=name,
-        task="object_detection",
+        task=TaskType.OBJECT_DETECTION,
         model_type="yolov8",
         model_size="n",
-        categories=["1", "2"],
+        categories=object_detection_dataset.category_names,
         root_dir=tmpdir,
     )
     hub = UltralyticsHub.load(name=name, root_dir=tmpdir)
     hub: UltralyticsHub = UltralyticsHub.from_model_config(
         name=name,
         model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
@@ -66,14 +76,15 @@
     assert Path(train_callback.best_ckpt_file).exists()
     assert Path(train_callback.last_ckpt_file).exists()
     assert Path(train_callback.metric_file).exists()
     assert Path(train_callback.result_dir).exists()
 
     inference_callback: InferenceCallback = hub.inference(
         source=export_dir,
+        draw=True,
         device="cpu",
     )
     assert inference_callback.get_progress() == 1
     assert Path(inference_callback.inference_dir).exists()
 
     export_callback: ExportCallback = hub.export()
     assert Path(export_callback.export_file).exists()
@@ -85,26 +96,27 @@
 
     x = torch.randn(4, 3, 64, 64)
     layer_name = layer_names[-1]
     x, feature_maps = model.get_feature_maps(x, layer_name)
     assert len(feature_maps) == 1
 
 
-def test_ultralytics_classification(tmpdir: Path, dummy_dataset: Dataset):
+def test_ultralytics_classification(
+    classification_dataset: Dataset, tmpdir: Path
+):
 
-    export_dir = dummy_dataset.export("yolo_classification")
+    export_dir = classification_dataset.export("yolo")
 
     name = "test_cls"
-
     hub = UltralyticsHub.new(
         name=name,
-        task="classification",
+        task=TaskType.CLASSIFICATION,
         model_type="yolov8",
         model_size="n",
-        categories=["1", "2"],
+        categories=classification_dataset.category_names,
         root_dir=tmpdir,
     )
     hub = UltralyticsHub.load(name=name, root_dir=tmpdir)
     hub: UltralyticsHub = UltralyticsHub.from_model_config(
         name=name,
         model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
@@ -122,14 +134,15 @@
     assert Path(train_callback.best_ckpt_file).exists()
     assert Path(train_callback.last_ckpt_file).exists()
     assert Path(train_callback.metric_file).exists()
     assert Path(train_callback.result_dir).exists()
 
     inference_callback: InferenceCallback = hub.inference(
         source=export_dir,
+        draw=True,
         device="cpu",
     )
     assert inference_callback.get_progress() == 1
     assert Path(inference_callback.inference_dir).exists()
 
     export_callback: ExportCallback = hub.export()
     assert Path(export_callback.export_file).exists()
@@ -141,26 +154,26 @@
 
     x = torch.randn(4, 3, 64, 64)
     layer_name = layer_names[-1]
     x, feature_maps = model.get_feature_maps(x, layer_name)
     assert len(feature_maps) == 1
 
 
-def test_non_hold(tmpdir: Path, dummy_dataset: Dataset):
+def test_non_hold(classification_dataset: Dataset, tmpdir: Path):
 
-    export_dir = dummy_dataset.export("yolo_detection")
+    export_dir = classification_dataset.export("yolo")
 
-    name = "test_det_hold"
+    name = "test_hold"
 
     hub = UltralyticsHub.new(
         name=name,
-        task="object_detection",
+        task=TaskType.CLASSIFICATION,
         model_type="yolov8",
         model_size="n",
-        categories=["1", "2"],
+        categories=classification_dataset.category_names,
         root_dir=tmpdir,
     )
     hub = UltralyticsHub.load(name=name, root_dir=tmpdir)
     hub: UltralyticsHub = UltralyticsHub.from_model_config(
         name=name,
         model_config_file=tmpdir / name / UltralyticsHub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
```

### Comparing `waffle_hub-0.1.7/waffle_hub/experimental/serve.py` & `waffle_hub-0.1.8/waffle_hub/experimental/serve.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py` & `waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/configs/data_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py` & `waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/configs/model_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.7/waffle_hub/hub/adapter/tx_model/tx_model_hub.py` & `waffle_hub-0.1.8/waffle_hub/hub/adapter/tx_model/tx_model_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.7/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py` & `waffle_hub-0.1.8/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.7/waffle_hub/hub/base_hub.py` & `waffle_hub-0.1.8/waffle_hub/hub/base_hub.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import cv2
 import torch
 import tqdm
 from waffle_utils.file import io
 from waffle_utils.utils import type_validator
 
+from waffle_hub import TaskType
 from waffle_hub.hub.model.wrapper import get_parser
 from waffle_hub.schema.configs import (
     ExportConfig,
     InferenceConfig,
     ModelConfig,
     TrainConfig,
 )
@@ -63,15 +64,15 @@
     ONNX_FILE = "weights/model.onnx"
 
     def __init__(
         self,
         name: str,
         backend: str = None,
         version: str = None,
-        task: str = None,
+        task: Union[str, TaskType] = None,
         model_type: str = None,
         model_size: str = None,
         categories: Union[list[dict], list] = None,
         root_dir: str = None,
     ):
         self.name: str = name
         self.task: str = task
@@ -179,16 +180,16 @@
 
     @property
     def task(self) -> str:
         """Task Name"""
         return self.__task
 
     @task.setter
-    @type_validator(str)
     def task(self, v):
+        v = str(v).lower()  # TODO: MODEL_TYPES should be enum
         if v not in self.MODEL_TYPES:
             raise ValueError(
                 f"Task {v} is not supported. Choose one of {self.MODEL_TYPES}"
             )
         self.__task = v
 
     @property
@@ -333,19 +334,15 @@
         return TrainConfig.load(self.train_config_file)
 
     def get_model_config(self):
         return ModelConfig.load(self.model_config_file)
 
     # Train Hook
     def before_train(self, cfg: TrainConfig):
-        if self.artifact_dir.exists():
-            raise FileExistsError(
-                f"{self.artifact_dir}\n"
-                "Train artifacts already exist. Remove artifact to re-train (hub.delete_artifact())."
-            )
+        pass
 
     def on_train_start(self, cfg: TrainConfig):
         pass
 
     def save_train_config(self, cfg: TrainConfig):
         cfg.save_yaml(self.train_config_file)
 
@@ -394,14 +391,36 @@
             FileNotFoundError: if can not detect appropriate dataset.
             ValueError: if can not detect appropriate dataset.
             e: something gone wrong with ultralytics
 
         Returns:
             TrainCallback: train callback
         """
+        
+        if self.artifact_dir.exists():
+            raise FileExistsError(
+                f"{self.artifact_dir}\n"
+                "Train artifacts already exist. Remove artifact to re-train (hub.delete_artifact())."
+            )
+
+        def inner(callback: TrainCallback):
+            try:
+                self.before_train(cfg)
+                self.on_train_start(cfg)
+                self.save_train_config(cfg)
+                self.training(cfg, callback)
+                self.on_train_end(cfg)
+                self.after_train(cfg)
+                callback.force_finish()
+            except Exception as e:
+                if self.artifact_dir.exists():
+                    io.remove_directory(self.artifact_dir)
+                callback.force_finish()
+                callback.set_failed()
+                raise e
 
         def inner(callback: TrainCallback):
             try:
                 self.before_train(cfg)
                 self.on_train_start(cfg)
                 self.save_train_config(cfg)
                 self.training(cfg, callback)
@@ -447,16 +466,14 @@
         return callback
 
     # Inference Hook
     def get_model(self):
         raise NotImplementedError
 
     def before_inference(self, cfg: InferenceConfig):
-        self.check_train_sanity()
-
         # overwrite training config
         train_config = self.get_train_config()
         if cfg.image_size is None:
             cfg.image_size = train_config.image_size
         if cfg.letter_box is None:
             cfg.letter_box = train_config.letter_box
 
@@ -564,14 +581,29 @@
             except Exception as e:
                 if self.inference_dir.exists():
                     io.remove_directory(self.inference_dir)
                 callback.force_finish()
                 callback.set_failed()
                 raise e
 
+        def inner(callback):
+            try:
+                self.before_inference(cfg)
+                self.on_inference_start(cfg)
+                self.inferencing(cfg, callback)
+                self.on_inference_end(cfg)
+                self.after_inference(cfg)
+                callback.force_finish()
+            except Exception as e:
+                if self.inference_dir.exists():
+                    io.remove_directory(self.inference_dir)
+                callback.force_finish()
+                callback.set_failed()
+                raise e
+
         cfg = InferenceConfig(
             source=source,
             batch_size=batch_size,
             recursive=recursive,
             image_size=image_size,
             letter_box=letter_box,
             confidence_threshold=confidence_threshold,
@@ -595,15 +627,14 @@
             callback.register_thread(thread)
             callback.start()
 
         return callback
 
     # Export Hook
     def before_export(self, cfg: ExportConfig):
-        self.check_train_sanity()
 
         # overwrite training config
         train_config = self.get_train_config()
         if cfg.image_size is None:
             cfg.image_size = train_config.image_size
 
     def on_export_start(self, cfg: ExportConfig):
@@ -665,14 +696,15 @@
             hold (bool, optional): hold or not.
                 If True then it holds until task finished.
                 If False then return Inferece Callback and run in background. Defaults to True.
 
         Returns:
             ExportCallback: export callback
         """
+        self.check_train_sanity()
 
         def inner(callback):
             try:
                 self.before_export(cfg)
                 self.on_export_start(cfg)
                 self.exporting(cfg, callback)
                 self.on_export_end(cfg)
```

### Comparing `waffle_hub-0.1.7/waffle_hub/hub/model/wrapper.py` & `waffle_hub-0.1.8/waffle_hub/hub/model/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,16 @@
 """
 
 from typing import Union
 
 import torch
 from torchvision.ops import batched_nms
 
-from waffle_hub.schema.data import (
-    ClassificationResult,
-    ImageInfo,
-    ObjectDetectionResult,
-)
+from waffle_hub.schema.data import ImageInfo
+from waffle_hub.schema.fields import Annotation
 
 
 class PreprocessFunction:
     pass
 
 
 class PostprocessFunction:
@@ -38,28 +35,28 @@
 
     def __call__(
         self,
         results: list[torch.Tensor],
         image_infos: list[ImageInfo] = None,
         *args,
         **kwargs
-    ) -> list[ClassificationResult]:
+    ) -> list[Annotation]:
         parseds = []
 
         results = results[0]  # TODO: multi label
         scores, class_ids = results.cpu().topk(results.shape[1], dim=-1)
         results = torch.cat(
             [class_ids.unsqueeze(-1), scores.unsqueeze(-1)], dim=-1
         )
         for result in results:
             parsed = []
             for class_id, score in result:
                 parsed.append(
-                    ClassificationResult(
-                        category_id=int(class_id), score=float(score)
+                    Annotation.classification(
+                        category_id=int(class_id) + 1, score=float(score)
                     )
                 )
             parseds.append(parsed)
         return parseds
 
 
 class ObjectDetectionResultParser(ResultParser):
@@ -75,15 +72,15 @@
 
     def __call__(
         self,
         results: list[torch.Tensor],
         image_infos: list[ImageInfo],
         *args,
         **kwargs
-    ) -> list[ObjectDetectionResult]:
+    ) -> list[Annotation]:
         parseds = []
 
         bboxes_batch, confs_batch, class_ids_batch = results
         for bboxes, confs, class_ids, image_info in zip(
             bboxes_batch, confs_batch, class_ids_batch, image_infos
         ):
 
@@ -112,18 +109,18 @@
 
                 x1 = max(float((x1 * W - left_pad) / new_w * ori_w), 0)
                 y1 = max(float((y1 * H - top_pad) / new_h * ori_h), 0)
                 x2 = min(float((x2 * W - left_pad) / new_w * ori_w), ori_w)
                 y2 = min(float((y2 * H - top_pad) / new_h * ori_h), ori_h)
 
                 parsed.append(
-                    ObjectDetectionResult(
+                    Annotation.object_detection(
+                        category_id=int(class_id) + 1,
                         bbox=[x1, y1, x2 - x1, y2 - y1],
                         area=float((x2 - x1) * (y2 - y1)),
-                        category_id=int(class_id),
                         score=float(conf),
                     )
                 )
             parseds.append(parsed)
         return parseds
 
 
@@ -216,13 +213,12 @@
         if layer_names is None:
             layer_names = self.get_layer_names()[-1]
         elif isinstance(layer_names, str):
             layer_names = [layer_names]
 
         for name, module in self.model.named_modules():
             if name in layer_names:
-                print(name)
                 module.register_forward_hook(hook(name))
 
         x = self.forward(x)
 
         return x, feature_maps
```

### Comparing `waffle_hub-0.1.7/waffle_hub/run.py` & `waffle_hub-0.1.8/waffle_hub/run.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.7/waffle_hub/schema/base_schema.py` & `waffle_hub-0.1.8/waffle_hub/schema/base_schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import asdict, dataclass
+from pathlib import Path
 
 from waffle_utils.file import io
 
 
 @dataclass
 class BaseSchema:
     def __enter__(self):
@@ -18,9 +19,13 @@
         io.save_json(self.to_dict(), save_path, create_directory=True)
 
     def save_yaml(self, save_path):
         io.save_yaml(self.to_dict(), save_path, create_directory=True)
 
     @classmethod
     def load(cls, load_path):
-        config = io.load_yaml(load_path)
+        load_path = Path(load_path)
+        if load_path.suffix == ".json":
+            config = io.load_json(load_path)
+        elif load_path.suffix == ".yaml":
+            config = io.load_yaml(load_path)
         return cls(**config)
```

### Comparing `waffle_hub-0.1.7/waffle_hub/schema/configs.py` & `waffle_hub-0.1.8/waffle_hub/schema/configs.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.7/waffle_hub/utils/callback.py` & `waffle_hub-0.1.8/waffle_hub/utils/callback.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.7/waffle_hub/utils/data.py` & `waffle_hub-0.1.8/waffle_hub/utils/data.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.1.7/waffle_hub.egg-info/PKG-INFO` & `waffle_hub-0.1.8/waffle_hub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-hub
-Version: 0.1.7
+Version: 0.1.8
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle-hub Version: 0.1.7 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle-hub Version: 0.1.8 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

### Comparing `waffle_hub-0.1.7/waffle_hub.egg-info/SOURCES.txt` & `waffle_hub-0.1.8/waffle_hub.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
+tests/test_dataset.py
 tests/test_hub.py
 waffle_hub/__init__.py
 waffle_hub/run.py
 waffle_hub.egg-info/PKG-INFO
 waffle_hub.egg-info/SOURCES.txt
 waffle_hub.egg-info/dependency_links.txt
 waffle_hub.egg-info/entry_points.txt
 waffle_hub.egg-info/requires.txt
 waffle_hub.egg-info/top_level.txt
+waffle_hub/dataset/__init__.py
+waffle_hub/dataset/dataset.py
+waffle_hub/dataset/adapter/__init__.py
+waffle_hub/dataset/adapter/coco.py
+waffle_hub/dataset/adapter/yolo.py
 waffle_hub/experimental/__init__.py
 waffle_hub/experimental/serve.py
+waffle_hub/experimental/auto_label/__init__.py
+waffle_hub/experimental/auto_label/grounding_dino.py
 waffle_hub/hub/__init__.py
 waffle_hub/hub/base_hub.py
 waffle_hub/hub/adapter/__init__.py
 waffle_hub/hub/adapter/tx_model/__init__.py
 waffle_hub/hub/adapter/tx_model/tx_model_hub.py
 waffle_hub/hub/adapter/tx_model/configs/__init__.py
 waffle_hub/hub/adapter/tx_model/configs/data_cfg.py
@@ -26,11 +34,16 @@
 waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
 waffle_hub/hub/model/__init__.py
 waffle_hub/hub/model/wrapper.py
 waffle_hub/schema/__init__.py
 waffle_hub/schema/base_schema.py
 waffle_hub/schema/configs.py
 waffle_hub/schema/data.py
+waffle_hub/schema/fields/__init__.py
+waffle_hub/schema/fields/annotation.py
+waffle_hub/schema/fields/base_field.py
+waffle_hub/schema/fields/category.py
+waffle_hub/schema/fields/image.py
 waffle_hub/utils/__init__.py
 waffle_hub/utils/callback.py
 waffle_hub/utils/data.py
 waffle_hub/utils/draw.py
```

