# Comparing `tmp/orthoseg-0.4.1b4.tar.gz` & `tmp/orthoseg-0.4.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orthoseg-0.4.1b4.tar", last modified: Thu Dec  8 17:00:52 2022, max compression
+gzip compressed data, was "orthoseg-0.4.2a1.tar", last modified: Tue Apr 18 08:54:13 2023, max compression
```

## Comparing `orthoseg-0.4.1b4.tar` & `orthoseg-0.4.2a1.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxrwxrwx   0        0        0        0 2022-12-08 17:00:52.811748 orthoseg-0.4.1b4/
--rw-rw-rw-   0        0        0    35823 2022-11-01 21:06:33.000000 orthoseg-0.4.1b4/LICENSE.MD
--rw-rw-rw-   0        0        0      111 2022-12-06 08:41:37.000000 orthoseg-0.4.1b4/MANIFEST.in
--rw-rw-rw-   0        0        0     1232 2022-12-08 17:00:52.811748 orthoseg-0.4.1b4/PKG-INFO
--rw-rw-rw-   0        0        0      808 2022-11-10 10:57:18.000000 orthoseg-0.4.1b4/README.md
-drwxrwxrwx   0        0        0        0 2022-12-08 17:00:52.642020 orthoseg-0.4.1b4/orthoseg/
--rw-rw-rw-   0        0        0      498 2022-12-06 08:41:37.000000 orthoseg-0.4.1b4/orthoseg/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-08 17:00:52.690367 orthoseg-0.4.1b4/orthoseg/helpers/
--rw-rw-rw-   0        0        0        0 2022-01-27 13:51:38.000000 orthoseg-0.4.1b4/orthoseg/helpers/__init__.py
--rw-rw-rw-   0        0        0     8979 2022-08-24 20:36:50.000000 orthoseg-0.4.1b4/orthoseg/helpers/config_helper.py
--rw-rw-rw-   0        0        0     2302 2022-11-22 17:31:16.000000 orthoseg-0.4.1b4/orthoseg/helpers/email_helper.py
--rw-rw-rw-   0        0        0     3888 2022-08-22 18:56:49.000000 orthoseg-0.4.1b4/orthoseg/helpers/progress_helper.py
--rw-rw-rw-   0        0        0     2817 2022-12-08 16:56:35.000000 orthoseg-0.4.1b4/orthoseg/helpers/vectorfile_helper.py
-drwxrwxrwx   0        0        0        0 2022-12-08 17:00:52.718496 orthoseg-0.4.1b4/orthoseg/lib/
--rw-rw-rw-   0        0        0        0 2022-01-27 13:51:38.000000 orthoseg-0.4.1b4/orthoseg/lib/__init__.py
--rw-rw-rw-   0        0        0    38210 2022-12-08 16:56:35.000000 orthoseg-0.4.1b4/orthoseg/lib/postprocess_predictions.py
--rw-rw-rw-   0        0        0    27806 2022-12-06 16:33:36.000000 orthoseg-0.4.1b4/orthoseg/lib/predicter.py
--rw-rw-rw-   0        0        0    33501 2022-12-02 09:52:36.000000 orthoseg-0.4.1b4/orthoseg/lib/prepare_traindatasets.py
--rw-rw-rw-   0        0        0    25661 2022-12-06 08:41:37.000000 orthoseg-0.4.1b4/orthoseg/lib/trainer.py
--rw-rw-rw-   0        0        0     6899 2022-08-22 18:56:49.000000 orthoseg-0.4.1b4/orthoseg/load_images.py
--rw-rw-rw-   0        0        0     4054 2022-12-06 08:41:37.000000 orthoseg-0.4.1b4/orthoseg/load_sampleprojects.py
-drwxrwxrwx   0        0        0        0 2022-12-08 17:00:52.733456 orthoseg-0.4.1b4/orthoseg/model/
--rw-rw-rw-   0        0        0        0 2022-01-27 13:51:38.000000 orthoseg-0.4.1b4/orthoseg/model/__init__.py
--rw-rw-rw-   0        0        0    18952 2022-12-06 08:41:37.000000 orthoseg-0.4.1b4/orthoseg/model/model_factory.py
--rw-rw-rw-   0        0        0    33034 2022-09-23 11:12:51.000000 orthoseg-0.4.1b4/orthoseg/model/model_helper.py
--rw-rw-rw-   0        0        0     6180 2022-12-08 00:31:41.000000 orthoseg-0.4.1b4/orthoseg/postprocess.py
--rw-rw-rw-   0        0        0    12305 2022-12-06 16:37:31.000000 orthoseg-0.4.1b4/orthoseg/predict.py
--rw-rw-rw-   0        0        0    18730 2022-12-08 00:31:41.000000 orthoseg-0.4.1b4/orthoseg/project_defaults.ini
--rw-rw-rw-   0        0        0     6083 2022-08-22 18:56:49.000000 orthoseg-0.4.1b4/orthoseg/scriptrunner.py
--rw-rw-rw-   0        0        0     2718 2022-01-27 13:51:38.000000 orthoseg-0.4.1b4/orthoseg/scriptrunner_defaults.ini
--rw-rw-rw-   0        0        0    24067 2022-12-02 09:52:36.000000 orthoseg-0.4.1b4/orthoseg/train.py
-drwxrwxrwx   0        0        0        0 2022-12-08 17:00:52.769224 orthoseg-0.4.1b4/orthoseg/util/
--rw-rw-rw-   0        0        0        0 2022-01-27 13:51:38.000000 orthoseg-0.4.1b4/orthoseg/util/__init__.py
--rw-rw-rw-   0        0        0     5126 2022-08-22 18:56:49.000000 orthoseg-0.4.1b4/orthoseg/util/config_util.py
--rw-rw-rw-   0        0        0     2160 2022-11-08 10:05:55.000000 orthoseg-0.4.1b4/orthoseg/util/gdrive_util.py
--rw-rw-rw-   0        0        0     4711 2022-08-22 18:56:49.000000 orthoseg-0.4.1b4/orthoseg/util/general_util.py
--rw-rw-rw-   0        0        0     4186 2022-12-06 08:41:37.000000 orthoseg-0.4.1b4/orthoseg/util/git_downloader.py
--rw-rw-rw-   0        0        0     6359 2022-08-22 18:56:49.000000 orthoseg-0.4.1b4/orthoseg/util/log_util.py
--rw-rw-rw-   0        0        0    46301 2022-12-02 09:56:00.000000 orthoseg-0.4.1b4/orthoseg/util/ows_util.py
--rw-rw-rw-   0        0        0    15608 2022-12-08 16:56:35.000000 orthoseg-0.4.1b4/orthoseg/util/vector_util.py
--rw-rw-rw-   0        0        0        7 2022-12-08 16:57:31.000000 orthoseg-0.4.1b4/orthoseg/version.txt
-drwxrwxrwx   0        0        0        0 2022-12-08 17:00:52.675407 orthoseg-0.4.1b4/orthoseg.egg-info/
--rw-rw-rw-   0        0        0     1232 2022-12-08 17:00:52.000000 orthoseg-0.4.1b4/orthoseg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1451 2022-12-08 17:00:52.000000 orthoseg-0.4.1b4/orthoseg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-08 17:00:52.000000 orthoseg-0.4.1b4/orthoseg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      303 2022-12-08 17:00:52.000000 orthoseg-0.4.1b4/orthoseg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      132 2022-12-08 17:00:52.000000 orthoseg-0.4.1b4/orthoseg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-12-08 17:00:52.000000 orthoseg-0.4.1b4/orthoseg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      104 2022-12-08 17:00:52.828513 orthoseg-0.4.1b4/setup.cfg
--rw-rw-rw-   0        0        0     1469 2022-12-06 08:41:37.000000 orthoseg-0.4.1b4/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-08 17:00:52.811748 orthoseg-0.4.1b4/tests/
--rw-rw-rw-   0        0        0        0 2022-08-22 18:56:49.000000 orthoseg-0.4.1b4/tests/__init__.py
--rw-rw-rw-   0        0        0     6879 2022-12-06 08:41:37.000000 orthoseg-0.4.1b4/tests/test_end2end.py
--rw-rw-rw-   0        0        0     3598 2022-12-06 08:41:37.000000 orthoseg-0.4.1b4/tests/test_helper.py
--rw-rw-rw-   0        0        0     1664 2022-12-06 08:41:37.000000 orthoseg-0.4.1b4/tests/test_load_sampleprojects.py
--rw-rw-rw-   0        0        0     2767 2022-12-06 08:41:37.000000 orthoseg-0.4.1b4/tests/test_model_factory.py
--rw-rw-rw-   0        0        0     5572 2022-11-14 14:38:51.000000 orthoseg-0.4.1b4/tests/test_ows_util.py
--rw-rw-rw-   0        0        0     2361 2022-11-22 14:10:08.000000 orthoseg-0.4.1b4/tests/test_postprocess_predictions.py
--rw-rw-rw-   0        0        0    11276 2022-12-06 08:41:37.000000 orthoseg-0.4.1b4/tests/test_prepare_traindata.py
--rw-rw-rw-   0        0        0      679 2022-09-20 18:54:20.000000 orthoseg-0.4.1b4/tests/test_train.py
--rw-rw-rw-   0        0        0    16057 2022-12-08 16:56:35.000000 orthoseg-0.4.1b4/tests/test_vector_util.py
--rw-rw-rw-   0        0        0     3505 2022-12-08 00:31:41.000000 orthoseg-0.4.1b4/tests/test_vectorfile_helper.py
--rw-rw-rw-   0        0        0      382 2022-12-06 08:41:37.000000 orthoseg-0.4.1b4/tests/test_version.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.658429 orthoseg-0.4.2a1/
+-rw-rw-rw-   0        0        0    35823 2022-11-01 21:06:33.000000 orthoseg-0.4.2a1/LICENSE.MD
+-rw-rw-rw-   0        0        0      111 2022-12-06 08:41:37.000000 orthoseg-0.4.2a1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1232 2023-04-18 08:54:13.658429 orthoseg-0.4.2a1/PKG-INFO
+-rw-rw-rw-   0        0        0      808 2022-11-10 10:57:18.000000 orthoseg-0.4.2a1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.455407 orthoseg-0.4.2a1/orthoseg/
+-rw-rw-rw-   0        0        0      498 2022-12-06 08:41:37.000000 orthoseg-0.4.2a1/orthoseg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.502271 orthoseg-0.4.2a1/orthoseg/helpers/
+-rw-rw-rw-   0        0        0        0 2022-01-27 13:51:38.000000 orthoseg-0.4.2a1/orthoseg/helpers/__init__.py
+-rw-rw-rw-   0        0        0     9473 2023-04-11 12:35:06.000000 orthoseg-0.4.2a1/orthoseg/helpers/config_helper.py
+-rw-rw-rw-   0        0        0     2302 2022-11-22 17:31:16.000000 orthoseg-0.4.2a1/orthoseg/helpers/email_helper.py
+-rw-rw-rw-   0        0        0     2817 2022-12-08 16:56:35.000000 orthoseg-0.4.2a1/orthoseg/helpers/vectorfile_helper.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.533311 orthoseg-0.4.2a1/orthoseg/lib/
+-rw-rw-rw-   0        0        0        0 2022-01-27 13:51:38.000000 orthoseg-0.4.2a1/orthoseg/lib/__init__.py
+-rw-rw-rw-   0        0        0    38210 2022-12-08 16:56:35.000000 orthoseg-0.4.2a1/orthoseg/lib/postprocess_predictions.py
+-rw-rw-rw-   0        0        0    27801 2023-04-13 08:01:36.000000 orthoseg-0.4.2a1/orthoseg/lib/predicter.py
+-rw-rw-rw-   0        0        0    33489 2023-04-13 08:01:36.000000 orthoseg-0.4.2a1/orthoseg/lib/prepare_traindatasets.py
+-rw-rw-rw-   0        0        0    25661 2022-12-06 08:41:37.000000 orthoseg-0.4.2a1/orthoseg/lib/trainer.py
+-rw-rw-rw-   0        0        0     6799 2023-04-12 12:57:54.000000 orthoseg-0.4.2a1/orthoseg/load_images.py
+-rw-rw-rw-   0        0        0     4185 2023-04-17 12:18:35.000000 orthoseg-0.4.2a1/orthoseg/load_sampleprojects.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.549165 orthoseg-0.4.2a1/orthoseg/model/
+-rw-rw-rw-   0        0        0        0 2022-01-27 13:51:38.000000 orthoseg-0.4.2a1/orthoseg/model/__init__.py
+-rw-rw-rw-   0        0        0    18952 2022-12-09 22:17:37.000000 orthoseg-0.4.2a1/orthoseg/model/model_factory.py
+-rw-rw-rw-   0        0        0    33034 2022-09-23 11:12:51.000000 orthoseg-0.4.2a1/orthoseg/model/model_helper.py
+-rw-rw-rw-   0        0        0     6180 2022-12-08 00:31:41.000000 orthoseg-0.4.2a1/orthoseg/postprocess.py
+-rw-rw-rw-   0        0        0    12305 2022-12-06 16:37:31.000000 orthoseg-0.4.2a1/orthoseg/predict.py
+-rw-rw-rw-   0        0        0    18730 2022-12-10 13:45:38.000000 orthoseg-0.4.2a1/orthoseg/project_defaults.ini
+-rw-rw-rw-   0        0        0     6083 2022-08-22 18:56:49.000000 orthoseg-0.4.2a1/orthoseg/scriptrunner.py
+-rw-rw-rw-   0        0        0     2718 2022-01-27 13:51:38.000000 orthoseg-0.4.2a1/orthoseg/scriptrunner_defaults.ini
+-rw-rw-rw-   0        0        0    24067 2022-12-02 09:52:36.000000 orthoseg-0.4.2a1/orthoseg/train.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.595847 orthoseg-0.4.2a1/orthoseg/util/
+-rw-rw-rw-   0        0        0        0 2022-01-27 13:51:38.000000 orthoseg-0.4.2a1/orthoseg/util/__init__.py
+-rw-rw-rw-   0        0        0     5126 2022-08-22 18:56:49.000000 orthoseg-0.4.2a1/orthoseg/util/config_util.py
+-rw-rw-rw-   0        0        0     4711 2022-08-22 18:56:49.000000 orthoseg-0.4.2a1/orthoseg/util/general_util.py
+-rw-rw-rw-   0        0        0     4675 2023-02-23 21:56:59.000000 orthoseg-0.4.2a1/orthoseg/util/git_downloader.py
+-rw-rw-rw-   0        0        0     6359 2022-08-22 18:56:49.000000 orthoseg-0.4.2a1/orthoseg/util/log_util.py
+-rw-rw-rw-   0        0        0    40677 2023-04-13 08:01:36.000000 orthoseg-0.4.2a1/orthoseg/util/ows_util.py
+-rw-rw-rw-   0        0        0     3434 2023-04-13 08:01:36.000000 orthoseg-0.4.2a1/orthoseg/util/progress_util.py
+-rw-rw-rw-   0        0        0    15608 2022-12-08 16:56:35.000000 orthoseg-0.4.2a1/orthoseg/util/vector_util.py
+-rw-rw-rw-   0        0        0        7 2023-04-18 08:53:48.000000 orthoseg-0.4.2a1/orthoseg/version.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.486645 orthoseg-0.4.2a1/orthoseg.egg-info/
+-rw-rw-rw-   0        0        0     1232 2023-04-18 08:54:13.000000 orthoseg-0.4.2a1/orthoseg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1417 2023-04-18 08:54:13.000000 orthoseg-0.4.2a1/orthoseg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 08:54:13.000000 orthoseg-0.4.2a1/orthoseg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      303 2023-04-18 08:54:13.000000 orthoseg-0.4.2a1/orthoseg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      139 2023-04-18 08:54:13.000000 orthoseg-0.4.2a1/orthoseg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 08:54:13.000000 orthoseg-0.4.2a1/orthoseg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      104 2023-04-18 08:54:13.658429 orthoseg-0.4.2a1/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2023-04-17 12:18:35.000000 orthoseg-0.4.2a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:54:13.658429 orthoseg-0.4.2a1/tests/
+-rw-rw-rw-   0        0        0        0 2022-08-22 18:56:49.000000 orthoseg-0.4.2a1/tests/__init__.py
+-rw-rw-rw-   0        0        0     7212 2023-04-17 12:18:35.000000 orthoseg-0.4.2a1/tests/test_end2end.py
+-rw-rw-rw-   0        0        0     3598 2022-12-06 08:41:37.000000 orthoseg-0.4.2a1/tests/test_helper.py
+-rw-rw-rw-   0        0        0     2203 2023-04-17 12:18:35.000000 orthoseg-0.4.2a1/tests/test_load_sampleprojects.py
+-rw-rw-rw-   0        0        0     2767 2022-12-06 08:41:37.000000 orthoseg-0.4.2a1/tests/test_model_factory.py
+-rw-rw-rw-   0        0        0     5572 2022-11-14 14:38:51.000000 orthoseg-0.4.2a1/tests/test_ows_util.py
+-rw-rw-rw-   0        0        0     2361 2022-11-22 14:10:08.000000 orthoseg-0.4.2a1/tests/test_postprocess_predictions.py
+-rw-rw-rw-   0        0        0    11276 2022-12-06 08:41:37.000000 orthoseg-0.4.2a1/tests/test_prepare_traindata.py
+-rw-rw-rw-   0        0        0      679 2022-09-20 18:54:20.000000 orthoseg-0.4.2a1/tests/test_train.py
+-rw-rw-rw-   0        0        0    16067 2023-01-20 22:38:51.000000 orthoseg-0.4.2a1/tests/test_vector_util.py
+-rw-rw-rw-   0        0        0     3505 2022-12-08 00:31:41.000000 orthoseg-0.4.2a1/tests/test_vectorfile_helper.py
+-rw-rw-rw-   0        0        0      382 2022-12-06 08:41:37.000000 orthoseg-0.4.2a1/tests/test_version.py
```

### Comparing `orthoseg-0.4.1b4/LICENSE.MD` & `orthoseg-0.4.2a1/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/PKG-INFO` & `orthoseg-0.4.2a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthoseg
-Version: 0.4.1b4
+Version: 0.4.2a1
 Summary: Package to make it easier to segment orthophotos.
 Home-page: https://github.com/orthoseg/orthoseg
 Author: Pieter Roggemans
 Author-email: pieter.roggemans@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `orthoseg-0.4.1b4/README.md` & `orthoseg-0.4.2a1/README.md`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/helpers/config_helper.py` & `orthoseg-0.4.2a1/orthoseg/helpers/config_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,24 +136,34 @@
 
             # Give default values to some optional properties of a server
             for layersource in image_layers[image_layer]["layersources"]:
                 if "random_sleep" not in layersource:
                     layersource["random_sleep"] = 0
                 if "wms_ignore_capabilities_url" not in layersource:
                     layersource["wms_ignore_capabilities_url"] = False
+                if "wms_username" not in layersource:
+                    layersource["wms_username"] = None
+                if "wms_password" not in layersource:
+                    layersource["wms_password"] = None
 
         else:
             # If not, the layersource should be specified in seperate parameters
             layersource = {}
             layersource["wms_server_url"] = layer_config[image_layer].get(
                 "wms_server_url"
             )
             layersource["wms_version"] = layer_config[image_layer].get(
                 "wms_version", fallback="1.3.0"
             )
+            layersource["wms_username"] = layer_config[image_layer].get(
+                "wms_username", fallback=None
+            )
+            layersource["wms_password"] = layer_config[image_layer].get(
+                "wms_password", fallback=None
+            )
             # The layer names and layer styles are lists
             layersource["layernames"] = layer_config[image_layer].getlist(
                 "wms_layernames"
             )
             layersource["layerstyles"] = layer_config[image_layer].getlist(
                 "wms_layerstyles"
             )
```

### Comparing `orthoseg-0.4.1b4/orthoseg/helpers/email_helper.py` & `orthoseg-0.4.2a1/orthoseg/helpers/email_helper.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/helpers/progress_helper.py` & `orthoseg-0.4.2a1/orthoseg/util/progress_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 # -*- coding: utf-8 -*-
 """
-Module with specific helper functions to manage progress reporting.
+Module with functions to manage progress logging.
 """
 
 import datetime
 import logging
 from typing import Optional
 
-# -------------------------------------------------------------
-# First define/init general variables/constants
-# -------------------------------------------------------------
 # Get a logger...
 logger = logging.getLogger(__name__)
 
-# -------------------------------------------------------------
-# The real work
-# -------------------------------------------------------------
 
-
-class ProgressHelper:
+class ProgressLogger:
     first_reporting_done = False
 
     def __init__(
         self,
         message: str,
         nb_steps_total: int,
         nb_steps_done: int = 0,
@@ -91,12 +84,7 @@
                 )
             logger.info(progress_message)
 
             self.start_time_lastreporting = time_now
             self.nb_steps_done_lastreporting = self.nb_steps_done
             if self.first_reporting_done is False:
                 self.first_reporting_done = True
-
-
-# If the script is ran directly...
-if __name__ == "__main__":
-    raise Exception("Not implemented")
```

### Comparing `orthoseg-0.4.1b4/orthoseg/helpers/vectorfile_helper.py` & `orthoseg-0.4.2a1/orthoseg/helpers/vectorfile_helper.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/lib/postprocess_predictions.py` & `orthoseg-0.4.2a1/orthoseg/lib/postprocess_predictions.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/lib/predicter.py` & `orthoseg-0.4.2a1/orthoseg/lib/predicter.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import rasterio as rio
 import rasterio.crs as rio_crs
 import rasterio.plot as rio_plot
 import tensorflow as tf
 import keras.models
 
 import orthoseg.lib.postprocess_predictions as postp
-from orthoseg.helpers.progress_helper import ProgressHelper
+from orthoseg.util.progress_util import ProgressLogger
 from orthoseg.util import general_util
 
 # -------------------------------------------------------------
 # First define/init some general variables/constants
 # -------------------------------------------------------------
 # Get a logger...
 logger = logging.getLogger(__name__)
@@ -509,15 +509,15 @@
                 if len(perfinfo) > 0:
                     logger.debug(perfinfo)
                 if progress is not None:
                     progress.step(nb_steps=batch_size)
                 # Init progress only when some imags were already processed, as the
                 # first are very slow.
                 if progress is None and nb_processed > 0:
-                    progress = ProgressHelper(
+                    progress = ProgressLogger(
                         message=f"predict to {output_image_dir.parent.name}/{output_image_dir.name}",  # noqa: E501
                         nb_steps_total=nb_to_process,
                         nb_steps_done=batch_size,
                     )
 
                 # If max number errors reached, stop processings
                 if max_prediction_errors >= 0 and nb_errors >= max_prediction_errors:
```

### Comparing `orthoseg-0.4.1b4/orthoseg/lib/prepare_traindatasets.py` & `orthoseg-0.4.2a1/orthoseg/lib/prepare_traindatasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from PIL import Image
 import pygeos
 import rasterio as rio
 import rasterio.features as rio_features
 import rasterio.profiles as rio_profiles
 import shapely.geometry as sh_geom
 
-from orthoseg.helpers.progress_helper import ProgressHelper
+from orthoseg.util.progress_util import ProgressLogger
 from orthoseg.util import ows_util
 from orthoseg.util import vector_util
 
 # -------------------------------------------------------------
 # First define/init some general variables/constants
 # -------------------------------------------------------------
 # Get a logger...
@@ -252,15 +252,15 @@
     traindata_types = ["train", "validation", "test"]
     nb_todo = 0
     for labellocations_gdf, _ in labeldata:
         labellocations_curr_gdf = labellocations_gdf[
             labellocations_gdf["traindata_type"].isin(traindata_types)
         ]
         nb_todo += len(labellocations_curr_gdf)
-    progress = ProgressHelper(message="prepare training images", nb_steps_total=nb_todo)
+    progress = ProgressLogger(message="prepare training images", nb_steps_total=nb_todo)
     logger.info(f"Get images for {nb_todo} labels")
 
     for traindata_type in traindata_types:
         # Create output dirs...
         output_imagedatatype_dir = output_tmp_dir / traindata_type
         output_imagedata_image_dir = output_imagedatatype_dir / "image"
         output_imagedata_mask_dir = output_imagedatatype_dir / "mask"
@@ -466,15 +466,15 @@
             image_pixel_width * image_pixel_x_size
         )  # tile width in units of crs => 500 m
         image_crs_height = math.fabs(
             image_pixel_height * image_pixel_y_size
         )  # tile height in units of crs => 500 m
         locations_none = []
         for location in labellocations_gdf.itertuples():
-            if location.geometry is None or len(location.geometry.bounds) < 4:
+            if location.geometry is None or location.geometry.is_empty:
                 logger.warning(
                     f"No or empty geometry found in file {Path(location.path).name} "
                     f"for index {location.Index}, it will be ignored"
                 )
                 locations_none.append(location.Index)
                 continue
```

### Comparing `orthoseg-0.4.1b4/orthoseg/lib/trainer.py` & `orthoseg-0.4.2a1/orthoseg/lib/trainer.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/load_images.py` & `orthoseg-0.4.2a1/orthoseg/load_images.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,30 +104,28 @@
             image_pixel_height = conf.train.getint("image_pixel_height")
             image_pixel_x_size = conf.train.getfloat("image_pixel_x_size")
             image_pixel_y_size = conf.train.getfloat("image_pixel_y_size")
             image_pixels_overlap = 0
             image_format = ows_util.FORMAT_JPEG
 
             # To create the testsample, fetch only on every ... images
-            column_start = 1
             nb_images_to_skip = 50
 
         else:
             output_image_dir = conf.dirs.getpath("predict_image_input_dir")
 
             # Get the image size for the predict
             image_pixel_width = conf.predict.getint("image_pixel_width")
             image_pixel_height = conf.predict.getint("image_pixel_height")
             image_pixel_x_size = conf.predict.getfloat("image_pixel_x_size")
             image_pixel_y_size = conf.predict.getfloat("image_pixel_y_size")
             image_pixels_overlap = conf.predict.getint("image_pixels_overlap")
             image_format = ows_util.FORMAT_JPEG
 
             # For the real prediction dataset, no skipping obviously...
-            column_start = 0
             nb_images_to_skip = 0
 
         # Get ssl_verify setting
         ssl_verify = conf.general["ssl_verify"]
         # Get the download cron schedule
         download_cron_schedule = conf.download["cron_schedule"]
 
@@ -158,15 +156,14 @@
             image_pixel_width=image_pixel_width,
             image_pixel_height=image_pixel_height,
             image_pixels_ignore_border=image_pixels_ignore_border,
             nb_concurrent_calls=nb_concurrent_calls,
             cron_schedule=download_cron_schedule,
             image_format=image_format,
             pixels_overlap=image_pixels_overlap,
-            column_start=column_start,
             nb_images_to_skip=nb_images_to_skip,
             ssl_verify=ssl_verify,
         )
 
         # Log and send mail
         message = f"Completed load_images for config {config_path.stem}"
         logger.info(message)
```

### Comparing `orthoseg-0.4.1b4/orthoseg/load_sampleprojects.py` & `orthoseg-0.4.2a1/orthoseg/load_sampleprojects.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 """
 
 import argparse
 import logging
 from pathlib import Path
 import shlex
 import sys
+from typing import Optional
+
+import gdown
 
 # orthoseg is higher in dir hierarchy, add root to sys.path
 sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
-from orthoseg.util import gdrive_util
 from orthoseg.util import git_downloader
 
 
 # -------------------------------------------------------------
 # First define/init general variables/constants
 # -------------------------------------------------------------
 # Get a logger...
@@ -58,51 +60,53 @@
     dest_dir = Path(args.dest_dir).expanduser() / "orthoseg"
     ssl_verify = args.ssl_verify
 
     # Return arguments
     return {"dest_dir": dest_dir, "ssl_verify": ssl_verify}
 
 
-def load_sampleprojects(dest_dir: Path, ssl_verify: bool):
+def load_sampleprojects(dest_dir: Path, ssl_verify: Optional[bool] = None):
     dest_dir_full = dest_dir / "sample_projects"
     if dest_dir_full.exists():
         raise Exception(f"Destination directory already exists: {dest_dir_full}")
 
     # Download
     print(f"Start download of sample projects to {str(dest_dir_full)}")
     git_downloader.download(
         repo_url="https://github.com/orthoseg/orthoseg/tree/master/sample_projects",
         output_dir=dest_dir,
         ssl_verify=ssl_verify,
     )
     print("Download finished")
     print("Start download of footballfields pretrained neural net")
+    verify = True if ssl_verify is None else ssl_verify
     footballfields_model_dir = dest_dir_full / "footballfields/models"
+    footballfields_model_dir.mkdir(parents=True, exist_ok=True)
     model_hdf5_path = footballfields_model_dir / "footballfields_01_0.92512_242.hdf5"
     if model_hdf5_path.exists() is False:
-        gdrive_util.download_file(
-            "1XmAenCW6K_RVwqC6xbkapJ5ws-f7-QgH",
-            model_hdf5_path,
-            ssl_verify=ssl_verify,
+        gdown.download(
+            id="1XmAenCW6K_RVwqC6xbkapJ5ws-f7-QgH",
+            output=str(model_hdf5_path),
+            verify=verify,
         )
     model_hyperparams_path = (
         footballfields_model_dir / "footballfields_01_hyperparams.json"
     )
     if model_hyperparams_path.exists() is False:
-        gdrive_util.download_file(
-            "1umxcd4RkB81sem9PdIpLoWeiIW8ga1u7",
-            model_hyperparams_path,
-            ssl_verify=ssl_verify,
+        gdown.download(
+            id="1umxcd4RkB81sem9PdIpLoWeiIW8ga1u7",
+            output=str(model_hyperparams_path),
+            verify=verify
         )
     model_modeljson_path = footballfields_model_dir / "footballfields_01_model.json"
     if model_modeljson_path.exists() is False:
-        gdrive_util.download_file(
-            "16qe8thBTrO3dFfLMU1T22gWcfHVXt8zQ",
-            model_modeljson_path,
-            ssl_verify=ssl_verify,
+        gdown.download(
+            id="16qe8thBTrO3dFfLMU1T22gWcfHVXt8zQ",
+            output=str(model_modeljson_path),
+            verify=verify
         )
     print("Download finished")
 
 
 def main():
     try:
         parsed_args = parse_load_sampleprojects_args(sys.argv[1:])
```

### Comparing `orthoseg-0.4.1b4/orthoseg/model/model_factory.py` & `orthoseg-0.4.2a1/orthoseg/model/model_factory.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/model/model_helper.py` & `orthoseg-0.4.2a1/orthoseg/model/model_helper.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/postprocess.py` & `orthoseg-0.4.2a1/orthoseg/postprocess.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/predict.py` & `orthoseg-0.4.2a1/orthoseg/predict.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/project_defaults.ini` & `orthoseg-0.4.2a1/orthoseg/project_defaults.ini`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/scriptrunner.py` & `orthoseg-0.4.2a1/orthoseg/scriptrunner.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/scriptrunner_defaults.ini` & `orthoseg-0.4.2a1/orthoseg/scriptrunner_defaults.ini`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/train.py` & `orthoseg-0.4.2a1/orthoseg/train.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/util/config_util.py` & `orthoseg-0.4.2a1/orthoseg/util/config_util.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/util/general_util.py` & `orthoseg-0.4.2a1/orthoseg/util/general_util.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/util/git_downloader.py` & `orthoseg-0.4.2a1/orthoseg/util/git_downloader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/python3
 # Based on https://github.com/sdushantha/gitdir/blob/master/gitdir/gitdir.py
 
 import re
 import os
 import ssl
+import time
 from typing import Union
 import urllib.request
 import json
 from pathlib import Path
 
 
 def create_url(url):
@@ -29,28 +30,34 @@
         api_url = re.sub(r"/tree/.*?/", "/contents/", api_url)
 
     api_url = api_url + "?ref=" + branch
     return api_url, download_dirs
 
 
 def download(
-    repo_url: str, output_dir: Path, ssl_verify: Union[bool, str, None] = None
+    repo_url: str,
+    output_dir: Path,
+    ssl_verify: Union[bool, str, None] = None,
+    limit_rate: bool = True,
 ):
     """
     Downloads the files and directories in repo_url.
 
     Args
         repo_url (str): url to the repository to download.
         output_dir (Path): directory to download the repository to.
         ssl_verify (bool or str, optional): True or None to use the default
             certificate bundle as installed on your system. False disables
             certificate validation (NOT recommended!). If a path to a
             certificate bundle file (.pem) is passed, this will be used.
             In corporate networks using a proxy server this is often needed
             to evade CERTIFICATE_VERIFY_FAILED errors. Defaults to None.
+        limit_rate (bool, optional): If True, limit the rate requests are done to
+            github to the maximum level allowed for unauthenticated users.
+            Defaults to True.
     """
     context = None
     if ssl_verify is not None:
         # If it is a string, make sure it isn't actually a bool
         if isinstance(ssl_verify, str):
             if ssl_verify.lower() == "true":
                 context = None
@@ -60,54 +67,61 @@
                 context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
                 context.load_verify_locations(ssl_verify)
 
         if isinstance(ssl_verify, bool) and not ssl_verify:
             context = ssl._create_unverified_context()
             print("SSL VERIFICATION IS TURNED OFF!!!")
 
-    # generate the url which returns the JSON data
+    # Generate the url which returns the JSON data
     api_url, download_dirs = create_url(repo_url)
 
     # To handle file names.
     if len(download_dirs.split(".")) == 0:
         dir_out = output_dir / download_dirs
     else:
         dir_out = output_dir / "/".join(download_dirs.split("/")[0:-1])
 
     # Download the file
+    # If limit_rate enabled, always sleep 1 second before doing a request!
+    if limit_rate:
+        time.sleep(1)
     with urllib.request.urlopen(api_url, context=context) as u:
-        # make a directory with the name which is taken from
+        # Make a directory with the name which is taken from
         # the actual repo
         dir_out.mkdir(parents=True, exist_ok=True)
 
-        # total files count
+        # Total files count
         total_files = 0
         raw_data = u.read()
         data = json.loads(raw_data)
 
         # Get the total number of files
         total_files += len(data)
 
         # If the data is a file, download it as one.
         if isinstance(data, dict) and data["type"] == "file":
-            # download the file
+            # Download the file
+            if limit_rate:
+                time.sleep(1)
             with urllib.request.urlopen(
                 data["download_url"], context=context
             ) as u, open(dir_out / data["name"], "wb") as f:
                 f.write(u.read())
             return total_files
 
         # Loop over all files/dirs found
         for file in data:
             file_url = file["download_url"]
             path = output_dir / file["path"]
             os.makedirs(path.parent, exist_ok=True)
 
             # If it is a file, download it, if dir, start recursively
             if file_url is not None:
+                if limit_rate:
+                    time.sleep(1)
                 with urllib.request.urlopen(file_url, context=context) as u, open(
                     path, "wb"
                 ) as f:
                     f.write(u.read())
             else:
                 download(file["html_url"], output_dir)
```

### Comparing `orthoseg-0.4.1b4/orthoseg/util/log_util.py` & `orthoseg-0.4.2a1/orthoseg/util/log_util.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg/util/ows_util.py` & `orthoseg-0.4.2a1/orthoseg/util/ows_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 # -*- coding: utf-8 -*-
 """
 Module with generic usable utility functions to make some tasks using OWS services
 easier.
 """
 
 import concurrent.futures as futures
-import datetime
-import itertools as it
 import logging
 import math
 from pathlib import Path
 import random
 import time
 from typing import List, Optional, Tuple, Union
 import urllib3
 import warnings
 
 import numpy as np
 import geofileops as gfo
 import geofileops.util.grid_util
+import geopandas as gpd
 import owslib
 import owslib.wms
 import owslib.util
 import pycron
 import pyproj
 import rasterio as rio
 import rasterio.errors as rio_errors
 from rasterio import profiles as rio_profiles
 from rasterio import transform as rio_transform
 from rasterio import windows as rio_windows
-import geopandas as gpd
-import shapely.geometry as sh_geom
+
+from . import progress_util
 
 # -------------------------------------------------------------
 # First define/init some general variables/constants
 # -------------------------------------------------------------
 FORMAT_GEOTIFF = "image/geotiff"
 FORMAT_GEOTIFF_EXT = ".tif"
 FORMAT_GEOTIFF_EXT_WORLD = ".tfw"
@@ -76,15 +75,14 @@
     nb_concurrent_calls: int = 1,
     cron_schedule: Optional[str] = None,
     image_format: str = FORMAT_GEOTIFF,
     image_format_save: Optional[str] = None,
     tiff_compress: str = "lzw",
     transparent: bool = False,
     pixels_overlap: int = 0,
-    column_start: int = 0,
     nb_images_to_skip: int = 0,
     max_nb_images: int = -1,
     ssl_verify: Union[bool, str] = True,
     force: bool = False,
 ):
     """
     Loads all images in a grid from a WMS service.
@@ -114,15 +112,14 @@
         image_format (str, optional): The image format to get. Defaults to
             FORMAT_GEOTIFF.
         image_format_save (str, optional): The image format to save to.
             Defaults to None.
         tiff_compress (str, optional): [description]. Defaults to 'lzw'.
         transparent (bool, optional): [description]. Defaults to False.
         pixels_overlap (int, optional): [description]. Defaults to 0.
-        column_start (int, optional): [description]. Defaults to 0.
         nb_images_to_skip (int, optional): [description]. Defaults to 0.
         max_nb_images (int, optional): [description]. Defaults to -1.
         ssl_verify (bool or str, optional): True to use the default
             certificate bundle as installed on your system. False disables
             certificate validation (NOT recommended!). If a path to a
             certificate bundle file (.pem) is passed, this will be used.
             In corporate networks using a proxy server this is often needed
@@ -133,182 +130,103 @@
         Exception: [description]
     """
 
     # Init
     if image_format_save is None:
         image_format_save = image_format
 
-    # Interprete ssl_verify
-    auth = None
-    if ssl_verify is not None:
-        # If it is a string, make sure it isn't actually a bool
-        if isinstance(ssl_verify, str):
-            if ssl_verify.lower() == "true":
-                ssl_verify = True
-            elif ssl_verify.lower() == "false":
-                ssl_verify = False
-
-        assert isinstance(ssl_verify, bool)
-        auth = owslib.util.Authentication(verify=ssl_verify)
-        if ssl_verify is False:
-            urllib3.disable_warnings()
-            logger.warn("SSL VERIFICATION IS TURNED OFF!!!")
-
     crs_width = math.fabs(
         image_pixel_width * image_crs_pixel_x_size
     )  # tile width in units of crs => 500 m
     crs_height = math.fabs(
         image_pixel_height * image_crs_pixel_y_size
     )  # tile height in units of crs => 500 m
     if cron_schedule is not None and cron_schedule != "":
         logger.info(
             "A cron_schedule was specified, so the download will only proceed in the "
             f"specified time range: {cron_schedule}"
         )
 
     # Read the region of interest file if provided
+    grid_bounds = image_gen_bounds
     roi_gdf = None
     if image_gen_roi_filepath is not None:
         # Read roi
         logger.info(f"Read + optimize region of interest from {image_gen_roi_filepath}")
         roi_gdf = gpd.read_file(str(image_gen_roi_filepath))
 
-        # If the generate_window wasn't specified, calculate the bounds
-        # based on the roi (but make sure they fit the grid!)
-        if image_gen_bounds is None:
-            roi_bounds = roi_gdf.geometry.total_bounds
-            image_gen_bounds = (
-                roi_bounds[0] - ((roi_bounds[0] - grid_xmin) % crs_width),
-                roi_bounds[1] - ((roi_bounds[1] - grid_ymin) % crs_height),
-                roi_bounds[2] + (grid_xmin - ((roi_bounds[2] - grid_xmin) % crs_width)),
-                roi_bounds[3]
-                + (grid_ymin - ((roi_bounds[3] - grid_ymin) % crs_height)),
-            )
-            logger.debug(
-                f"roi_bounds: {roi_bounds}, image_gen_bounds: {image_gen_bounds}"
-            )
+        # If the generate_window not specified, use bounds of the roi
+        if grid_bounds is None:
+            grid_bounds = roi_gdf.geometry.total_bounds
 
     # If there is still no image_gen_bounds, stop.
-    if image_gen_bounds is None:
+    if grid_bounds is None:
         raise Exception(
             "Either image_gen_bounds or an image_gen_roi_filepath should be specified."
         )
 
-    # Check if the image_gen_bounds are compatible with the grid...
-    if (image_gen_bounds[0] - grid_xmin) % crs_width != 0:
-        xmin_new = image_gen_bounds[0] - ((image_gen_bounds[0] - grid_xmin) % crs_width)
-        logger.warning(
-            f"xmin {image_gen_bounds[0]} incompatible with grid, {xmin_new} used"
-        )
-        image_gen_bounds = (
-            xmin_new,
-            image_gen_bounds[1],
-            image_gen_bounds[2],
-            image_gen_bounds[3],
-        )
-    if (image_gen_bounds[1] - grid_ymin) % crs_height != 0:
-        ymin_new = image_gen_bounds[1] - (
-            (image_gen_bounds[1] - grid_ymin) % crs_height
-        )
-        logger.warning(
-            f"ymin {image_gen_bounds[1]} incompatible with grid, {ymin_new} used"
-        )
-        image_gen_bounds = (
-            image_gen_bounds[0],
-            ymin_new,
-            image_gen_bounds[2],
-            image_gen_bounds[3],
-        )
-    if (image_gen_bounds[2] - grid_xmin) % crs_width != 0:
+    # Make grid_bounds compatible with the grid
+    grid_bounds = list(grid_bounds)
+    if (grid_bounds[0] - grid_xmin) % crs_width != 0:
+        xmin_new = grid_bounds[0] - ((grid_bounds[0] - grid_xmin) % crs_width)
+        logger.warning(f"xmin {grid_bounds[0]} incompatible with grid, {xmin_new} used")
+        grid_bounds[0] = xmin_new
+    if (grid_bounds[1] - grid_ymin) % crs_height != 0:
+        ymin_new = grid_bounds[1] - ((grid_bounds[1] - grid_ymin) % crs_height)
+        logger.warning(f"ymin {grid_bounds[1]} incompatible with grid, {ymin_new} used")
+        grid_bounds[1] = ymin_new
+    if (grid_bounds[2] - grid_xmin) % crs_width != 0:
         xmax_new = (
-            image_gen_bounds[2]
-            + crs_width
-            - ((image_gen_bounds[2] - grid_xmin) % crs_width)
-        )
-        logger.warning(
-            f"xmax {image_gen_bounds[2]} incompatible with grid, {xmax_new} used"
-        )
-        image_gen_bounds = (
-            image_gen_bounds[0],
-            image_gen_bounds[1],
-            xmax_new,
-            image_gen_bounds[3],
+            grid_bounds[2] + crs_width - ((grid_bounds[2] - grid_xmin) % crs_width)
         )
-    if (image_gen_bounds[3] - grid_ymin) % crs_height != 0:
+        logger.warning(f"xmax {grid_bounds[2]} incompatible with grid, {xmax_new} used")
+        grid_bounds[2] = xmax_new
+    if (grid_bounds[3] - grid_ymin) % crs_height != 0:
         ymax_new = (
-            image_gen_bounds[3]
-            + crs_height
-            - ((image_gen_bounds[3] - grid_ymin) % crs_height)
-        )
-        logger.warning(
-            f"ymax {image_gen_bounds[3]} incompatible with grid, {ymax_new} used"
-        )
-        image_gen_bounds = (
-            image_gen_bounds[0],
-            image_gen_bounds[1],
-            image_gen_bounds[2],
-            ymax_new,
+            grid_bounds[3] + crs_height - ((grid_bounds[3] - grid_ymin) % crs_height)
         )
+        logger.warning(f"ymax {grid_bounds[3]} incompatible with grid, {ymax_new} used")
+        grid_bounds[3] = ymax_new
+    grid_bounds = tuple(grid_bounds)
 
     # Create the output dir if it doesn't exist yet
     output_image_dir.mkdir(parents=True, exist_ok=True)
 
-    # Write the cache image grid to file
-    grid_path = output_image_dir / "imagecache_grid.gpkg"
-    if not grid_path.exists():
-        grid_for_roi_gdf = geofileops.util.grid_util.create_grid3(
-            image_gen_bounds, width=crs_width, height=crs_height, crs=crs
-        )
-        gfo.to_file(grid_for_roi_gdf, grid_path)
-
-    # Calculate width and height...
-    dx = math.fabs(
-        image_gen_bounds[0] - image_gen_bounds[2]
-    )  # area width in units of crs
-    dy = math.fabs(
-        image_gen_bounds[1] - image_gen_bounds[3]
-    )  # area height in units of crs
-    cols = int(math.ceil(dx / crs_width)) + 1
-    rows = int(math.ceil(dy / crs_height)) + 1
+    # Create a grid of the images that need to be downloaded
+    tiles_to_download_gdf = geofileops.util.grid_util.create_grid3(
+        grid_bounds, width=crs_width, height=crs_height, crs=crs
+    )
 
-    # If an roi is defined, split it using a grid as large objects are small
+    # If an roi is defined, filter the split it using a grid as large objects are small
     if roi_gdf is not None:
-        # TODO: support creating a grid in latlon????
-        if crs.is_projected:
-
-            # Create grid
-            grid_for_roi_gdf = geofileops.util.grid_util.create_grid3(
-                image_gen_bounds, width=crs_width, height=crs_height, crs=crs
-            )
-
-            # Create intersection layer between grid and roi
-            roi_gdf = gpd.overlay(grid_for_roi_gdf, roi_gdf, how="intersection")
-
-            # Explode possible multipolygons to polygons
-            # roi_gdf.reset_index(drop=True, inplace=True)
-            # assert to evade pyLance warning
-            assert isinstance(roi_gdf, gpd.GeoDataFrame)
-            roi_gdf = roi_gdf.explode(ignore_index=True)
-            # roi_gdf.reset_index(drop=True, inplace=True)
-
-            # Write to file
-            grid_for_roi_path = output_image_dir / "grid_for_roi.gpkg"
-            if grid_for_roi_path.exists() is False:
-                gfo.to_file(grid_for_roi_gdf, grid_for_roi_path)
-            assert isinstance(roi_gdf, gpd.GeoDataFrame)
-            gridded_roi_path = output_image_dir / "gridded_roi.gpkg"
-            if gridded_roi_path.exists() is False:
-                gfo.to_file(roi_gdf, gridded_roi_path)
+        # The tiles should intersect, but touching is not enough
+        tiles_intersects_roi_gdf = tiles_to_download_gdf.sjoin(
+            roi_gdf[["geometry"]], how="inner", predicate="intersects"
+        )
+        tiles_touches_roi_gdf = tiles_to_download_gdf.sjoin(
+            roi_gdf[["geometry"]], how="inner", predicate="touches"
+        )
+        tiles_to_download_gdf = tiles_intersects_roi_gdf.loc[
+            ~tiles_intersects_roi_gdf.index.isin(tiles_touches_roi_gdf.index)
+        ]
+
+    # Write the tiles to download to file for reference
+    tiles_path = output_image_dir / "tiles_to_download.gpkg"
+    if not tiles_path.exists():
+        gfo.to_file(tiles_to_download_gdf, tiles_path)
 
-    # Inits to start getting images
+    # Prepare WMS connection(s)
+    auth = _interprete_ssl_verify(ssl_verify=ssl_verify)
     layersources_prepared = []
     for layersource in layersources:
         wms_service = owslib.wms.WebMapService(
             url=layersource["wms_server_url"],
             version=layersource["wms_version"],
+            username=layersource["wms_username"],
+            password=layersource["wms_password"],
             auth=auth,
         )
         if layersource["wms_ignore_capabilities_url"]:
             # If the wms url in capabilities should be ignored,
             # overwrite with original url
             nb = len(wms_service.getOperationByName("GetMap").methods)
             for method_id in range(nb):
@@ -324,218 +242,166 @@
                 random_sleep=layersource["random_sleep"],
             )
         )
 
     with futures.ThreadPoolExecutor(nb_concurrent_calls) as pool:
 
         # Loop through all columns and get the images...
-        logger.info("Start loading images")
-        start_time = None
-        start_time_lastprogress = None
-        nb_todo = cols * rows
+        has_switched_axes = _has_switched_axes(crs)
+        nb_total = len(tiles_to_download_gdf)
         nb_processed = 0
-        nb_processed_lastprogress = 0
         nb_downloaded = 0
-        nb_ignore_in_progress = 0
-        bbox_list = []
-        size_list = []
-        output_filename_list = []
-        output_dir_list = []
-        for col in range(column_start, cols):
+        download_queue = {}
+        logger.info(f"Start loading {nb_total} images")
+        progress = None
+        for tile in tiles_to_download_gdf.geometry.bounds.itertuples():
+            # If a cron_schedule is specified, check if we should be running
+            if cron_schedule is not None and cron_schedule != "":
+                # Sleep till the schedule becomes active
+                first_cron_check = True
+                while not pycron.is_now(cron_schedule):
+                    # The first time, log message that we are going to sleep...
+                    if first_cron_check is True:
+                        logger.info(f"Time schedule specified: sleep: {cron_schedule}")
+                        first_cron_check = False
+                    time.sleep(60)
+
+            # Init progress
+            if progress is None:
+                message = (
+                    f"load_images to {output_image_dir.parent.name}/"
+                    f"{output_image_dir.name}"
+                )
+                progress = progress_util.ProgressLogger(
+                    message=message,
+                    nb_steps_total=nb_total,
+                    nb_steps_done=0,
+                )
 
-            image_xmin = col * crs_width + image_gen_bounds[0]
-            image_xmax = (col + 1) * crs_width + image_gen_bounds[0]
+            nb_processed += 1
+            _, tile_xmin, tile_ymin, tile_xmax, tile_ymax = tile
+            tile_pixel_width = image_pixel_width
+            tile_pixel_height = image_pixel_height
 
             # If overlapping images are wanted... increase image bbox
             if pixels_overlap:
-                image_xmin = image_xmin - (pixels_overlap * image_crs_pixel_x_size)
-                image_xmax = image_xmax + (pixels_overlap * image_crs_pixel_x_size)
+                tile_xmin -= pixels_overlap * image_crs_pixel_x_size
+                tile_xmax += pixels_overlap * image_crs_pixel_x_size
+                tile_ymin -= pixels_overlap * image_crs_pixel_y_size
+                tile_ymax += pixels_overlap * image_crs_pixel_y_size
+                tile_pixel_width += 2 * pixels_overlap
+                tile_pixel_height += 2 * pixels_overlap
 
-            # Put all the images of this column in a dir
+            # Create output filepath
             if crs.is_projected:
-                output_dir = output_image_dir / f"{image_xmin:06.0f}"
+                output_dir = output_image_dir / f"{tile_xmin:06.0f}"
             else:
-                output_dir = output_image_dir / f"{image_xmin:09.4f}"
-            if not output_dir.exists():
-                output_dir.mkdir()
-
-            logger.debug(
-                f"load_images to {output_image_dir.parent.name}/{output_image_dir.name}"
-                f", column {col} ({output_dir.name})"
+                output_dir = output_image_dir / f"{tile_xmin:09.4f}"
+            output_filename = _create_filename(
+                crs=crs,
+                bbox=(tile_xmin, tile_ymin, tile_xmax, tile_ymax),
+                size=(tile_pixel_width, tile_pixel_height),
+                image_format=image_format,
+                layername=None,
             )
-            for row in range(0, rows):
+            output_filepath = output_dir / output_filename
 
-                # If a cron_schedule is specified, check if we should be running
-                if cron_schedule is not None and cron_schedule != "":
-                    # Sleep till the schedule becomes active
-                    first_time = True
-                    while not pycron.is_now(cron_schedule):
-                        # The first time, log message that we are going to sleep...
-                        if first_time is True:
-                            logger.info(
-                                f"Time schedule specified: sleep: {cron_schedule}"
-                            )
-                            first_time = False
-                        time.sleep(60)
-
-                nb_processed += 1
-
-                # Calculate y bounds
-                image_ymin = row * crs_height + image_gen_bounds[1]
-                image_ymax = (row + 1) * crs_height + image_gen_bounds[1]
-
-                # If overlapping images are wanted... increase image bbox
-                if pixels_overlap:
-                    image_ymin = image_ymin - (pixels_overlap * image_crs_pixel_y_size)
-                    image_ymax = image_ymax + (pixels_overlap * image_crs_pixel_y_size)
-
-                # Create output filename
-                output_filename = _create_filename(
-                    crs=crs,
-                    bbox=(image_xmin, image_ymin, image_xmax, image_ymax),
-                    size=(
-                        image_pixel_width + 2 * pixels_overlap,
-                        image_pixel_height + 2 * pixels_overlap,
-                    ),
-                    image_format=image_format,
-                    layername=None,
-                )
-                output_filepath = output_dir / output_filename
+            # Do some checks to know if the image needs to be downloaded
+            if nb_images_to_skip > 0 and (nb_processed % nb_images_to_skip) != 0:
+                # If we need to skip images, do so...
+                progress.step()
+                continue
+            elif (
+                not force
+                and output_filepath.exists()
+                and output_filepath.stat().st_size > 0
+            ):
+                # Image exists already
+                progress.step()
+                logger.debug("    -> image exists already, so skip")
+                continue
+
+            # Submit the image to be downloaded
+            output_dir.mkdir(parents=True, exist_ok=True)
+            future = pool.submit(
+                getmap_to_file,  # Function
+                layersources=layersources_prepared,
+                output_dir=output_dir,
+                crs=crs,
+                bbox=(tile_xmin, tile_ymin, tile_xmax, tile_ymax),
+                size=(tile_pixel_width, tile_pixel_height),
+                image_format=image_format,
+                image_format_save=image_format_save,
+                output_filename=output_filename,
+                transparent=transparent,
+                tiff_compress=tiff_compress,
+                image_pixels_ignore_border=image_pixels_ignore_border,
+                has_switched_axes=has_switched_axes,
+                force=force,
+            )
+            download_queue[future] = output_filename
 
-                # Do some checks to know if the image needs to be downloaded
-                image_to_be_skipped = False
-                if nb_images_to_skip > 0 and (nb_processed % nb_images_to_skip) != 0:
-                    # If we need to skip images, do so...
-                    nb_ignore_in_progress += 1
-                    image_to_be_skipped = True
-                elif (
-                    not force
-                    and output_filepath.exists()
-                    and output_filepath.stat().st_size > 0
-                ):
-                    # Image exists already
-                    nb_ignore_in_progress += 1
-                    image_to_be_skipped = True
-                    logger.debug("    -> image exists already, so skip")
-                elif roi_gdf is not None:
-                    # If roi was provided, check first if the current image overlaps
-                    image_shape = sh_geom.box(
-                        image_xmin, image_ymin, image_xmax, image_ymax
-                    )
-
-                    possible_match_indexes = list(
-                        roi_gdf.geometry.sindex.query(image_shape)
-                    )
-                    possible_matches_gdf = roi_gdf.iloc[possible_match_indexes]
-                    precise_matches_gdf = possible_matches_gdf.loc[
-                        possible_matches_gdf.intersects(image_shape)
-                    ]
-
-                    if len(precise_matches_gdf) == 0:
-                        nb_ignore_in_progress += 1
-                        logger.debug("    -> image doesn't overlap with roi, so skip")
-                        image_to_be_skipped = True
-
-                # If the image doesn't need to be skipped... append the image
-                # info to the batch arrays so they can be treated in
-                # bulk if the batch size is reached
-                if image_to_be_skipped is False:
-                    bbox_list.append((image_xmin, image_ymin, image_xmax, image_ymax))
-                    size_list.append(
-                        (
-                            image_pixel_width + 2 * pixels_overlap,
-                            image_pixel_height + 2 * pixels_overlap,
-                        )
-                    )
-                    output_filename_list.append(output_filename)
-                    output_dir_list.append(output_dir)
-
-                # If the batch size is reached or we are at the last images
-                nb_images_in_batch = len(bbox_list)
-                if nb_images_in_batch == nb_concurrent_calls or nb_processed == (
-                    nb_todo - 1
+            # Process finished downloads till queue is of acceptable size
+            while True:
+                # Process downloads that are ready
+                futures_done = []
+                for future in download_queue:
+                    if not future.done():
+                        continue
+
+                    # Fetch result: will throw exception if something went wrong
+                    _ = future.result()
+                    nb_downloaded += 1
+                    futures_done.append(future)
+
+                    # Log the progress and download speed
+                    progress.step()
+
+                # Remove futures that are done
+                for future in futures_done:
+                    del download_queue[future]
+                futures_done = []
+
+                # If all image tiles have been processed or if the max number of
+                # images to download is reached...
+                if (
+                    nb_processed >= nb_total
+                    or max_nb_images > -1
+                    and nb_downloaded >= max_nb_images
                 ):
+                    if len(download_queue) == 0:
+                        return
+                else:
+                    # Not all tiles have been processed yet, and the queue isn't too
+                    # full, so process some more
+                    if len(download_queue) < nb_concurrent_calls * 2:
+                        break
 
-                    # Now we are getting to start fetching images... init start_time
-                    if start_time is None or start_time_lastprogress is None:
-                        start_time = datetime.datetime.now()
-                        nb_processed_lastprogress = nb_processed
-
-                    # Exec in parallel
-                    read_results = pool.map(
-                        getmap_to_file,  # Function
-                        it.repeat(layersources_prepared),
-                        output_dir_list,
-                        it.repeat(crs),
-                        bbox_list,
-                        size_list,
-                        it.repeat(image_format),
-                        it.repeat(image_format_save),
-                        output_filename_list,
-                        it.repeat(transparent),
-                        it.repeat(tiff_compress),
-                        it.repeat(image_pixels_ignore_border),
-                        it.repeat(force),
-                    )
-
-                    for _ in read_results:
-                        nb_downloaded += 1
-
-                    # Progress
-                    logger.debug(
-                        f"Process image {nb_processed} out of {cols*rows}: "
-                        f"{nb_processed/(cols*rows):.2f} %"
-                    )
-
-                    # Log the progress and prediction speed
-                    time_between_progress_s = 60
-                    time_passed_s = (
-                        datetime.datetime.now() - start_time
-                    ).total_seconds()
-                    if start_time_lastprogress is None:
-                        time_passed_lastprogress_s = time_between_progress_s
-                    else:
-                        time_passed_lastprogress_s = (
-                            datetime.datetime.now() - start_time_lastprogress
-                        ).total_seconds()
-                    if (
-                        time_passed_s > 0
-                        and time_passed_lastprogress_s >= time_between_progress_s
-                    ):
-                        nb_per_hour = (
-                            (nb_processed - nb_ignore_in_progress) / time_passed_s
-                        ) * 3600
-                        nb_per_hour_lastprogress = (
-                            nb_processed_lastprogress
-                            - nb_processed / time_passed_lastprogress_s
-                        ) * 3600
-                        hours_to_go = (int)((nb_todo - nb_processed) / nb_per_hour)
-                        min_to_go = (int)(
-                            (((nb_todo - nb_processed) / nb_per_hour) % 1) * 60
-                        )
-                        progress_message = (
-                            f"load_images to {output_image_dir.parent.name}/"
-                            f"{output_image_dir.name}, {hours_to_go:3d}:{min_to_go:2d} "
-                            f"left for {nb_todo-nb_processed} images at "
-                            f"{nb_per_hour:0.0f}/h ({nb_per_hour_lastprogress:0.0f}/h "
-                            f"last batch), with {nb_ignore_in_progress} skipped"
-                        )
-                        logger.info(progress_message)
-
-                        start_time_lastprogress = datetime.datetime.now()
-                        nb_processed_lastprogress = nb_processed
-
-                    # Reset variable for next batch
-                    bbox_list = []
-                    size_list = []
-                    output_filename_list = []
-                    output_dir_list = []
+                # Sleep a bit before checking again if there are downloads ready
+                time.sleep(0.1)
 
-                    if max_nb_images > -1 and nb_downloaded >= max_nb_images:
-                        return
+
+def _interprete_ssl_verify(ssl_verify: Union[bool, str, None]):
+    # Interprete ssl_verify
+    auth = None
+    if ssl_verify is not None:
+        # If it is a string, make sure it isn't actually a bool
+        if isinstance(ssl_verify, str):
+            if ssl_verify.lower() == "true":
+                ssl_verify = True
+            elif ssl_verify.lower() == "false":
+                ssl_verify = False
+
+        assert isinstance(ssl_verify, bool)
+        auth = owslib.util.Authentication(verify=ssl_verify)
+        if ssl_verify is False:
+            urllib3.disable_warnings()
+            logger.warn("SSL VERIFICATION IS TURNED OFF!!!")
+
+    return auth
 
 
 class LayerSource:
     def __init__(
         self,
         wms_service: Union[
             owslib.wms.wms111.WebMapService_1_1_1, owslib.wms.wms130.WebMapService_1_3_0
@@ -562,14 +428,15 @@
     image_format_save: Optional[str] = None,
     output_filename: Optional[str] = None,
     transparent: bool = False,
     tiff_compress: str = "lzw",
     image_pixels_ignore_border: int = 0,
     force: bool = False,
     layername_in_filename: bool = False,
+    has_switched_axes: Optional[bool] = None,
 ) -> Optional[Path]:
     """
 
 
     Args:
         layersources (List[dict]): Layer sources to get images from. Multiple
             sources can be specified to create a combined image, eg. use band
@@ -582,14 +449,17 @@
         image_format_save (str, optional): [description]. Defaults to None.
         output_filename (str, optional): [description]. Defaults to None.
         transparent (bool, optional): [description]. Defaults to False.
         tiff_compress (str, optional): [description]. Defaults to 'lzw'.
         image_pixels_ignore_border (int, optional): [description]. Defaults to 0.
         force (bool, optional): [description]. Defaults to False.
         layername_in_filename (bool, optional): [description]. Defaults to False.
+        has_switched_axes (bool, optional): True if x and y axes should be switched to
+            in the WMS GetMap request. If None, an effort is made to determine it
+            automatically based on the crs. Defaults to None.
 
     Raises:
         Exception: [description]
         Exception: [description]
         Exception: [description]
         Exception: [description]
 
@@ -656,15 +526,17 @@
         )
         size_for_getmap = (
             size[0] + 2 * image_pixels_ignore_border,
             size[1] + 2 * image_pixels_ignore_border,
         )
 
     # For coordinate systems with switched axis (y, x or lon, lat), switch x and y
-    if _has_switched_axes(crs):
+    if has_switched_axes is None:
+        has_switched_axes = _has_switched_axes(crs)
+    if has_switched_axes:
         bbox_for_getmap = (
             bbox_for_getmap[1],
             bbox_for_getmap[0],
             bbox_for_getmap[3],
             bbox_for_getmap[2],
         )
```

### Comparing `orthoseg-0.4.1b4/orthoseg/util/vector_util.py` & `orthoseg-0.4.2a1/orthoseg/util/vector_util.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/orthoseg.egg-info/PKG-INFO` & `orthoseg-0.4.2a1/orthoseg.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthoseg
-Version: 0.4.1b4
+Version: 0.4.2a1
 Summary: Package to make it easier to segment orthophotos.
 Home-page: https://github.com/orthoseg/orthoseg
 Author: Pieter Roggemans
 Author-email: pieter.roggemans@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `orthoseg-0.4.1b4/orthoseg.egg-info/SOURCES.txt` & `orthoseg-0.4.2a1/orthoseg.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,31 +18,30 @@
 orthoseg.egg-info/dependency_links.txt
 orthoseg.egg-info/entry_points.txt
 orthoseg.egg-info/requires.txt
 orthoseg.egg-info/top_level.txt
 orthoseg/helpers/__init__.py
 orthoseg/helpers/config_helper.py
 orthoseg/helpers/email_helper.py
-orthoseg/helpers/progress_helper.py
 orthoseg/helpers/vectorfile_helper.py
 orthoseg/lib/__init__.py
 orthoseg/lib/postprocess_predictions.py
 orthoseg/lib/predicter.py
 orthoseg/lib/prepare_traindatasets.py
 orthoseg/lib/trainer.py
 orthoseg/model/__init__.py
 orthoseg/model/model_factory.py
 orthoseg/model/model_helper.py
 orthoseg/util/__init__.py
 orthoseg/util/config_util.py
-orthoseg/util/gdrive_util.py
 orthoseg/util/general_util.py
 orthoseg/util/git_downloader.py
 orthoseg/util/log_util.py
 orthoseg/util/ows_util.py
+orthoseg/util/progress_util.py
 orthoseg/util/vector_util.py
 tests/__init__.py
 tests/test_end2end.py
 tests/test_helper.py
 tests/test_load_sampleprojects.py
 tests/test_model_factory.py
 tests/test_ows_util.py
```

### Comparing `orthoseg-0.4.1b4/setup.py` & `orthoseg-0.4.2a1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,23 +15,24 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/orthoseg/orthoseg",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=[
         "fiona",
+        "gdown",
         "geofileops>0.5,<0.7",
         "geopandas",
         "owslib",
         "pillow",
         "pycron",
         "rasterio",
         "segmentation-models>=1.0,<1.1",
         "simplification",
-        "tensorflow>=2.5,<2.9",
+        "tensorflow>=2.5,<2.11",
     ],
     entry_points="""
             [console_scripts]
             orthoseg_load_images=orthoseg.load_images:main
             orthoseg_train=orthoseg.train:main
             orthoseg_predict=orthoseg.predict:main
             orthoseg_postprocess=orthoseg.postprocess:main
```

### Comparing `orthoseg-0.4.1b4/tests/test_end2end.py` & `orthoseg-0.4.2a1/tests/test_end2end.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 from datetime import datetime
 import os
 from pathlib import Path
 import shutil
 import sys
 import tempfile
 
+import gdown
 import geofileops as gfo
 import pytest
 
 # Add path so the local orthoseg packages are found
 root_dir = Path(__file__).resolve().parent.parent
 sys.path.insert(0, str(root_dir))
 import orthoseg
 from orthoseg.helpers import config_helper as conf
 import orthoseg.model.model_helper as mh
-from orthoseg.util import gdrive_util
+
 from tests.test_helper import TestData
 
 # ----------------------------------------------------
 # Init
 # ----------------------------------------------------
 
 testprojects_dir = Path(tempfile.gettempdir()) / "orthoseg_test_end2end/sample_projects"
@@ -60,15 +61,15 @@
 
     # Run task to load images
     orthoseg.load_images(config_path)
 
     # Check if the right number of files was loaded
     assert image_cache_dir.exists()
     files = list(image_cache_dir.glob("**/*.jpg"))
-    assert len(files) == 8
+    assert len(files) == 4
 
 
 @pytest.mark.skipif(
     "GITHUB_ACTIONS" in os.environ and os.name == "nt",
     reason="crashes on github CI on windows",
 )
 @pytest.mark.order(after="test_1_init_testproject")
@@ -140,34 +141,40 @@
         assert not result_vector_dir.exists()
 
     # Download the version 01 model
     model_dir = conf.dirs.getpath("model_dir")
     model_dir.mkdir(parents=True, exist_ok=True)
     model_hdf5_path = model_dir / "footballfields_01_0.97392_201.hdf5"
     if not model_hdf5_path.exists():
-        gdrive_util.download_file("1UlNorZ74ADCr3pL4MCJ_tnKRNoeZX79g", model_hdf5_path)
+        gdown.download(
+            id="1UlNorZ74ADCr3pL4MCJ_tnKRNoeZX79g", output=str(model_hdf5_path)
+        )
     model_hyperparams_path = model_dir / "footballfields_01_hyperparams.json"
     if not model_hyperparams_path.exists():
-        gdrive_util.download_file(
-            "1NwrVVjx9IsjvaioQ4-bkPMrq7S6HeWIo", model_hyperparams_path
+        gdown.download(
+            id="1NwrVVjx9IsjvaioQ4-bkPMrq7S6HeWIo", output=str(model_hyperparams_path)
         )
     model_modeljson_path = model_dir / "footballfields_01_model.json"
     if not model_modeljson_path.exists():
-        gdrive_util.download_file(
-            "1LNPLypM5in3aZngBKK_U4Si47Oe97ZWN", model_modeljson_path
+        gdown.download(
+            id="1LNPLypM5in3aZngBKK_U4Si47Oe97ZWN", output=str(model_modeljson_path)
         )
 
     # Run task to predict
     orthoseg.predict(config_path)
 
     # Check results
     result_vector_path = result_vector_dir / "footballfields_01_201_BEFL-2019.gpkg"
     assert result_vector_path.exists()
     result_gdf = gfo.read_file(result_vector_path)
-    assert len(result_gdf) == 356
+    if os.name == "nt":
+        assert len(result_gdf) == 233
+    else:
+        # Since 2023-02-17, predict result on linux and Mac became different...
+        assert len(result_gdf) == 259
 
 
 @pytest.mark.skipif(
     "GITHUB_ACTIONS" in os.environ and os.name == "nt",
     reason="crashes on github CI on windows",
 )
 @pytest.mark.order(after="test_4_predict")
@@ -186,8 +193,12 @@
 
     # Run task to postprocess
     orthoseg.postprocess(config_path)
 
     # Check results
     assert result_diss_path.exists()
     result_gdf = gfo.read_file(result_diss_path)
-    assert len(result_gdf) == 350
+    if os.name == "nt":
+        assert len(result_gdf) == 227
+    else:
+        # Since 2023-02-17, predict result on linux and Mac became different...
+        assert len(result_gdf) == 239
```

### Comparing `orthoseg-0.4.1b4/tests/test_helper.py` & `orthoseg-0.4.2a1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/tests/test_load_sampleprojects.py` & `orthoseg-0.4.2a1/tests/test_load_sampleprojects.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,63 @@
 # -*- coding: utf-8 -*-
 """
 Tests for functionalities in orthoseg.train.
 """
 
+import os
 from pathlib import Path
+import platform
 import shutil
 import sys
 
+import pytest
+
 # Add path so the local orthoseg packages are found
 sys.path.insert(0, str(Path(__file__).resolve().parent.parent))
 from orthoseg import load_sampleprojects
 
 # ----------------------------------------------------
 # Tests
 # ----------------------------------------------------
 
 
 def get_testdata_dir() -> Path:
     return Path(__file__).resolve().parent / "data"
 
 
+@pytest.mark.skipif(
+    "GITHUB_ACTIONS" in os.environ
+    and not (
+        platform.system() == "Linux"
+        and sys.version_info.major == 3
+        and sys.version_info.minor == 10
+    ),
+    reason="on github CI, run this only in one env to avoid rate limit exceeded",
+)
 def test_load_sampleprojects(tmp_path):
     sampleprojects_dir = tmp_path / "sample_projects"
     shutil.rmtree(sampleprojects_dir, ignore_errors=True)
-    load_sampleprojects.load_sampleprojects(
-        dest_dir=sampleprojects_dir.parent, ssl_verify=False
-    )
-    # Check if the right number of files was loaded
+    load_sampleprojects.load_sampleprojects(dest_dir=sampleprojects_dir.parent)
+
+    # Check if the files were correctly loaded
     assert sampleprojects_dir.exists()
     assert (sampleprojects_dir / "imagelayers.ini").exists()
     assert (sampleprojects_dir / "project_defaults_overrule.ini").exists()
     assert (sampleprojects_dir / "run_footballfields.py").exists()
 
     footballfields_dir = sampleprojects_dir / "footballfields"
     assert footballfields_dir.exists()
     files = list((footballfields_dir).glob("**/*.ini"))
     assert len(files) > 0
     files = list((footballfields_dir / "labels").glob("**/*.gpkg"))
     assert len(files) == 2
+    model_path = footballfields_dir / "models" / "footballfields_01_0.92512_242.hdf5"
+    assert model_path.exists()
+    # The model should be larger than 50 MB, otherwise not normal
+    assert model_path.stat().st_size > 50 * 1024 * 1024
 
     projecttemplate_dir = sampleprojects_dir / "project_template"
     assert projecttemplate_dir.exists()
     files = list((projecttemplate_dir).glob("**/*.ini"))
     assert len(files) > 0
     files = list((projecttemplate_dir / "labels").glob("**/*.gpkg"))
     assert len(files) == 2
```

### Comparing `orthoseg-0.4.1b4/tests/test_model_factory.py` & `orthoseg-0.4.2a1/tests/test_model_factory.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/tests/test_ows_util.py` & `orthoseg-0.4.2a1/tests/test_ows_util.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/tests/test_postprocess_predictions.py` & `orthoseg-0.4.2a1/tests/test_postprocess_predictions.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/tests/test_prepare_traindata.py` & `orthoseg-0.4.2a1/tests/test_prepare_traindata.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/tests/test_train.py` & `orthoseg-0.4.2a1/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `orthoseg-0.4.1b4/tests/test_vector_util.py` & `orthoseg-0.4.2a1/tests/test_vector_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
         testdata_gdf.geometry, tolerance=0.375, algorithm=gfo.SimplifyAlgorithm.LANG
     )
     for index, _, geometry in testdata_gdf.itertuples():
         if geometry is None or geometry.is_empty or index > 4:
             assert simplified_gdf["geometry"][index] is None
         else:
             if index == 4:
-                assert geometry.type == simplified_gdf["geometry"][index].type
+                assert geometry.geom_type == simplified_gdf["geometry"][index].geom_type
 
     # Test empty geoseries
     # --------------------
     result = vector_util.simplify_topo_orthoseg(
         gpd.GeoSeries(), tolerance=0.375, algorithm=gfo.SimplifyAlgorithm.LANG
     )
     assert result is not None
```

### Comparing `orthoseg-0.4.1b4/tests/test_vectorfile_helper.py` & `orthoseg-0.4.2a1/tests/test_vectorfile_helper.py`

 * *Files identical despite different names*

