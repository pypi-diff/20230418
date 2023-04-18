# Comparing `tmp/seg2map-0.0.7.tar.gz` & `tmp/seg2map-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seg2map-0.0.7.tar", last modified: Mon Apr 17 16:16:42 2023, max compression
+gzip compressed data, was "seg2map-0.0.8.tar", last modified: Tue Apr 18 20:22:29 2023, max compression
```

## Comparing `seg2map-0.0.7.tar` & `seg2map-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:16:42.857835 seg2map-0.0.7/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-04-17 16:16:33.000000 seg2map-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-17 16:16:33.000000 seg2map-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-04-17 16:16:42.857835 seg2map-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17716 2023-04-17 16:16:33.000000 seg2map-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-17 16:16:33.000000 seg2map-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:16:42.857835 seg2map-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-17 16:16:33.000000 seg2map-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:16:42.853835 seg2map-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:16:42.853835 seg2map-0.0.7/src/seg2map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55318 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    32288 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/log_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/map_UI.py
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/map_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    53017 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/map_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    24669 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/model_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/models_UI.py
--rw-r--r--   0 runner    (1001) docker     (123)    35003 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/new_downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/roi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)    40888 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/zoo_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:16:42.857835 seg2map-0.0.7/src/seg2map.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-04-17 16:16:42.000000 seg2map-0.0.7/src/seg2map.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-17 16:16:42.000000 seg2map-0.0.7/src/seg2map.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:16:42.000000 seg2map-0.0.7/src/seg2map.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 16:16:42.000000 seg2map-0.0.7/src/seg2map.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 16:16:42.000000 seg2map-0.0.7/src/seg2map.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:22:29.397714 seg2map-0.0.8/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-04-18 20:22:15.000000 seg2map-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-18 20:22:15.000000 seg2map-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-04-18 20:22:29.397714 seg2map-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17716 2023-04-18 20:22:15.000000 seg2map-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-18 20:22:15.000000 seg2map-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:22:29.397714 seg2map-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-18 20:22:15.000000 seg2map-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:22:29.393713 seg2map-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:22:29.397714 seg2map-0.0.8/src/seg2map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58158 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32288 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/log_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/map_UI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/map_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53017 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/map_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24669 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/model_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/models_UI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35003 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/new_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42245 2023-04-18 20:22:15.000000 seg2map-0.0.8/src/seg2map/zoo_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:22:29.397714 seg2map-0.0.8/src/seg2map.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-04-18 20:22:29.000000 seg2map-0.0.8/src/seg2map.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-18 20:22:29.000000 seg2map-0.0.8/src/seg2map.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:22:29.000000 seg2map-0.0.8/src/seg2map.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-18 20:22:29.000000 seg2map-0.0.8/src/seg2map.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 20:22:29.000000 seg2map-0.0.8/src/seg2map.egg-info/top_level.txt
```

### Comparing `seg2map-0.0.7/LICENSE` & `seg2map-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.7/PKG-INFO` & `seg2map-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seg2map
-Version: 0.0.7
+Version: 0.0.8
 Summary: An interactive jupyter notebook for downloading satellite imagery
 Author-email:  Sharon Fitzpatrick <sharon.fitzpatrick23@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Doodleverse
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `seg2map-0.0.7/README.md` & `seg2map-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.7/pyproject.toml` & `seg2map-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seg2map"
 dynamic = ["readme"]
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name=" Sharon Fitzpatrick", email="sharon.fitzpatrick23@gmail.com" },
 ]
 # find` directive with `include` or `exclude`
 description = "An interactive jupyter notebook for downloading satellite imagery"
 dependencies = [
   "scikit-image",
```

### Comparing `seg2map-0.0.7/src/seg2map/common.py` & `seg2map-0.0.8/src/seg2map/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,27 +106,101 @@
     """
     png_files = []
     npzs = sorted(glob(os.path.join(full_path, "*.npz")))
     for npz in npzs:
         png_files.append(write_greylabel_to_png(npz))
     return png_files
 
+def validate_is_roi_directory(base_path: str) -> bool:
+    """
+    Validates if the given base_path is a Region of Interest (ROI) directory by checking for the presence of
+    both a "multiband" subdirectory and a "config" file.
+
+    Args:
+        base_path (str): The path to the base directory to be validated.
+
+    Returns:
+        bool: True if base_path contains the "multiband" subdirectory and the "config" file, otherwise False.
+    """
+    
+    # Flags to check for the existence of the required items
+    has_mulitband = False
+    has_config = False
+
+    # Iterate over items in the directory
+    for item in base_path.iterdir():
+        # Check if the item is a directory and starts with "multiband"
+        if item.is_dir() and item.name.startswith("multiband"):
+            has_mulitband = True
+
+        # Check if the item is a file and starts with "config"
+        if item.is_file() and item.name.startswith("config"):
+            has_config = True
+
+    # Return True if both the "multiband" directory and the "config" file are found in base_path
+    return has_mulitband and has_config
 
 def get_subdirectories_with_ids(base_path: str) -> dict:
-    all_items = os.listdir(base_path)
+    """
+    This function takes a base path as input and returns a dictionary containing
+    the IDs and paths of the parent directory as well as any subdirectories that start with "ID_".
+    
+    Args:
+        base_path (str): The base path to search for subdirectories.
+        
+    Returns:
+        dict: A dictionary with IDs as keys and subdirectory paths as values.
+    """
+    base_path = Path(base_path)
     subdirs_with_ids = {}
 
-    for item in all_items:
-        item_path = os.path.join(base_path, item)
-        if os.path.isdir(item_path) and item.startswith("ID_"):
-            id = item.split("_")[1]
-            subdirs_with_ids[id] = item_path
+    if base_path.exists():
+        if base_path.is_dir() and base_path.name.startswith("ID_"):
+            # make sure this is a valid ROI directory and not just a directory with an ID
+            if validate_is_roi_directory(base_path):
+                    roi_id = base_path.name.split("_")[1]
+                    subdirs_with_ids[roi_id]=str(base_path)
+
+    for item in base_path.iterdir():
+        if item.is_dir() and item.name.startswith("ID_"):
+            roi_id = item.name.split("_")[1]
+            subdirs_with_ids[roi_id] = str(item)
 
     return subdirs_with_ids
 
+def check_id_subdirectories_exist(base_path: str) -> bool:
+    """
+    Check if any subdirectories with names starting with "ID_" exist in the given base_path.
+
+    Args:
+        base_path (str): The absolute or relative path to the directory to look in.
+
+    Returns:
+        bool: True if any subdirectories with names starting with "ID_" are found, otherwise False.
+    """
+    # Check if the given base_path exists
+    if not os.path.exists(base_path):
+        return False
+
+    # Convert base_path to a Path object
+    base_path = Path(base_path)
+
+    # Check if the base_path itself meets the condition
+    if base_path.is_dir() and base_path.name.startswith("ID_"):
+        return True
+
+    # Iterate over the items in the base_path
+    for item in base_path.iterdir():
+        # Check if the item is a subdirectory and if its name starts with "ID_"
+        if item.is_dir() and item.name.startswith("ID_"):
+            return True
+
+    # If no subdirectories with names starting with "ID_" are found, return False
+    return False
+
 
 def extract_roi_id_from_path(path):
     """
     Extracts roi_id from a directory name in a given path.
 
     The function assumes that the directory name is in the format "ID_{roiid}_dates_*".
```

### Comparing `seg2map-0.0.7/src/seg2map/downloads.py` & `seg2map-0.0.8/src/seg2map/downloads.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.7/src/seg2map/exception_handler.py` & `seg2map-0.0.8/src/seg2map/exception_handler.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.7/src/seg2map/exceptions.py` & `seg2map-0.0.8/src/seg2map/exceptions.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.7/src/seg2map/log_maker.py` & `seg2map-0.0.8/src/seg2map/log_maker.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.7/src/seg2map/map_UI.py` & `seg2map-0.0.8/src/seg2map/map_UI.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.7/src/seg2map/map_functions.py` & `seg2map-0.0.8/src/seg2map/map_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     color_map = {}
     for i, color in enumerate(rgb_colors):
         color_map[i] = tuple(int(255 * c) for c in color)
 
     return color_map
 
 
-@time_func
+# @time_func
 def generate_class_masks(file: str, class_mapping: dict, save_path: str) -> List[str]:
     """
     Generate binary masks for each class in the given grayscale image, based on a color-to-class mapping.
 
     Args:
         file (str): The path to the grayscale input image file.
         class_mapping (dict): A dictionary that maps pixel colors to class names.
```

### Comparing `seg2map-0.0.7/src/seg2map/map_interface.py` & `seg2map-0.0.8/src/seg2map/map_interface.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.7/src/seg2map/model_functions.py` & `seg2map-0.0.8/src/seg2map/model_functions.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.7/src/seg2map/models_UI.py` & `seg2map-0.0.8/src/seg2map/models_UI.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,15 +254,15 @@
         """
         self.line_widget = HTML(
             value="____________________________________________________"
         )
 
         self.instr_select_images = HTML(
             value="<b>1. Select Images</b> \
-                <br> - Select multiband directory within an ROI directory",
+                <br> - Select an ROI directory or a directory containing at least one ROI subdirectory.\nExample: ./data/dataset1/ID_e7CxBi_dates_2010-01-01_to_2014-12-31",
             layout=Layout(margin="0px 0px 0px 20px"),
         )
 
         self.instr_run_model = HTML(
             value="<b>2. Run Model </b> \
                 <br> - Click Select Images first, then click run model",
             layout=Layout(margin="0px 0px 0px 20px"),
@@ -321,39 +321,44 @@
             return
         if inputs_directory == "":
             self.launch_error_box(
                 "Cannot Run Model",
                 "Must click 'Select Images' first",
             )
             return
+        if not common.check_id_subdirectories_exist(inputs_directory):
+            self.launch_error_box(
+                "Cannot Run Model",
+                "You must select a directory that contains ROI subdirectories. Example ROI name: 'ID_e7CxBi_dates_2010-01-01_to_2014-12-31'",
+            )
+            return
         # Disable run and open results buttons while the model is running
-        # self.open_results_button.disabled = True
-        # self.run_model_button.disabled = True
+        self.run_model_button.disabled = True
 
         # gets GPU or CPU depending on whether use_GPU is True
         use_GPU = self.model_dict["use_GPU"]
         model_implementation = self.model_dict["implementation"]
         model_id = self.model_dict["model_type"]
         use_otsu = self.model_dict["otsu"]
         use_tta = self.model_dict["tta"]
 
         zoo_model_instance = zoo_model.ZooModel()
-
-        zoo_model_instance.run_model(
-            model_implementation,
-            session_name=session_name,
-            src_directory=inputs_directory,
-            model_id=model_id,
-            use_GPU=use_GPU,
-            use_otsu=use_otsu,
-            use_tta=use_tta,
+        try:
+            zoo_model_instance.run_model(
+                model_implementation,
+                session_name=session_name,
+                src_directory=inputs_directory,
+                model_id=model_id,
+                use_GPU=use_GPU,
+                use_otsu=use_otsu,
+                use_tta=use_tta,
         )
-        # # Enable run and open results buttons when model has executed
-        # self.run_model_button.disabled = False
-        # self.open_results_button.disabled = False
+        finally:
+            # Enable run and open results buttons when model has executed
+            self.run_model_button.disabled = False
 
     @run_model_view.capture(clear_output=True)
     def open_results_button_clicked(self, button):
         """open_results_button_clicked on click handler for 'open results' button.
 
         prints location of model outputs
```

### Comparing `seg2map-0.0.7/src/seg2map/new_downloads.py` & `seg2map-0.0.8/src/seg2map/new_downloads.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.7/src/seg2map/roi.py` & `seg2map-0.0.8/src/seg2map/roi.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.7/src/seg2map/sessions.py` & `seg2map-0.0.8/src/seg2map/sessions.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.7/src/seg2map/zoo_model.py` & `seg2map-0.0.8/src/seg2map/zoo_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from typing import List, Set
+from typing import Dict, List, Set
+from typing import Dict, Any
 import requests
 import logging
 import os
 import shutil
 import json
+from pathlib import Path
 from glob import glob
 
 from seg2map import common
 from seg2map import downloads
 from seg2map import sessions
 from seg2map import map_functions
 
@@ -27,14 +29,83 @@
     segformer,
 )
 from doodleverse_utils.model_imports import dice_coef_loss, iou_multi, dice_multi
 import tensorflow as tf
 
 logger = logging.getLogger(__name__)
 
+def process_roi(roi_path: str, model_dict: dict) -> Dict:
+    """
+    Process a Region of Interest (ROI) directory and return a dictionary containing the
+    processed data for each year within the ROI.
+
+    Args:
+        roi_path (str): The path to the ROI directory.
+        model_dict (dict): A dictionary containing model-specific configuration data.
+
+    Returns:
+        Dict: A dictionary where keys are the years (e.g., '2010', '2011', ...) and
+              values are dictionaries containing model configuration data specific to
+              that year, including the path to the preprocessed data directory for
+              that year. For example:
+
+                  {
+                      '2010': {"model_type": "OpenEarthNet_RGB_9class_7576894",, 'sample_direc': '/path/to/roi/2010/data', ...},
+                      '2011': {"model_type": "OpenEarthNet_RGB_9class_7576894",, 'sample_direc': '/path/to/roi/2011/data', ...},
+                      ...
+                  }
+
+    Example usage:
+        roi_path = '/path/to/roi_directory'
+        model_dict = {'model_param1': value1, 'model_param2': value2, ...}
+        model_data_per_year = process_roi(roi_path, model_dict)
+    """
+    model_data_per_year = {}
+    multiband_path = os.path.join(roi_path, "multiband")
+    year_dirs = common.get_matching_dirs(multiband_path, pattern=r"^\d{4}$")
+    
+    for year_dir in tqdm.auto.tqdm(year_dirs, desc="Preparing data", leave=False, unit_scale=True):
+        model_year_dict = process_year_directory(year_dir, model_dict)
+        
+        if model_year_dict:
+            year_key = os.path.basename(year_dir)
+            model_data_per_year[year_key] = model_year_dict
+    
+    return model_data_per_year
+
+def process_year_directory(year_dir: str, model_dict: Dict[str, Any]) -> Dict[str, Any]:
+    """
+    Process a year's directory of multispectral images by creating overlapping tiles,
+    and update the model dictionary with the new sample directory.
+
+    Args:
+        year_dir (str): Path to the year's directory containing multispectral images.
+        model_dict (Dict[str, Any]): The original model dictionary.
+
+    Returns:
+        Dict[str, Any]: The updated model dictionary with the new sample directory, or None if input directory is empty.
+
+    """
+    if len(os.listdir(year_dir)) == 0:
+        logger.warning(f"len(os.listdir({year_dir})) == 0")
+        return {}
+    # Construct the file path to the original merged multispectral image
+    original_merged_tif = os.path.join(year_dir, "merged_multispectral.tif")
+    # Create a new "tiles" directory within the year_dir
+    tiles_path = common.create_directory(year_dir, "tiles")
+    # Generate overlapping tiles from the original merged multispectral image and get the new tiles path
+    tiles_path = create_overlapping_tiles(original_merged_tif, tiles_path)
+    # Check if the returned tiles_path is empty or None, log a warning and return an empty dictionary if true
+    if tiles_path == "" or tiles_path is None:
+        logger.warning(f"Empty or None tiles_path for {year_dir}")
+        return {}
+    # Create a copy of the model dictionary and update the sample directory with the new tiles path
+    model_year_dict = model_dict.copy()
+    model_year_dict["sample_direc"] = tiles_path
+    return model_year_dict
 
 def get_sorted_files_with_extension(
     sample_direc: str, file_extensions: List[str]
 ) -> List[str]:
     """
     Get a sorted list of paths to files that have one of the file_extensions.
     It will return the first set of files that matches the first file_extension, so put the
@@ -52,16 +123,15 @@
     for ext in file_extensions:
         filenames = sorted(tf.io.gfile.glob(os.path.join(sample_direc, f"*{ext}")))
         sample_filenames.extend(filenames)
         if sample_filenames:
             break
     return sample_filenames
 
-
-def write_greylabel_to_png(npz_location: str) -> str:
+def save_greyscale_label_as_png(npz_location: str) -> str:
     """
     Given the path of an .npz file containing a 'grey_label' key with an array of uint8 values,
     writes the array to a PNG file with the same name and location as the .npz file, with the extension
     changed to .png. Returns the path of the PNG file.
 
     Parameters:
     npz_location (str): The path of the .npz file to read from.
@@ -71,16 +141,15 @@
     """
     png_path = npz_location.replace(".npz", ".png")
     with np.load(npz_location) as data:
         dat = 1 + np.round(data["grey_label"].astype("uint8"))
     imsave(png_path, dat, check_contrast=False, compression=0)
     return png_path
 
-
-def create_greylabel_pngs(full_path: str) -> List[str]:
+def generate_greyscale_label_pngs(full_path: str) -> List[str]:
     """
     Given a directory path, finds all .npz files in the directory, writes the 'grey_label' array of each .npz
     file to a corresponding PNG file, and returns a list of the paths of the written PNG files.
 
     Parameters:
     full_path (str): The path of the directory to search for .npz files.
 
@@ -88,44 +157,66 @@
     List[str]: A list of the paths of the written PNG files.
     """
     png_files = []
     logger.info(f"full_path: {full_path}")
     npzs = sorted(glob(os.path.join(full_path, "*.npz")))
     logger.info(f"npzs: {npzs}")
     for npz in npzs:
-        png_files.append(write_greylabel_to_png(npz))
+        png_files.append(save_greyscale_label_as_png(npz))
     return png_files
 
-
-def rename_xmls(src, old_name, new_name):
-    xml_files = sorted(glob(os.path.join(src, "*.xml")))
-    ## rename xmls
+def rename_xmls(src: str, old_name: str, new_name: str) -> None:
+    """
+    Renames all .xml files in the source directory by replacing 'old_name' with 'new_name'.
+    
+    Parameters:
+    src (str): The path of the source directory containing .xml files.
+    old_name (str): The old substring to be replaced in the .xml filenames.
+    new_name (str): The new substring to replace the 'old_name' in the .xml filenames.
+    """
+    xml_files = sorted(Path(src).glob("*.xml"))
     for xml_file in xml_files:
-        new_filename = xml_file.replace(old_name, new_name)
-        if not os.path.isfile(new_filename):
-            os.rename(xml_file, new_filename)
+        new_filename = str(xml_file).replace(old_name, new_name)
+        if not Path(new_filename).is_file():
+            xml_file.rename(new_filename)
 
+def copy_xmls(src: str, dst: str) -> None:
+    """
+    Copies all .xml files from the source directory to the destination directory.
 
-def copy_xmls(src, dst):
-    ## copy the xml files into the 'out' folder
-    xml_files = sorted(glob(os.path.join(src, "*.xml")))
+    Parameters:
+    src (str): The path of the source directory containing .xml files.
+    dst (str): The path of the destination directory where .xml files will be copied.
+    """
+    xml_files = sorted(Path(src).glob("*.xml"))
     for xml_file in xml_files:
-        new_filename = xml_file.replace(src, dst)
-        if not os.path.isfile(new_filename):
-            shutil.copyfile(xml_file, new_filename)
+        new_filename = str(xml_file).replace(src, dst)
+        if not Path(new_filename).is_file():
+            shutil.copyfile(str(xml_file), new_filename)
 
 
-def remove_unused_files(outputs_path):
-    # Remove "prob.png" files
-    _ = [os.remove(k) for k in glob(os.path.join(outputs_path, "*prob.png"))]
-    # Remove "overlay.png" files ...
-    _ = [os.remove(k) for k in glob(os.path.join(outputs_path, "*overlay.png"))]
+def remove_unused_files(outputs_path: str) -> None:
+    """
+    Removes unused files (e.g., 'prob.png' and 'overlay.png') from the specified directory.
 
+    Parameters:
+    outputs_path (str): The path of the directory containing unused files to be removed.
+    """
+    for file_extension in ["*prob.png", "*overlay.png"]:
+        for unused_file in Path(outputs_path).glob(file_extension):
+            unused_file.unlink()
 
-def rename_predictions(predictions_location):
+
+def rename_predictions(predictions_location: str) -> None:
+    """
+    Renames prediction PNG files in the specified directory by removing the '_predseg' suffix.
+
+    Parameters:
+    predictions_location (str): The path of the directory containing prediction PNG files.
+    """
     # find predictions and rename
     # Get imgs list
     predicition_pngs = sorted(glob(os.path.join(predictions_location, "*.png")))
     # rename pngs
     for prediction in predicition_pngs:
         new_filename = prediction.replace("_predseg", "")
         if not os.path.isfile(new_filename):
@@ -151,15 +242,15 @@
     outputs_path = os.path.join(tiles_location, "out")
     logger.info(f"outputs_path: {outputs_path}")
     # copy xmls to the out folder
     copy_xmls(tiles_location, outputs_path)
     rename_xmls(outputs_path, ".jpg.aux.xml", ".png.aux.xml")
     rename_predictions(outputs_path)
     # create pngs from the npz files (segmentations)
-    imgsToMosaic = create_greylabel_pngs(outputs_path)
+    imgsToMosaic = generate_greyscale_label_pngs(outputs_path)
     if len(imgsToMosaic) == 0:
         logger.warning("No segmented images were found")
         return ""
     # rename the segmented images
     rename_xmls(outputs_path, ".png", "_res.png")
     outVRT = os.path.join(tif_location, "Mosaic_greyscale.vrt")
     outTIF = os.path.join(tif_location, "Mosaic_greyscale.tif")
@@ -182,14 +273,15 @@
     kwargs = {"format": "JPEG", "outputType": gdal.GDT_Byte}
     # create jpgs for new tifs
     common.gdal_translate_jpegs(tif_files, kwargs=kwargs)
     # delete tif files
     for file in tif_files:
         os.remove(file)
     if len(os.listdir(tiles_path)) == 0:
+        logger.warning(f"{tiles_path} is empty. No tiles were created.")
         return None
     return tiles_path
 
 
 def download_url(
     url: str, save_path: str, progress_bar_name: str = "", chunk_size: int = 1024
 ):
@@ -445,69 +537,46 @@
         # if any files are not found locally download them asynchronous
         if download_dict != {}:
             downloads.run_async_function(
                 downloads.async_download_url_dict, url_dict=download_dict
             )
 
     def get_model(self, weights_list: list):
+        if not weights_list:
+            raise Exception("No Model Info Passed")
+    
         model_list = []
         config_files = []
         model_types = []
-        if weights_list == []:
-            raise Exception("No Model Info Passed")
-        for weights in weights_list:
-            # "fullmodel" is for serving on zoo they are smaller and more portable between systems than traditional h5 files
-            # gym makes a h5 file, then you use gym to make a "fullmodel" version then zoo can read "fullmodel" version
-            configfile = (
-                weights.replace(".h5", ".json").replace("weights", "config").strip()
-            )
-            if "fullmodel" in configfile:
-                configfile = configfile.replace("_fullmodel", "").strip()
-            with open(configfile) as f:
+    
+        for weights_path in weights_list:
+            weights_path = Path(weights_path)
+            config_path = weights_path.with_name(weights_path.stem.replace("weights", "config")).with_suffix(".json")
+    
+            if "fullmodel" in config_path.name:
+                config_path = config_path.with_name(config_path.stem.replace("_fullmodel", "") + config_path.suffix)
+    
+            with config_path.open() as f:
                 config = json.load(f)
+    
             self.TARGET_SIZE = config.get("TARGET_SIZE")
             MODEL = config.get("MODEL")
             self.NCLASSES = config.get("NCLASSES")
             KERNEL = config.get("KERNEL")
             STRIDE = config.get("STRIDE")
             FILTERS = config.get("FILTERS")
             self.N_DATA_BANDS = config.get("N_DATA_BANDS")
             DROPOUT = config.get("DROPOUT")
             DROPOUT_CHANGE_PER_LAYER = config.get("DROPOUT_CHANGE_PER_LAYER")
             DROPOUT_TYPE = config.get("DROPOUT_TYPE")
             USE_DROPOUT_ON_UPSAMPLING = config.get("USE_DROPOUT_ON_UPSAMPLING")
-            DO_TRAIN = config.get("DO_TRAIN")
-            LOSS = config.get("LOSS")
-            PATIENCE = config.get("PATIENCE")
-            MAX_EPOCHS = config.get("MAX_EPOCHS")
-            VALIDATION_SPLIT = config.get("VALIDATION_SPLIT")
-            RAMPUP_EPOCHS = config.get("RAMPUP_EPOCHS")
-            SUSTAIN_EPOCHS = config.get("SUSTAIN_EPOCHS")
-            EXP_DECAY = config.get("EXP_DECAY")
-            START_LR = config.get("START_LR")
-            MIN_LR = config.get("MIN_LR")
-            MAX_LR = config.get("MAX_LR")
-            FILTER_VALUE = config.get("FILTER_VALUE")
-            DOPLOT = config.get("DOPLOT")
-            ROOT_STRING = config.get("ROOT_STRING")
-            USEMASK = config.get("USEMASK")
-            AUG_ROT = config.get("AUG_ROT")
-            AUG_ZOOM = config.get("AUG_ZOOM")
-            AUG_WIDTHSHIFT = config.get("AUG_WIDTHSHIFT")
-            AUG_HEIGHTSHIFT = config.get("AUG_HEIGHTSHIFT")
-            AUG_HFLIP = config.get("AUG_HFLIP")
-            AUG_VFLIP = config.get("AUG_VFLIP")
-            AUG_LOOPS = config.get("AUG_LOOPS")
-            AUG_COPIES = config.get("AUG_COPIES")
-            REMAP_CLASSES = config.get("REMAP_CLASSES")
 
             try:
-                model = tf.keras.models.load_model(weights)
-                #  nclasses=NCLASSES, may have to replace nclasses with NCLASSES
-            except BaseException:
+                model = tf.keras.models.load_model(str(weights_path))
+            except Exception:
                 if MODEL == "resunet":
                     model = custom_resunet(
                         (self.TARGET_SIZE[0], self.TARGET_SIZE[1], self.N_DATA_BANDS),
                         FILTERS,
                         nclasses=[
                             self.NCLASSES + 1 if self.NCLASSES == 1 else self.NCLASSES
                         ][0],
@@ -530,15 +599,14 @@
                         dropout=DROPOUT,  # 0.1,
                         dropout_change_per_layer=DROPOUT_CHANGE_PER_LAYER,  # 0.0,
                         dropout_type=DROPOUT_TYPE,  # "standard",
                         use_dropout_on_upsampling=USE_DROPOUT_ON_UPSAMPLING,  # False,
                     )
 
                 elif MODEL == "simple_resunet":
-                    # num_filters = 8 # initial filters
                     model = simple_resunet(
                         (self.TARGET_SIZE[0], self.TARGET_SIZE[1], self.N_DATA_BANDS),
                         kernel=(2, 2),
                         num_classes=[
                             self.NCLASSES + 1 if self.NCLASSES == 1 else self.NCLASSES
                         ][0],
                         activation="relu",
@@ -579,39 +647,33 @@
                         dropout_type=DROPOUT_TYPE,
                         use_dropout_on_upsampling=USE_DROPOUT_ON_UPSAMPLING,
                         filters=FILTERS,
                         num_layers=4,
                         strides=(1, 1),
                     )
                 elif MODEL == "segformer":
-                    id2label = {}
-                    for k in range(self.NCLASSES):
-                        id2label[k] = str(k)
+                    id2label = {k: str(k) for k in range(self.NCLASSES)}
                     model = segformer(id2label, num_classes=self.NCLASSES)
                     model.compile(optimizer="adam")
-                # 242,812
                 else:
                     raise Exception(
                         f"An unknown model type {MODEL} was received. Please select a valid model.\n \
                         Model must be one of 'unet', 'resunet', 'segformer', or 'satunet'"
                     )
-
-                # Load in the custom loss function from doodleverse_utils
-                model.compile(
-                    optimizer="adam", loss=dice_coef_loss(self.NCLASSES)
-                )  # , metrics = [iou_multi(self.NCLASSESNCLASSES), dice_multi(self.NCLASSESNCLASSES)])
-
-                model.load_weights(weights)
-
+    
+                model.compile(optimizer="adam", loss=dice_coef_loss(self.NCLASSES))
+                model.load_weights(str(weights_path))
+    
             model_types.append(MODEL)
             model_list.append(model)
-            config_files.append(configfile)
-
+            config_files.append(str(config_path))
+    
         return model, model_list, config_files, model_types
 
+
     def get_files_for_seg(
         self, sample_direc: str, avoid_patterns: List[str] = []
     ) -> list:
         """
         Returns a list of files to be segmented.
 
         The function reads in the image filenames as either (`.npz`) OR (`.jpg`, or `.png`)
@@ -629,49 +691,48 @@
             sample_direc, file_extensions
         )
         # filter out files whose filenames match any of the avoid_patterns
         sample_filenames = common.filter_files(sample_filenames, avoid_patterns)
         logger.info(f"files to seg: {sample_filenames}")
         return sample_filenames
 
+
     def preprocess_data(
         self, src_directory: str, model_dict: dict, session: sessions.Session
-    ):
+    )-> dict:
+        """
+        Preprocesses the data for regions of interest (ROIs) given a source directory
+        and a dictionary containing model information.
+        
+        Args:
+        - src_directory (str): Path to the source directory containing the ROIs.
+        - model_dict (dict): Dictionary containing key-value pairs related to the model.
+        - session (Session): A session object which holds other essential data.
+
+        Returns:
+        - preprocessed_data (dict): A dictionary containing preprocessed data for each
+          ROI for a specific year, including the path to the ROI.
+
+        """
         # load year directories for each ROI
         roi_dict = common.get_subdirectories_with_ids(src_directory)
+        logger.info(f"roi_dict: {roi_dict}")
+        
         session.roi_ids = list(roi_dict.keys())
-
         # create dictionary to run on model on for each year in each ROI
         preprocessed_data = {}
         for roi_id, roi_path in roi_dict.items():
             # for each year create overlapping tiles and save location of tiles
-            model_data_per_year = {}
-            multiband_path = os.path.join(roi_path, "multiband")
-            year_dirs = common.get_matching_dirs(multiband_path, pattern=r"^\d{4}$")
-            for year_dir in tqdm.auto.tqdm(
-                year_dirs, desc="Preparing data", leave=False, unit_scale=True
-            ):
-                if len(os.listdir(year_dir)) == 0:
-                    continue
-                original_merged_tif = os.path.join(year_dir, "merged_multispectral.tif")
-                tiles_path = common.create_directory(year_dir, "tiles")
-                tiles_path = create_overlapping_tiles(original_merged_tif, tiles_path)
-                if tiles_path == "":
-                    continue
-                model_year_dict = model_dict.copy()
-                model_year_dict["sample_direc"] = tiles_path
-                # use year name as the key ex.{ roi_id: '2010':{},'2011':{}}
-                model_data_per_year[os.path.basename(year_dir)] = model_year_dict
-                model_data_per_year["roi_path"] = roi_path
-            # if ROI directory had no years then skip it
-            if len(year_dirs) == 0:
-                continue
-            preprocessed_data[roi_id] = model_data_per_year
-
+            model_data_per_year = process_roi(roi_path, model_dict)
+            if model_data_per_year:
+                preprocessed_data[roi_id] = model_data_per_year
+                preprocessed_data[roi_id]["roi_path"] = roi_path
+                
         logger.info(f"preprocessed_data: {preprocessed_data}")
+
         return preprocessed_data
 
     def compute_segmentation(
         self,
         preprocessed_data: dict,
     ):
         """
@@ -685,28 +746,27 @@
             None.
 
         Raises:
             None.
         """
         # perform segmentations for each year in each ROI
         for roi_data in preprocessed_data.values():
+
             for key in roi_data.keys():
                 if key == "roi_path":
                     continue
-                logger.info(f"key: {key}")
-                logger.info(f"roi_data[key]: {roi_data[key]}")
+                logger.info(f"roi_data[{key}]: {roi_data[key]}")
                 sample_direc = roi_data[key]["sample_direc"]
                 use_tta = roi_data[key]["tta"]
                 use_otsu = roi_data[key]["otsu"]
                 files_to_segment = self.get_files_for_seg(sample_direc)
                 logger.info(f"files_to_segment: {files_to_segment}")
                 if self.model_types[0] != "segformer":
                     ### mixed precision
                     from tensorflow.keras import mixed_precision
-
                     mixed_precision.set_global_policy("mixed_float16")
                 # run model for each file
                 for file_to_seg in tqdm.auto.tqdm(files_to_segment):
                     do_seg(
                         file_to_seg,
                         self.model_list,
                         self.metadata_dict,
@@ -719,87 +779,52 @@
                         WRITE_MODELMETADATA=False,
                         OTSU_THRESHOLD=use_otsu,
                         out_dir_name="out",
                         profile="meta",
                     )
 
     def postprocess_data(self, preprocessed_data: dict, session: sessions.Session):
-        """
-        Preprocesses the outputs of the model by preparing moving the outputs to the session directory and creating a mask for each
-        class in the output. For example if the model outputs 3 classes then this will create 3 masks for each year in each ROI.
-
-        Args:
-            src_directory (str): The path to the directory containing the multispectral images to be segmented.
-            model_dict (dict): A dictionary containing the model configuration.
-            session (sessions.Session): A session object to keep track of segmentation parameters and results.
-
-        Returns:
-            dict: A dictionary containing the preprocessed the outputs of the model.
-
-        Raises:
-            None.
-        """
-        # get roi_ids
-        for roi_id in preprocessed_data.keys():
-            # create session roi directories
+        if preprocessed_data == {}:
+            raise Exception("No data to postprocess. You may not have selected a valid directory.")
+        # save preprocessed data to session directory
+        preprocessed_data_path = os.path.join(session.path, "preprocessed_data.json")
+        common.write_to_json(preprocessed_data_path, preprocessed_data)
+        # save segmentations & config files to session directory
+        for roi_id, roi_data in preprocessed_data.items():
             roi_session_directory = common.create_directory(session.path, roi_id)
-            # copy config files to session directory
+            # roi_directory = roi_data["roi_path"]
             roi_directory = preprocessed_data[roi_id]["roi_path"]
+            # copy config files to session directory
             self.copy_configs(roi_directory, roi_session_directory)
 
-            for key in preprocessed_data[roi_id].keys():
-                if key == "roi_path":
+            for year_key in roi_data.keys():
+                print(f"Saving segmentations for year {year_key}")
+                if year_key == "roi_path":
                     continue
-                year = key
-                session.add_years(year)
-                # create session year sub directories
-                year_session_directory = common.create_directory(
-                    roi_session_directory, year
-                )
-                tiles_path = preprocessed_data[roi_id][year]["sample_direc"]
-                # move 'tiles' to session directories
-                session_tiles_path = common.create_directory(
-                    year_session_directory, "tiles"
-                )
+                session.add_years(year_key)
+                year_session_directory = common.create_directory(roi_session_directory, year_key)
+                tiles_path = preprocessed_data[roi_id][year_key]["sample_direc"]
+                session_tiles_path = common.create_directory(year_session_directory, "tiles")
                 common.move_files_resurcively(src=tiles_path, dest=session_tiles_path)
-                # remove empty tiles directory
                 if os.path.basename(tiles_path).lower() == "tiles":
                     os.rmdir(tiles_path)
-                # save model settings
-                model_settings_path = os.path.join(
-                    year_session_directory, "model_settings.json"
-                )
-                common.write_to_json(
-                    model_settings_path, preprocessed_data[roi_id][year]
-                )
-                # merge tiles to create greyscale tif
-                # outputs of model are in session_name/ROI_ID/year/tiles/out
-                greyscale_tif = make_greyscale_tif(
-                    session_tiles_path, year_session_directory
-                )
+                model_settings_path = os.path.join(year_session_directory, "model_settings.json")
+                common.write_to_json(model_settings_path, preprocessed_data[roi_id][year_key])
+
+                greyscale_tif = make_greyscale_tif(session_tiles_path, year_session_directory)
                 if not greyscale_tif:
-                    logger.info(f"Year {year} could not generate a  greyscale tif")
+                    logger.info(f"Year {year_key} could not generate a greyscale tif")
                     continue
-                # create class mask pngs for each merged tif
-                # get class names to create class mapping
-                class_mapping = map_functions.get_class_mapping(session.classes)
-                # see if any class masks already exist in directory and if they don't exist then create them
-                class_masks_filenames = map_functions.get_existing_class_files(
-                    year_session_directory, session.classes
-                )
 
-                # in year_session_directory make a separate png containing all the pixels in each class within the tif
+                class_mapping = map_functions.get_class_mapping(session.classes)
+                class_masks_filenames = map_functions.get_existing_class_files(year_session_directory, session.classes)
                 if not class_masks_filenames:
-                    class_masks_filenames = map_functions.generate_class_masks(
-                        greyscale_tif, class_mapping, year_session_directory
-                    )
+                    class_masks_filenames = map_functions.generate_class_masks(greyscale_tif, class_mapping, year_session_directory)
 
-        # save session copy_configssettings
-        preprocessed_data_path = os.path.join(session.path, "preprocessed_data.json")
-        common.write_to_json(preprocessed_data_path, preprocessed_data)
+        print(f"Segmentations saved at {session.path}")
         session.save(session.path)
 
     def copy_configs(self, src: str, dst: str) -> None:
         """
         Copies 'config.geojson' and 'config.json' files from the source to the destination directories.
 
         Args:
@@ -944,15 +969,15 @@
         use_GPU: str,
         use_otsu: bool,
         use_tta: bool,
     ):
 
         logger.info(f"ROI directory: {src_directory}")
         logger.info(f"session name: {session_name}")
-
+        print(f"Running model {model_id}")
         self.prepare_model(model_implementation, model_id)
         classes = self.get_classes(self.weights_directory)
         model_dict = {
             "sample_direc": None,
             "use_GPU": use_GPU,
             "implementation": model_implementation,
             "model_type": model_id,
@@ -965,14 +990,18 @@
         session = sessions.Session()
         sessions_path = common.create_directory(os.getcwd(), "sessions")
         session_path = common.create_directory(sessions_path, session_name)
 
         session.classes = classes
         session.path = session_path
         session.name = session_name
-
+        print(f"Preprocessing the data at {src_directory}")
         preprocessed_data = self.preprocess_data(src_directory, model_dict, session)
+        if preprocessed_data == {}:
+            logger.error(f"No data to process at {src_directory}")
+            raise Exception(f"No data to process at {src_directory}")
 
         self.compute_segmentation(preprocessed_data)
         self.postprocess_data(preprocessed_data, session)
         # save session data after postprocessing data
         session.save(session_path)
+        print(f"Session saved at {session_path}")
```

### Comparing `seg2map-0.0.7/src/seg2map.egg-info/PKG-INFO` & `seg2map-0.0.8/src/seg2map.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seg2map
-Version: 0.0.7
+Version: 0.0.8
 Summary: An interactive jupyter notebook for downloading satellite imagery
 Author-email:  Sharon Fitzpatrick <sharon.fitzpatrick23@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Doodleverse
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `seg2map-0.0.7/src/seg2map.egg-info/SOURCES.txt` & `seg2map-0.0.8/src/seg2map.egg-info/SOURCES.txt`

 * *Files identical despite different names*

