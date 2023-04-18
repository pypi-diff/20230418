# Comparing `tmp/ethome-ml-0.5.5.tar.gz` & `tmp/ethome-ml-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethome-ml-0.5.5.tar", last modified: Mon Apr 17 06:43:55 2023, max compression
+gzip compressed data, was "ethome-ml-0.6.0.tar", last modified: Tue Apr 18 06:40:37 2023, max compression
```

## Comparing `ethome-ml-0.5.5.tar` & `ethome-ml-0.6.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.069591 ethome-ml-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-17 06:43:55.069591 ethome-ml-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.053592 ethome-ml-0.5.5/ethome/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.053592 ethome-ml-0.5.5/ethome/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.053592 ethome-ml-0.5.5/ethome/data/boris/
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/boris/e3v813a-20210610T120637-121213_reencode.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/boris/e3v813a-20210610T121558-122141_reencode.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/boris/e3v813a-20210610T122332-122642_reencode.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/boris/e3v813a-20210610T122758-123309_reencode.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/boris/e3v813a-20210610T123521-124106_reencode.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.053592 ethome-ml-0.5.5/ethome/data/boris/multiple_behaviors/
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/boris/multiple_behaviors/e3v813a-20210610T120637-121213_reencode_multiple_behaviors.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.053592 ethome-ml-0.5.5/ethome/data/dlc/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/dlc/e3v813a-20210610T120637-121213DLC_dlcrnetms5_pilot_studySep24shuffle1_100000_el_filtered.csv
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/dlc/e3v813a-20210610T121558-122141DLC_dlcrnetms5_pilot_studySep24shuffle1_100000_el_filtered.csv
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/dlc/e3v813a-20210610T122332-122642DLC_dlcrnetms5_pilot_studySep24shuffle1_100000_el_filtered.csv
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/dlc/e3v813a-20210610T122758-123309DLC_dlcrnetms5_pilot_studySep24shuffle1_100000_el_filtered.csv
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/dlc/e3v813a-20210610T123521-124106DLC_dlcrnetms5_pilot_studySep24shuffle1_100000_el_filtered.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.057592 ethome-ml-0.5.5/ethome/data/dlc/openfield/
--rw-r--r--   0 runner    (1001) docker     (123)   525609 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/dlc/openfield/openfield_dlc_inference_example.csv
--rw-r--r--   0 runner    (1001) docker     (123)   525507 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/dlc/openfield/openfield_dlc_inference_example_missingdata.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1547416 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/dlc/openfield/openfield_dlc_inference_example_three.csv
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/sample_dataframe.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   500848 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/data/sample_nwb_.nwb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.057592 ethome-ml-0.5.5/ethome/features/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/cnn1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/dl_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/generic_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/mars_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.049591 ethome-ml-0.5.5/ethome/features/pretrained_models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.049591 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.057592 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_0/the_model/
--rw-r--r--   0 runner    (1001) docker     (123)   532906 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_0/the_model/saved_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.061591 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_0/the_model/variables/
--rw-r--r--   0 runner    (1001) docker     (123)  1493838 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_0/the_model/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_0/the_model/variables/variables.index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.049591 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.061591 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_1/the_model/
--rw-r--r--   0 runner    (1001) docker     (123)   536176 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_1/the_model/saved_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.061591 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_1/the_model/variables/
--rw-r--r--   0 runner    (1001) docker     (123)  1493878 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_1/the_model/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_1/the_model/variables/variables.index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.049591 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.061591 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_2/the_model/
--rw-r--r--   0 runner    (1001) docker     (123)   537931 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_2/the_model/saved_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.065591 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_2/the_model/variables/
--rw-r--r--   0 runner    (1001) docker     (123)  1493894 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_2/the_model/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_2/the_model/variables/variables.index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.049591 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.065591 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_3/the_model/
--rw-r--r--   0 runner    (1001) docker     (123)   539701 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_3/the_model/saved_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.065591 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_3/the_model/variables/
--rw-r--r--   0 runner    (1001) docker     (123)  1493922 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_3/the_model/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_3/the_model/variables/variables.index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.049591 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.065591 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_4/the_model/
--rw-r--r--   0 runner    (1001) docker     (123)   540133 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_4/the_model/saved_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.069591 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_4/the_model/variables/
--rw-r--r--   0 runner    (1001) docker     (123)  1493928 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_4/the_model/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_4/the_model/variables/variables.index
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25377 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/unsupervised.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34347 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/ethome/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.069591 ethome-ml-0.5.5/ethome_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-17 06:43:55.000000 ethome-ml-0.5.5/ethome_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-17 06:43:55.000000 ethome-ml-0.5.5/ethome_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 06:43:55.000000 ethome-ml-0.5.5/ethome_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 06:43:55.000000 ethome-ml-0.5.5/ethome_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 06:43:55.000000 ethome-ml-0.5.5/ethome_ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-17 06:43:43.000000 ethome-ml-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-17 06:43:55.069591 ethome-ml-0.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:43:55.069591 ethome-ml-0.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-04-17 06:43:44.000000 ethome-ml-0.5.5/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-04-17 06:43:44.000000 ethome-ml-0.5.5/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-17 06:43:44.000000 ethome-ml-0.5.5/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-17 06:43:44.000000 ethome-ml-0.5.5/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-17 06:43:44.000000 ethome-ml-0.5.5/tests/test_unsupervised.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-17 06:43:44.000000 ethome-ml-0.5.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.720725 ethome-ml-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-18 06:40:37.720725 ethome-ml-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.700726 ethome-ml-0.6.0/ethome/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.704726 ethome-ml-0.6.0/ethome/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.704726 ethome-ml-0.6.0/ethome/data/boris/
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/boris/e3v813a-20210610T120637-121213_reencode.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/boris/e3v813a-20210610T121558-122141_reencode.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/boris/e3v813a-20210610T122332-122642_reencode.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/boris/e3v813a-20210610T122758-123309_reencode.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/boris/e3v813a-20210610T123521-124106_reencode.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.704726 ethome-ml-0.6.0/ethome/data/boris/multiple_behaviors/
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/boris/multiple_behaviors/e3v813a-20210610T120637-121213_reencode_multiple_behaviors.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.704726 ethome-ml-0.6.0/ethome/data/dlc/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/dlc/e3v813a-20210610T120637-121213DLC_dlcrnetms5_pilot_studySep24shuffle1_100000_el_filtered.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/dlc/e3v813a-20210610T121558-122141DLC_dlcrnetms5_pilot_studySep24shuffle1_100000_el_filtered.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/dlc/e3v813a-20210610T122332-122642DLC_dlcrnetms5_pilot_studySep24shuffle1_100000_el_filtered.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/dlc/e3v813a-20210610T122758-123309DLC_dlcrnetms5_pilot_studySep24shuffle1_100000_el_filtered.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/dlc/e3v813a-20210610T123521-124106DLC_dlcrnetms5_pilot_studySep24shuffle1_100000_el_filtered.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.704726 ethome-ml-0.6.0/ethome/data/dlc/openfield/
+-rw-r--r--   0 runner    (1001) docker     (123)   525609 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/dlc/openfield/openfield_dlc_inference_example.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   525507 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/dlc/openfield/openfield_dlc_inference_example_missingdata.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1547416 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/dlc/openfield/openfield_dlc_inference_example_three.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/sample_dataframe.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   500848 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/data/sample_nwb_.nwb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.708726 ethome-ml-0.6.0/ethome/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/cnn1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/dl_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/generic_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26019 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/mars_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.700726 ethome-ml-0.6.0/ethome/features/pretrained_models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.700726 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.708726 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_0/the_model/
+-rw-r--r--   0 runner    (1001) docker     (123)   532906 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_0/the_model/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.708726 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_0/the_model/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)  1493838 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_0/the_model/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_0/the_model/variables/variables.index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.700726 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.708726 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_1/the_model/
+-rw-r--r--   0 runner    (1001) docker     (123)   536176 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_1/the_model/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.712725 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_1/the_model/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)  1493878 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_1/the_model/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_1/the_model/variables/variables.index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.700726 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.712725 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_2/the_model/
+-rw-r--r--   0 runner    (1001) docker     (123)   537931 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_2/the_model/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.716725 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_2/the_model/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)  1493894 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_2/the_model/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_2/the_model/variables/variables.index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.700726 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.716725 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_3/the_model/
+-rw-r--r--   0 runner    (1001) docker     (123)   539701 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_3/the_model/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.716725 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_3/the_model/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)  1493922 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_3/the_model/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_3/the_model/variables/variables.index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.700726 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.716725 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_4/the_model/
+-rw-r--r--   0 runner    (1001) docker     (123)   540133 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_4/the_model/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.720725 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_4/the_model/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)  1493928 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_4/the_model/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_4/the_model/variables/variables.index
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25377 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19568 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/unsupervised.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34042 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/ethome/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.720725 ethome-ml-0.6.0/ethome_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-18 06:40:37.000000 ethome-ml-0.6.0/ethome_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-18 06:40:37.000000 ethome-ml-0.6.0/ethome_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:40:37.000000 ethome-ml-0.6.0/ethome_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-18 06:40:37.000000 ethome-ml-0.6.0/ethome_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 06:40:37.000000 ethome-ml-0.6.0/ethome_ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-18 06:40:37.720725 ethome-ml-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:40:37.720725 ethome-ml-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/tests/test_unsupervised.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-18 06:40:26.000000 ethome-ml-0.6.0/tests/test_utils.py
```

### Comparing `ethome-ml-0.5.5/LICENSE` & `ethome-ml-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/PKG-INFO` & `ethome-ml-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethome-ml
-Version: 0.5.5
+Version: 0.6.0
 Summary: Tools for machine learning of animal behavior.
 Home-page: https://github.com/benlansdell/ethome
 Author: Ben Lansdell
 Author-email: ben.lansdell@gmail.com
 Project-URL: Bug Tracker, https://github.com/benlansdell/ethome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -56,26 +56,26 @@
 ```
 
 Create the dataframe:
 ```python
 dataset = create_dataset(fn_in)
 ```
 `dataset` is an extended pandas DataFrame, so can be treated exactly as you would treat any other dataframe. `ethome` adds a bunch of metadata about the dataset, for instance you can list the body parts with:
-```
+```python
 dataset.pose.body_parts
 ```
 
 A key functionality of `ethome` is the ability to easily create features for machine learning. You can use pre-built featuresets or make your own. For instance:
 ```python
 dataset.features.add('distances')
 ``` 
 will compute all distances between all body parts (both between and within animals).
 
 There are featuresets specifically tailored for social mice studies (resident intruder). For instance, 
-```
+```python
 dataset.features.add('cnn1d_prob')
 ```
 Uses a pretrained CNN to output probabilities of 3 behaviors (attack, mount, social investigation). For this, you must have labeled your body parts in a certain way (refer to How To). Other, more generic, feature creation functions are provided that work for any animal configuration. 
 
 Now you can access a features table, labels, and groups for learning with `dataset.ml.features, dataset.ml.labels, dataset.ml.group`. From here it's easy to use some ML libraries to train a behavior classifier. For example:
 ```python
 from sklearn.ensemble import RandomForestClassifier
@@ -103,9 +103,8 @@
 
 If the raw video file paths are provided in the metadata, under the `video` key, we can make a movie overlaying these predictions over the original video:
 ```python
 dataset.io.save_movie(['label', 'prediction'], '.')
 ```
 where `label` and `prediction` reference column names to annotate the video with.
 
-A more detailed run through of features is provided in the How To guide.
- 
+A more detailed run through of features is provided in the How To guide. Also checkout `examples` for working demos to quickly see how things work.
```

### Comparing `ethome-ml-0.5.5/README.md` & `ethome-ml-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,26 +41,26 @@
 ```
 
 Create the dataframe:
 ```python
 dataset = create_dataset(fn_in)
 ```
 `dataset` is an extended pandas DataFrame, so can be treated exactly as you would treat any other dataframe. `ethome` adds a bunch of metadata about the dataset, for instance you can list the body parts with:
-```
+```python
 dataset.pose.body_parts
 ```
 
 A key functionality of `ethome` is the ability to easily create features for machine learning. You can use pre-built featuresets or make your own. For instance:
 ```python
 dataset.features.add('distances')
 ``` 
 will compute all distances between all body parts (both between and within animals).
 
 There are featuresets specifically tailored for social mice studies (resident intruder). For instance, 
-```
+```python
 dataset.features.add('cnn1d_prob')
 ```
 Uses a pretrained CNN to output probabilities of 3 behaviors (attack, mount, social investigation). For this, you must have labeled your body parts in a certain way (refer to How To). Other, more generic, feature creation functions are provided that work for any animal configuration. 
 
 Now you can access a features table, labels, and groups for learning with `dataset.ml.features, dataset.ml.labels, dataset.ml.group`. From here it's easy to use some ML libraries to train a behavior classifier. For example:
 ```python
 from sklearn.ensemble import RandomForestClassifier
@@ -88,9 +88,8 @@
 
 If the raw video file paths are provided in the metadata, under the `video` key, we can make a movie overlaying these predictions over the original video:
 ```python
 dataset.io.save_movie(['label', 'prediction'], '.')
 ```
 where `label` and `prediction` reference column names to annotate the video with.
 
-A more detailed run through of features is provided in the How To guide.
- 
+A more detailed run through of features is provided in the How To guide. Also checkout `examples` for working demos to quickly see how things work.
```

### Comparing `ethome-ml-0.5.5/ethome/__init__.py` & `ethome-ml-0.6.0/ethome/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.5.5'
+__version__ = '0.6.0'
 
 #Suppress tensorflow import text...
 import os
 from importlib.util import find_spec 
 if find_spec('tensorflow') is not None:
     if 'TF_CPP_MIN_LOG_LEVEL' in os.environ:
         old_val = os.environ['TF_CPP_MIN_LOG_LEVEL']
```

### Comparing `ethome-ml-0.5.5/ethome/data/boris/e3v813a-20210610T120637-121213_reencode.csv` & `ethome-ml-0.6.0/ethome/data/boris/e3v813a-20210610T120637-121213_reencode.csv`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/data/boris/e3v813a-20210610T121558-122141_reencode.csv` & `ethome-ml-0.6.0/ethome/data/boris/e3v813a-20210610T121558-122141_reencode.csv`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/data/boris/e3v813a-20210610T122332-122642_reencode.csv` & `ethome-ml-0.6.0/ethome/data/boris/e3v813a-20210610T122332-122642_reencode.csv`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/data/boris/e3v813a-20210610T122758-123309_reencode.csv` & `ethome-ml-0.6.0/ethome/data/boris/e3v813a-20210610T122758-123309_reencode.csv`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/data/boris/e3v813a-20210610T123521-124106_reencode.csv` & `ethome-ml-0.6.0/ethome/data/boris/e3v813a-20210610T123521-124106_reencode.csv`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/data/boris/multiple_behaviors/e3v813a-20210610T120637-121213_reencode_multiple_behaviors.csv` & `ethome-ml-0.6.0/ethome/data/boris/multiple_behaviors/e3v813a-20210610T120637-121213_reencode_multiple_behaviors.csv`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/data/dlc/openfield/openfield_dlc_inference_example.csv` & `ethome-ml-0.6.0/ethome/data/dlc/openfield/openfield_dlc_inference_example.csv`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/data/dlc/openfield/openfield_dlc_inference_example_missingdata.csv` & `ethome-ml-0.6.0/ethome/data/dlc/openfield/openfield_dlc_inference_example_missingdata.csv`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/data/dlc/openfield/openfield_dlc_inference_example_three.csv` & `ethome-ml-0.6.0/ethome/data/dlc/openfield/openfield_dlc_inference_example_three.csv`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/data/sample_nwb_.nwb` & `ethome-ml-0.6.0/ethome/data/sample_nwb_.nwb`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/cnn1d.py` & `ethome-ml-0.6.0/ethome/features/cnn1d.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/dl_features.py` & `ethome-ml-0.6.0/ethome/features/dl_features.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/features.py` & `ethome-ml-0.6.0/ethome/features/features.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/generic_features.py` & `ethome-ml-0.6.0/ethome/features/generic_features.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/mars_features.py` & `ethome-ml-0.6.0/ethome/features/mars_features.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_0/the_model/saved_model.pb` & `ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_0/the_model/saved_model.pb`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_0/the_model/variables/variables.data-00000-of-00001` & `ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_0/the_model/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_0/the_model/variables/variables.index` & `ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_0/the_model/variables/variables.index`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_1/the_model/saved_model.pb` & `ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_1/the_model/saved_model.pb`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_1/the_model/variables/variables.data-00000-of-00001` & `ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_1/the_model/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_1/the_model/variables/variables.index` & `ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_1/the_model/variables/variables.index`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_2/the_model/saved_model.pb` & `ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_2/the_model/saved_model.pb`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_2/the_model/variables/variables.data-00000-of-00001` & `ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_2/the_model/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_2/the_model/variables/variables.index` & `ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_2/the_model/variables/variables.index`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_3/the_model/saved_model.pb` & `ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_3/the_model/saved_model.pb`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_3/the_model/variables/variables.data-00000-of-00001` & `ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_3/the_model/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_3/the_model/variables/variables.index` & `ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_3/the_model/variables/variables.index`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_4/the_model/saved_model.pb` & `ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_4/the_model/saved_model.pb`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_4/the_model/variables/variables.data-00000-of-00001` & `ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_4/the_model/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/features/pretrained_models/task1_model_fold_4/the_model/variables/variables.index` & `ethome-ml-0.6.0/ethome/features/pretrained_models/task1_model_fold_4/the_model/variables/variables.index`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/interpolation.py` & `ethome-ml-0.6.0/ethome/interpolation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Interpolate over low confidence data"""
+
 import pandas as pd 
 import numpy as np
 
 def interpolate_lowconf_points(edf : pd.DataFrame,
                                conf_threshold : float = 0.9,
                                in_place : bool = True,
                                rolling_window : bool = True,
```

### Comparing `ethome-ml-0.5.5/ethome/io.py` & `ethome-ml-0.6.0/ethome/io.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/models.py` & `ethome-ml-0.6.0/ethome/models.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/plot.py` & `ethome-ml-0.6.0/ethome/plot.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,83 @@
-import matplotlib.pyplot as plt
-import matplotlib as mpl
-from matplotlib import cm
 import os
 import time
+import matplotlib.pyplot as plt
+import matplotlib as mpl
 import numpy as np
-from glob import glob
 import pandas as pd
 
+from matplotlib import cm
+from glob import glob
+from ipywidgets import interact, IntSlider
+from IPython.display import display
+from itertools import product
+
 from ethome.config import global_config
 
+def interactive_tracks(df : pd.DataFrame, 
+                       filename : str, 
+                       animals : list = None,
+                       start_frame : int = 0, 
+                       stop_frame : int = None):
+    """Simple interactive widget to explore pose tracking data from a recording.
+    
+    Use within Jupyter Notebook, with %matplotlib inline
+
+    Args:
+        df: input DataFrame
+        filename: tracking file to source trackes from
+        animals: if provided, only plot these animals. Default = None = plot all
+        start_frame: Display frames after this value
+        stop_frame: Display frames up to this value. If None, show all frames in recording.
+        
+    Returns:
+        None. Plot is created and displayed by the function without returning. 
+    """
+    if animals is None:
+        animals = df.pose.animals 
+
+    df = df[(df['filename'] == filename)]
+    if stop_frame is None:
+        stop_frame = df.frame.max() 
+    df = df[(df['frame'] >= start_frame) & (df['frame'] <= stop_frame)]
+
+    all_x_cols = [f'{animal}_x_{bp}' for animal, bp in product(animals, df.pose.body_parts)]
+    all_y_cols = [f'{animal}_y_{bp}' for animal, bp in product(animals, df.pose.body_parts)]
+
+    xmin, xmax = np.min(df[all_x_cols].values), np.max(df[all_x_cols].values)
+    ymin, ymax = np.min(df[all_y_cols].values), np.max(df[all_y_cols].values)
+    
+    fig = plt.figure(figsize=(8,8))
+    styles = ['bo', 'r+', 'g.']
+
+    lines = {}
+    for idx, animal in enumerate(animals):
+        line, = plt.plot([], [], styles[idx%len(styles)])
+        lines[animal] = line
+
+    plt.xlim(xmin, xmax)
+    plt.ylim(ymin, ymax)
+    plt.xlabel('x')
+    plt.ylabel('y')
+    plt.title(','.join(animals) + ' from ' + os.path.basename(filename))
+    plt.close()
+
+    def plot_frame(frame):
+        for animal in animals:
+            x = []
+            y = []
+            for bp in df.pose.body_parts:
+                x.append(df.loc[df['frame'] == frame, f'{animal}_x_{bp}'].values[0])
+                y.append(df.loc[df['frame'] == frame, f'{animal}_y_{bp}'].values[0])
+            lines[animal].set_data(x, y)
+
+        display(fig)
+        
+    interact(plot_frame, frame=IntSlider(min=start_frame, max=stop_frame, value=start_frame))
+
 def plot_embedding(dataset : pd.DataFrame, 
                    col_names : list  = ['embedding_0', 'embedding_1'],
                    col_labels : list = None,
                    color_col : str = None, 
                    figsize : tuple = (10,10),
                    **kwargs) -> tuple:
     """Scatterplot of a 2D TSNE or UMAP embedding from the dataset.
```

### Comparing `ethome-ml-0.5.5/ethome/unsupervised.py` & `ethome-ml-0.6.0/ethome/unsupervised.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/utils.py` & `ethome-ml-0.6.0/ethome/utils.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/ethome/video.py` & `ethome-ml-0.6.0/ethome/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     metadata = {}
     for fn in tracking_files:
         metadata[fn] = {}
     n_files = len(tracking_files)
 
     for k,v in kwargs.items():
         if hasattr(v, '__len__'):
-            if len(v) != n_files:
+            if len(v) != n_files or type(v) is not list:
                 _add_item_to_dict(tracking_files, metadata, k, v)
             else:
                 _add_items_to_dict(tracking_files, metadata, k, v)
         else:
             _add_item_to_dict(tracking_files, metadata, k, v)
 
     return metadata
@@ -562,15 +562,15 @@
             label_string = ','.join(label_strings)
 
             #ffmpeg is the fastest way to add this information to a video
             #Prepare the ffmpeg command
             cmd = f'ffmpeg -y -i {vid_in} -vf "{label_string}" {vid_out}'
             os.system(cmd)            
 
-def _create_from_dict(metadata, label_key, part_renamer, animal_renamer):
+def _create_from_dict(metadata, part_renamer, animal_renamer):
     df = pd.DataFrame()
     #req_cols = ['fps']
     #Drop requirement this is provided. Just omit addition of time column, if fps omitted
     req_cols = []
     is_valid, should_rescale = _validate_metadata(metadata, req_cols)
     if is_valid:   
         df.metadata.details = metadata
@@ -584,74 +584,69 @@
     if should_rescale:
         _convert_units(df)
     elif 'scale_factor' in df.columns: 
         df.drop(columns = 'scale_factor', inplace = True)
 
     return df    
 
-def _create_from_list(input, label_key, part_renamer, animal_renamer, **kwargs):
+def _create_from_list(input, part_renamer, animal_renamer, **kwargs):
     if len(input) == 0:
         return pd.DataFrame()
     supported_exts = ['.csv', '.h5', '.nwb', '.hdf5']
     exts = [os.path.splitext(m)[1] for m in input]
     supported = [e in supported_exts for e in exts]
-    is_nwb = [e == 'nwb' for e in exts]
+    is_nwb = [e == '.nwb' for e in exts]
     if not all(supported):
         ValueError("Only NWB, dlc (csv) or SLEAP (h5, hdf5) formats are supported.")
 
     if all(is_nwb):
         df = _load_nwb(input, part_renamer, animal_renamer)
     else:
         metadata = create_metadata(input, **kwargs)
-        df = _create_from_dict(metadata, label_key, part_renamer, animal_renamer)
+        df = _create_from_dict(metadata, part_renamer, animal_renamer)
 
     return df
 
 def create_dataset(input : dict = None, 
-                     label_key : dict = None, 
                      part_renamer : dict = None,
                      animal_renamer : dict = None,
                      video : list = None, 
                      labels : list = None,
                      **kwargs) -> pd.DataFrame:
     """Creates DataFrame that houses pose-tracking data and behavior annotations, along with relevant metadata, features and behavior annotation labels.
 
     Args:
         input: String OR list of strings with path(s) to tracking file(s). 
             OR Dictionary whose keys are pose tracking files, and value is a dictionary of associated metadata
             for that video (see `create_metadata` if using this construction option)
-        label_key: Default None. Dictionary whose keys are positive integers and values are behavior labels. If none, then this is inferred from the behavior annotation files provided.  
         part_renamer: Default None. Dictionary that can rename body parts from tracking files if needed (for feature creation, e.g.)
         animal_renamer: Default None. Dictionary that can rename animals from tracking files if needed
         **kwargs: Any other data to associate with each of the tracking files. This includes label files, and other metadata. 
             Any list-like arguments of appropriate length are zipped (associated) with each tracking file. See How To guide for more information.
         
     Returns:
         DataFrame object. This is a pandas DataFrame with additional metadata and methods.
     """
 
     if type(input) is dict:
-        df = _create_from_dict(input, label_key, part_renamer, animal_renamer)
+        df = _create_from_dict(input, part_renamer, animal_renamer)
     elif type(input) is str:
         if video is not None: kwargs['video'] = video 
         if labels is not None: kwargs['labels'] = labels
-        df = _create_from_list([input], label_key, part_renamer, animal_renamer, **kwargs)
+        df = _create_from_list([input], part_renamer, animal_renamer, **kwargs)
     elif type(input) is list:
         if video is not None: kwargs['video'] = video 
         if labels is not None: kwargs['labels'] = labels
-        df = _create_from_list(input, label_key, part_renamer, animal_renamer, **kwargs)
+        df = _create_from_list(input, part_renamer, animal_renamer, **kwargs)
     else:
         raise ValueError("Metadata not properly formatted. See docstring.")
 
-    if label_key:
-        df.metadata.label_key = label_key
-
     return df
 
-def _load_nwb(nwb_files, part_renamer, animal_renamer):
+def _load_nwb(nwb_files, part_renamer, animal_renamer, set_as_label = True):
 
     metadata = {}
     dfs = []
     col_names_old = None
     for fn in nwb_files:
         df_fn, body_parts, animals, col_names, scorer, meta = read_NWB_tracks(fn, 
                                                                               part_renamer, 
@@ -674,14 +669,21 @@
     #df[dfs.columns] = dfs
     df.reset_index(drop = True, inplace = True)
     df.metadata.details = metadata
     df.pose.body_parts = body_parts
     df.pose.animals = animals
     df.pose.animal_setup = {'mouse_ids': animals, 'bodypart_ids': body_parts, 'colnames': col_names}
     df.pose.raw_track_columns = col_names
+
+    label_cols = [x for x in df.columns if x.startswith('label_')]
+    df.metadata.label_key = {idx:k for idx, k in enumerate(list(set(label_cols)))}
+
+    if set_as_label:
+        df.ml.label_cols = list(df.metadata.label_key.values())
+
     return df
 
 def _load_tracks(df, part_renamer, animal_renamer, rescale = False):
     """Add tracks to DataFrame"""
     dfs = []
     col_names_old = None
     #Go through each video file and load tracks
@@ -746,44 +748,39 @@
             warnings.warn(f"One of the animal names is protected ({animal}), unexpected behavior may occur.")
     return col_names
 
 def _load_labels(df, col_name = 'label', set_as_label = False):
     #For the moment only BORIS support
     return _load_labels_boris(df, col_name, set_as_label)
 
-def _load_labels_boris(df, col_name = 'label', set_as_label = False):
+def _load_labels_boris(df, prefix = 'label', set_as_label = False):
     """Add behavior label data to DataFrame"""
 
-    if not df.metadata.label_key:
-        label_files = []
-        for fn in df.metadata.details.keys():
-            if 'labels' in df.metadata.details[fn]:
-                label_files.append(df.metadata.details[fn]['labels'])
-        df.metadata.label_key = create_behavior_labels(label_files)
-
     label_cols = []
     for vid in df.metadata.details:
         if 'labels' in df.metadata.details[vid] and 'fps' in df.metadata.details[vid]:
             fn_in = df.metadata.details[vid]['labels']
             fps = df.metadata.details[vid]['fps']
             duration = df.metadata.details[vid]['duration']
 
-            ground_truth = read_boris_annotation(fn_in, fps, duration, df.metadata.label_key.values())
+            ground_truth = read_boris_annotation(fn_in, fps, duration)
 
             for behavior in ground_truth:
-                col_name = 'label_' + behavior
+                col_name = prefix + '_' + behavior
                 label_cols.append(col_name)
                 if col_name not in df.columns:
                     df[col_name] = 0.
                 df.loc[df['filename'] == vid, col_name] = ground_truth[behavior]
         elif 'fps' not in df.metadata.details[vid]:
             print(f"'fps' not provided for video {vid}. Cannot link pose data to BORIS annotations.")
 
+    df.metadata.label_key = {idx:k for idx, k in enumerate(list(set(label_cols)))}
+
     if set_as_label:
-        df.ml.label_cols = list(set(label_cols))
+        df.ml.label_cols = list(df.metadata.label_key.values())
 
 def load_experiment(fn_in : str) -> pd.DataFrame:
     """Load DataFrame from file.
     
     Args:
         fn_in: path to file to load
```

### Comparing `ethome-ml-0.5.5/ethome_ml.egg-info/PKG-INFO` & `ethome-ml-0.6.0/ethome_ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethome-ml
-Version: 0.5.5
+Version: 0.6.0
 Summary: Tools for machine learning of animal behavior.
 Home-page: https://github.com/benlansdell/ethome
 Author: Ben Lansdell
 Author-email: ben.lansdell@gmail.com
 Project-URL: Bug Tracker, https://github.com/benlansdell/ethome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -56,26 +56,26 @@
 ```
 
 Create the dataframe:
 ```python
 dataset = create_dataset(fn_in)
 ```
 `dataset` is an extended pandas DataFrame, so can be treated exactly as you would treat any other dataframe. `ethome` adds a bunch of metadata about the dataset, for instance you can list the body parts with:
-```
+```python
 dataset.pose.body_parts
 ```
 
 A key functionality of `ethome` is the ability to easily create features for machine learning. You can use pre-built featuresets or make your own. For instance:
 ```python
 dataset.features.add('distances')
 ``` 
 will compute all distances between all body parts (both between and within animals).
 
 There are featuresets specifically tailored for social mice studies (resident intruder). For instance, 
-```
+```python
 dataset.features.add('cnn1d_prob')
 ```
 Uses a pretrained CNN to output probabilities of 3 behaviors (attack, mount, social investigation). For this, you must have labeled your body parts in a certain way (refer to How To). Other, more generic, feature creation functions are provided that work for any animal configuration. 
 
 Now you can access a features table, labels, and groups for learning with `dataset.ml.features, dataset.ml.labels, dataset.ml.group`. From here it's easy to use some ML libraries to train a behavior classifier. For example:
 ```python
 from sklearn.ensemble import RandomForestClassifier
@@ -103,9 +103,8 @@
 
 If the raw video file paths are provided in the metadata, under the `video` key, we can make a movie overlaying these predictions over the original video:
 ```python
 dataset.io.save_movie(['label', 'prediction'], '.')
 ```
 where `label` and `prediction` reference column names to annotate the video with.
 
-A more detailed run through of features is provided in the How To guide.
- 
+A more detailed run through of features is provided in the How To guide. Also checkout `examples` for working demos to quickly see how things work.
```

### Comparing `ethome-ml-0.5.5/ethome_ml.egg-info/SOURCES.txt` & `ethome-ml-0.6.0/ethome_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/setup.cfg` & `ethome-ml-0.6.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 	typeguard
 	typing
 	matplotlib
 	scikit-image
 	umap-learn
 	dill
 	pynwb
+	ipywidgets
 packages = find:
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	= .
 
 [options.packages.find]
```

### Comparing `ethome-ml-0.5.5/tests/test_analysis.py` & `ethome-ml-0.6.0/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/tests/test_io.py` & `ethome-ml-0.6.0/tests/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,17 +86,17 @@
     #Metadata is a dictionary that attaches each of the above parameters to the video/behavior annotations
     metadata = create_metadata(tracking_files, 
                               labels = label_files,
                               fps = fps)
 
     edf = create_dataset(metadata)
 
-    assert 'interact' in edf.metadata.label_key.values()
-    assert 'mount' in edf.metadata.label_key.values()
-    assert all(np.array(list(edf.metadata.label_key.keys())) > 0)
+    assert 'label_interact' in edf.metadata.label_key.values()
+    assert 'label_mount' in edf.metadata.label_key.values()
+    assert all(np.array(list(edf.metadata.label_key.keys())) >= 0)
 
 def test_sample_singlemouse_data_missing():
 
     import os 
     from glob import glob 
     from ethome import create_dataset, create_metadata
```

### Comparing `ethome-ml-0.5.5/tests/test_plot.py` & `ethome-ml-0.6.0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `ethome-ml-0.5.5/tests/test_unsupervised.py` & `ethome-ml-0.6.0/tests/test_unsupervised.py`

 * *Files identical despite different names*

