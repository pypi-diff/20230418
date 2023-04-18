# Comparing `tmp/YALTAi-0.1.2.tar.gz` & `tmp/YALTAi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YALTAi-0.1.2.tar", last modified: Thu Mar  2 14:35:43 2023, max compression
+gzip compressed data, was "YALTAi-0.1.3.tar", last modified: Tue Apr 18 06:42:48 2023, max compression
```

## Comparing `YALTAi-0.1.2.tar` & `YALTAi-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-03-02 14:35:43.616792 YALTAi-0.1.2/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    35149 2022-07-06 06:59:25.000000 YALTAi-0.1.2/LICENSE
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       27 2022-07-08 14:49:38.000000 YALTAi-0.1.2/MANIFEST.in
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2583 2023-03-02 14:35:43.616792 YALTAi-0.1.2/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1865 2022-10-11 12:11:53.000000 YALTAi-0.1.2/README.md
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-03-02 14:35:43.616792 YALTAi-0.1.2/YALTAi.egg-info/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2583 2023-03-02 14:35:43.000000 YALTAi-0.1.2/YALTAi.egg-info/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      392 2023-03-02 14:35:43.000000 YALTAi-0.1.2/YALTAi.egg-info/SOURCES.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2023-03-02 14:35:43.000000 YALTAi-0.1.2/YALTAi.egg-info/dependency_links.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       87 2023-03-02 14:35:43.000000 YALTAi-0.1.2/YALTAi.egg-info/entry_points.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      306 2023-03-02 14:35:43.000000 YALTAi-0.1.2/YALTAi.egg-info/requires.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        7 2023-03-02 14:35:43.000000 YALTAi-0.1.2/YALTAi.egg-info/top_level.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2023-03-02 14:35:43.616792 YALTAi-0.1.2/setup.cfg
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3850 2023-03-02 14:35:29.000000 YALTAi-0.1.2/setup.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-03-02 14:35:43.616792 YALTAi-0.1.2/yaltai/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2022-07-06 07:04:33.000000 YALTAi-0.1.2/yaltai/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2758 2022-07-11 09:16:09.000000 YALTAi-0.1.2/yaltai/converter.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     5334 2022-10-15 08:16:58.000000 YALTAi-0.1.2/yaltai/kraken_adapter.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    11786 2023-03-02 14:35:15.000000 YALTAi-0.1.2/yaltai/kraken_yaltai.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1242 2022-11-02 13:44:52.000000 YALTAi-0.1.2/yaltai/preprocessing.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      784 2022-07-08 13:56:45.000000 YALTAi-0.1.2/yaltai/template.xml
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    11832 2023-03-02 14:31:06.000000 YALTAi-0.1.2/yaltai/yaltai.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1987 2022-11-02 13:45:48.000000 YALTAi-0.1.2/yaltai/yolo_adapter.py
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-04-18 06:42:48.675756 YALTAi-0.1.3/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       27 2023-04-18 06:34:32.000000 YALTAi-0.1.3/MANIFEST.in
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     3068 2023-04-18 06:42:48.675756 YALTAi-0.1.3/PKG-INFO
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1865 2023-04-18 06:34:32.000000 YALTAi-0.1.3/README.md
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-04-18 06:42:48.675756 YALTAi-0.1.3/YALTAi.egg-info/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     3068 2023-04-18 06:42:48.000000 YALTAi-0.1.3/YALTAi.egg-info/PKG-INFO
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      384 2023-04-18 06:42:48.000000 YALTAi-0.1.3/YALTAi.egg-info/SOURCES.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        1 2023-04-18 06:42:48.000000 YALTAi-0.1.3/YALTAi.egg-info/dependency_links.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       87 2023-04-18 06:42:48.000000 YALTAi-0.1.3/YALTAi.egg-info/entry_points.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      332 2023-04-18 06:42:48.000000 YALTAi-0.1.3/YALTAi.egg-info/requires.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        7 2023-04-18 06:42:48.000000 YALTAi-0.1.3/YALTAi.egg-info/top_level.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       38 2023-04-18 06:42:48.675756 YALTAi-0.1.3/setup.cfg
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     3850 2023-04-18 06:42:14.000000 YALTAi-0.1.3/setup.py
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-04-18 06:42:48.675756 YALTAi-0.1.3/yaltai/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        0 2023-04-18 06:34:32.000000 YALTAi-0.1.3/yaltai/__init__.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2758 2023-04-18 06:34:32.000000 YALTAi-0.1.3/yaltai/converter.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     5334 2023-04-18 06:34:32.000000 YALTAi-0.1.3/yaltai/kraken_adapter.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)    11786 2023-04-18 06:34:32.000000 YALTAi-0.1.3/yaltai/kraken_yaltai.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1242 2023-04-18 06:34:32.000000 YALTAi-0.1.3/yaltai/preprocessing.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      784 2023-04-18 06:34:32.000000 YALTAi-0.1.3/yaltai/template.xml
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)    11832 2023-04-18 06:34:32.000000 YALTAi-0.1.3/yaltai/yaltai.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1987 2023-04-18 06:34:32.000000 YALTAi-0.1.3/yaltai/yolo_adapter.py
```

### Comparing `YALTAi-0.1.2/PKG-INFO` & `YALTAi-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: YALTAi
-Version: 0.1.2
-Summary: You Actually Look Twice At it, YOLOv5-Kraken adapter for region detection 
-Home-page: https://github.com/ponteineptique/yaltai
-Author: Thibault Clérice
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # YALTAi
 You Actually Look Twice At it
 
 This provides an adapter for Kraken to use YOLOv5 Object Detection routine.
 
 This tool can be used for both segmenting and conversion of models.
 
@@ -55,15 +35,15 @@
 python train.py --data "../my-dataset/config.yml" --batch-size 4 --img 640 --weights yolov5x.pt --epochs 50
 ```
 
 ## Predicting
 
 YALTAi has the same CLI interface as Kraken, so:
 
-- You can use base BLLA model for line or provide yours with `-m model.mlmodel`
+- You can use base BLLA model for line or provide yours with `-i model.mlmodel`
 - Use a GPU (`--device cuda:0`) or a CPU (`--device cpu`)
 - Apply on batch (`*.jpg`)
 
 ```bash
 # Retrieve the best.pt after the training
 # It should be in runs/train/exp[NUMBER]/weights/best.pt
 # And then annotate your new data with the same CLI API as Kraken !
@@ -75,9 +55,7 @@
 The metrics produced from various libraries never gives the same mAP or Precision. I tried
 
 - `object-detection-metrics==0.4`
 - `mapCalc`
 - `mean-average-precision` which ended up being the chosen one (cleanest in terms of how I can access info) 
 
 and of course I compared with YOLOv5 raw results. Nothing worked the same. And the library YOLOv5 derives its metrics from is uninstallable through pip.
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `YALTAi-0.1.2/setup.py` & `YALTAi-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Package meta-data.
 NAME = 'YALTAi'
 DESCRIPTION = "You Actually Look Twice At it, YOLOv5-Kraken adapter for region detection "
 URL = 'https://github.com/ponteineptique/yaltai'
 AUTHOR = 'Thibault Clérice'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 
 # What packages are required for this module to be executed?
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     REQUIRED = f.read().splitlines()
 
 # What packages are optional?
```

### Comparing `YALTAi-0.1.2/yaltai/converter.py` & `YALTAi-0.1.3/yaltai/converter.py`

 * *Files identical despite different names*

### Comparing `YALTAi-0.1.2/yaltai/kraken_adapter.py` & `YALTAi-0.1.3/yaltai/kraken_adapter.py`

 * *Files identical despite different names*

### Comparing `YALTAi-0.1.2/yaltai/kraken_yaltai.py` & `YALTAi-0.1.3/yaltai/kraken_yaltai.py`

 * *Files identical despite different names*

### Comparing `YALTAi-0.1.2/yaltai/preprocessing.py` & `YALTAi-0.1.3/yaltai/preprocessing.py`

 * *Files identical despite different names*

### Comparing `YALTAi-0.1.2/yaltai/template.xml` & `YALTAi-0.1.3/yaltai/template.xml`

 * *Files identical despite different names*

### Comparing `YALTAi-0.1.2/yaltai/yaltai.py` & `YALTAi-0.1.3/yaltai/yaltai.py`

 * *Files identical despite different names*

### Comparing `YALTAi-0.1.2/yaltai/yolo_adapter.py` & `YALTAi-0.1.3/yaltai/yolo_adapter.py`

 * *Files identical despite different names*

