# Comparing `tmp/volume_segmantics_vsui-0.2.8.tar.gz` & `tmp/volume_segmantics_vsui-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volume_segmantics_vsui-0.2.8.tar", max compression
+gzip compressed data, was "volume_segmantics_vsui-0.3.3.tar", max compression
```

## Comparing `volume_segmantics_vsui-0.2.8.tar` & `volume_segmantics_vsui-0.3.3.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0    11357 2022-11-04 15:16:25.432262 volume_segmantics_vsui-0.2.8/LICENSE.md
--rw-r--r--   0        0        0     7738 2022-11-23 12:03:19.047796 volume_segmantics_vsui-0.2.8/README.md
--rw-r--r--   0        0        0     1754 2022-12-09 09:21:41.959285 volume_segmantics_vsui-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       33 2022-11-04 15:16:32.280162 volume_segmantics_vsui-0.2.8/volume_segmantics/__init__.py
--rw-r--r--   0        0        0      184 2022-11-18 10:09:08.613020 volume_segmantics_vsui-0.2.8/volume_segmantics/data/__init__.py
--rw-r--r--   0        0        0     3219 2022-11-04 15:16:32.287172 volume_segmantics_vsui-0.2.8/volume_segmantics/data/augmentations.py
--rw-r--r--   0        0        0     1611 2022-11-04 15:16:32.291149 volume_segmantics_vsui-0.2.8/volume_segmantics/data/base_data_manager.py
--rw-r--r--   0        0        0     2564 2022-11-04 15:16:32.292171 volume_segmantics_vsui-0.2.8/volume_segmantics/data/dataloaders.py
--rw-r--r--   0        0        0     5532 2022-11-23 12:03:19.199794 volume_segmantics_vsui-0.2.8/volume_segmantics/data/datasets.py
--rw-r--r--   0        0        0    13578 2022-11-04 15:16:32.297162 volume_segmantics_vsui-0.2.8/volume_segmantics/data/pytorch3dunet_losses.py
--rw-r--r--   0        0        0     5315 2022-11-04 15:16:32.300156 volume_segmantics_vsui-0.2.8/volume_segmantics/data/pytorch3dunet_metrics.py
--rw-r--r--   0        0        0      883 2022-12-08 13:45:36.205093 volume_segmantics_vsui-0.2.8/volume_segmantics/data/settings_data.py
--rw-r--r--   0        0        0     5947 2022-11-23 12:03:19.206766 volume_segmantics_vsui-0.2.8/volume_segmantics/data/slicers.py
--rw-r--r--   0        0        0      251 2022-11-04 15:16:32.309155 volume_segmantics_vsui-0.2.8/volume_segmantics/model/__init__.py
--rw-r--r--   0        0        0     2376 2022-11-04 15:16:32.311165 volume_segmantics_vsui-0.2.8/volume_segmantics/model/model_2d.py
--rw-r--r--   0        0        0     6610 2022-11-17 16:56:39.453422 volume_segmantics_vsui-0.2.8/volume_segmantics/model/operations/vol_seg_2d_predictor.py
--rw-r--r--   0        0        0    24933 2022-11-21 13:22:21.257363 volume_segmantics_vsui-0.2.8/volume_segmantics/model/operations/vol_seg_2d_trainer.py
--rw-r--r--   0        0        0     4128 2022-11-23 12:03:19.224787 volume_segmantics_vsui-0.2.8/volume_segmantics/model/operations/vol_seg_prediction_manager.py
--rw-r--r--   0        0        0     2199 2022-11-21 14:02:30.325204 volume_segmantics_vsui-0.2.8/volume_segmantics/scripts/predict_2d_model.py
--rw-r--r--   0        0        0     3913 2022-11-18 10:02:55.594149 volume_segmantics_vsui-0.2.8/volume_segmantics/scripts/predict_2d_model_oo.py
--rw-r--r--   0        0        0     3865 2022-11-21 14:00:22.313329 volume_segmantics_vsui-0.2.8/volume_segmantics/scripts/train_2d_model.py
--rw-r--r--   0        0        0     5747 2022-11-18 10:02:38.742085 volume_segmantics_vsui-0.2.8/volume_segmantics/scripts/train_2d_model_oo.py
--rw-r--r--   0        0        0   570399 2022-11-04 15:16:32.361156 volume_segmantics_vsui-0.2.8/volume_segmantics/scripts/volume_segmantics
--rw-r--r--   0        0        0      280 2022-11-18 17:03:13.211286 volume_segmantics_vsui-0.2.8/volume_segmantics/utilities/__init__.py
--rw-r--r--   0        0        0     4893 2022-11-09 09:39:13.730919 volume_segmantics_vsui-0.2.8/volume_segmantics/utilities/arg_parsing.py
--rw-r--r--   0        0        0    11219 2022-11-23 12:03:19.236788 volume_segmantics_vsui-0.2.8/volume_segmantics/utilities/base_data_utils.py
--rw-r--r--   0        0        0     1197 2022-11-18 09:23:23.040192 volume_segmantics_vsui-0.2.8/volume_segmantics/utilities/cmdline.py
--rw-r--r--   0        0        0     1843 2022-11-04 15:16:32.377153 volume_segmantics_vsui-0.2.8/volume_segmantics/utilities/config.py
--rw-r--r--   0        0        0     2537 2022-11-04 15:16:32.379154 volume_segmantics_vsui-0.2.8/volume_segmantics/utilities/early_stopping.py
--rw-r--r--   0        0        0     1903 2022-11-04 15:16:32.381151 volume_segmantics_vsui-0.2.8/volume_segmantics/utilities/pytorch3dunet_utils.py
--rw-r--r--   0        0        0     9260 1970-01-01 00:00:00.000000 volume_segmantics_vsui-0.2.8/setup.py
--rw-r--r--   0        0        0     9090 1970-01-01 00:00:00.000000 volume_segmantics_vsui-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-11 12:00:14.923609 volume_segmantics_vsui-0.3.3/LICENSE.md
+-rw-r--r--   0        0        0     7861 2023-04-13 08:54:44.656609 volume_segmantics_vsui-0.3.3/README.md
+-rw-r--r--   0        0        0     1827 2023-04-18 10:52:38.326202 volume_segmantics_vsui-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-04-11 12:00:20.688662 volume_segmantics_vsui-0.3.3/volume_segmantics/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-11 12:00:20.691680 volume_segmantics_vsui-0.3.3/volume_segmantics/data/__init__.py
+-rw-r--r--   0        0        0     3219 2023-04-11 12:00:20.693685 volume_segmantics_vsui-0.3.3/volume_segmantics/data/augmentations.py
+-rw-r--r--   0        0        0     1611 2023-04-11 12:00:20.696663 volume_segmantics_vsui-0.3.3/volume_segmantics/data/base_data_manager.py
+-rw-r--r--   0        0        0     2564 2023-04-11 12:00:20.699676 volume_segmantics_vsui-0.3.3/volume_segmantics/data/dataloaders.py
+-rw-r--r--   0        0        0     5532 2023-04-11 12:00:20.702694 volume_segmantics_vsui-0.3.3/volume_segmantics/data/datasets.py
+-rw-r--r--   0        0        0    13578 2023-04-11 12:00:20.706691 volume_segmantics_vsui-0.3.3/volume_segmantics/data/pytorch3dunet_losses.py
+-rw-r--r--   0        0        0     5315 2023-04-11 12:00:20.709679 volume_segmantics_vsui-0.3.3/volume_segmantics/data/pytorch3dunet_metrics.py
+-rw-r--r--   0        0        0      947 2023-04-17 10:14:00.079580 volume_segmantics_vsui-0.3.3/volume_segmantics/data/settings_data.py
+-rw-r--r--   0        0        0     5947 2023-04-11 12:00:20.714678 volume_segmantics_vsui-0.3.3/volume_segmantics/data/slicers.py
+-rw-r--r--   0        0        0      251 2023-04-11 12:00:20.720659 volume_segmantics_vsui-0.3.3/volume_segmantics/model/__init__.py
+-rw-r--r--   0        0        0     2464 2023-04-13 08:54:44.689601 volume_segmantics_vsui-0.3.3/volume_segmantics/model/model_2d.py
+-rw-r--r--   0        0        0     6626 2023-04-17 08:56:54.644642 volume_segmantics_vsui-0.3.3/volume_segmantics/model/operations/vol_seg_2d_predictor.py
+-rw-r--r--   0        0        0    24903 2023-04-17 10:14:20.555320 volume_segmantics_vsui-0.3.3/volume_segmantics/model/operations/vol_seg_2d_trainer.py
+-rw-r--r--   0        0        0     4128 2023-04-11 12:00:20.731684 volume_segmantics_vsui-0.3.3/volume_segmantics/model/operations/vol_seg_prediction_manager.py
+-rw-r--r--   0        0        0     2161 2023-04-17 09:38:50.301696 volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/predict_2d_model.py
+-rw-r--r--   0        0        0     3764 2023-04-13 14:00:02.078267 volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/predict_2d_model_oo.py
+-rw-r--r--   0        0        0     4364 2023-04-18 10:08:58.833356 volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/train_2d_model.py
+-rw-r--r--   0        0        0     5737 2023-04-17 10:15:51.296357 volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/train_2d_model_oo.py
+-rw-r--r--   0        0        0   570399 2023-04-13 08:23:05.091847 volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/volume_segmantics
+-rw-r--r--   0        0        0      280 2023-04-13 08:23:05.093867 volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/__init__.py
+-rw-r--r--   0        0        0     5382 2023-04-18 10:07:47.981474 volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/arg_parsing.py
+-rw-r--r--   0        0        0    11367 2023-04-17 10:15:27.528305 volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/base_data_utils.py
+-rw-r--r--   0        0        0     1197 2023-04-13 08:23:05.101850 volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/cmdline.py
+-rw-r--r--   0        0        0     1843 2023-04-13 08:23:05.103851 volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/config.py
+-rw-r--r--   0        0        0     2537 2023-04-11 12:00:20.774685 volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/early_stopping.py
+-rw-r--r--   0        0        0     1903 2023-04-11 12:00:20.777682 volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/pytorch3dunet_utils.py
+-rw-r--r--   0        0        0     9232 1970-01-01 00:00:00.000000 volume_segmantics_vsui-0.3.3/PKG-INFO
```

### Comparing `volume_segmantics_vsui-0.2.8/LICENSE.md` & `volume_segmantics_vsui-0.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.2.8/README.md` & `volume_segmantics_vsui-0.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 The easiest way to install the package is to first create a new conda environment or virtualenv with python (ideally >= version 3.8) and also pip, then activate the environment and `pip install volume-segmantics`. If a CUDA-enabled build of PyTorch is not being installed by pip, you can try `pip install volume-segmantics --extra-index-url https://download.pytorch.org/whl` this particularity seems to be an issue on Windows. 
 
 ## Configuration and command line use
 
 After installation, two new commands will be available from your terminal whilst your environment is activated, `model-train-2d` and `model-predict-2d`.
 
-These commands require access to some settings stored in YAML files. These need to be located in a directory named `volseg-settings` within the directory where you are running the commands. The settings files can be copied from [here](https://github.com/DiamondLightSource/volume-segmantics/releases/download/v0.2.8/volseg-settings.zip). 
+These commands require access to some settings stored in YAML files. These need to be located in a directory named `volseg-settings` within the directory where you are running the commands. The settings files can be copied from [here](https://github.com/DiamondLightSource/volume-segmantics/releases/download/v0.3.1/volseg-settings.zip). 
 
 The file `2d_model_train_settings.yaml` can be edited in order to change training parameters such as number of epochs, loss functions, evaluation metrics and also model and encoder architectures. The file `2d_model_predict_settings.yaml` can be edited to change parameters such as the prediction "quality" e.g "low" quality refers to prediction of the volume segmentation by taking images along a single axis (images in the (x,y) plane). For "medium" and "high" quality, predictions are done along 3 axes and in 12 directions (3 axes, 4 rotations) respectively, before being combined by maximum probability. 
 
 ### For training a 2d model on a 3d image volume and corresponding labels
 Run the following command. Input files can be in HDF5 or multi-page TIFF format.
 
 ```shell
@@ -53,20 +53,27 @@
 The model architectures which are currently available and tested are: 
 - U-Net
 - U-Net++
 - FPN
 - DeepLabV3
 - DeepLabV3+
 - MA-Net
-- LinkNet.
+- LinkNet
+- PAN
 
 The pre-trained encoders that can be used with these architectures are: 
 - ResNet-34
 - ResNet50
-- ResNeXt-50_32x4d.
+- ResNeXt-50_32x4d
+- Efficientnet-b3
+- Efficientnet-b4
+- Resnest50d\*
+- Resnest101e\*
+
+\* Encoders with asterisk not compatible with PAN.
 
 ## Using the API
 
 You can use the functionality of the package in your own program via the API, this is [documented here](https://diamondlightsource.github.io/volume-segmantics/). This interface is the one used by [SuRVoS2](https://github.com/DiamondLightSource/SuRVoS2), a client/server GUI application that allows fast annotation and segmentation of volumetric data. 
 
 ## Contributing
```

### Comparing `volume_segmantics_vsui-0.2.8/pyproject.toml` & `volume_segmantics_vsui-0.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [tool.poetry]
 name = "volume-segmantics-vsui"
-version = "0.2.8"
+version = "0.3.3"
 description = "A toolkit for semantic segmentation of volumetric data using pyTorch deep learning models"
 authors = ["Oliver King <olly.king@diamond.ac.uk>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "volume_segmantics"}]
 repository = "https://github.com/DiamondLightSource/volume-segmantics"
 keywords = ["segmentation", "deep-learning", "volumetric", "3d"]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Image Processing",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-albumentations = "<=1.1.0"
+albumentations = "^1.1.0"
 h5py = "^3.0.0"
 numpy = "^1.18.0"
 matplotlib = "^3.3.0"
-torch = ">=1.7.1, <1.13.0"
+torch = "^1.7.1"
 segmentation-models-pytorch = "^0.2.1"
 termplotlib = "^0.3.6"
 imagecodecs = "*"
-vsui-client = "^0.2.0"#{path = "/dls/science/users/jig77871/projects/vsui-client"}#
+vsui-client = "^1.1.9"
+#vsui-client = {path = "/dls/science/groups/imaging/Matthew/volume-segmantics/vsui-client/dist/vsui_client-1.1.9-py3-none-any.whl"}
 
 [tool.poetry.dev-dependencies]
 black = ">=22.1.0"
 pdoc = ">=10"
 pylint = ">=2.4.0"
 pytest = ">=6"
 pytest-cov = "*"
```

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/data/augmentations.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/data/augmentations.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/data/base_data_manager.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/data/base_data_manager.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/data/dataloaders.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/data/dataloaders.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/data/datasets.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/data/datasets.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/data/pytorch3dunet_losses.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/data/pytorch3dunet_losses.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/data/pytorch3dunet_metrics.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/data/pytorch3dunet_metrics.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/data/settings_data.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/data/settings_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,10 +18,10 @@
         logging.info(f"Loading settings from {data}!")
         if data.exists():
             with open(data, "r") as stream:
                 settings_dict = yaml.safe_load(stream)
             return SimpleNamespace(**settings_dict)
         else:
             logging.error("Couldn't find settings file... Exiting!")
-            sys.exit(1)
+            raise FileNotFoundError(f"Couldn't find settings file at {data}! Exiting!")
     elif isinstance(data, dict):
         return SimpleNamespace(**data)
```

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/data/slicers.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/data/slicers.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/model/model_2d.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/model/model_2d.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,16 @@
         model = smp.DeepLabV3Plus(**struct_dict_copy)
         logging.info(f"Sending the DeepLabV3+ model to device {device_num}")
     elif model_type == utils.ModelType.MA_NET:
         model = smp.MAnet(**struct_dict_copy)
         logging.info(f"Sending the MA-Net model to device {device_num}")
     elif model_type == utils.ModelType.LINKNET:
         model = smp.Linknet(**struct_dict_copy)
+    elif model_type == utils.ModelType.PAN:
+        model = smp.PAN(**struct_dict_copy)
         logging.info(f"Sending the Linknet model to device {device_num}")
     return model.to(device_num)
 
 
 def create_model_from_file(
     weights_fn: Path, gpu: bool = True, device_num: int = 0,
 ) -> Tuple[torch.nn.Module, int, dict]:
```

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/model/operations/vol_seg_2d_predictor.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/model/operations/vol_seg_2d_predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 import volume_segmantics.utilities.base_data_utils as utils
 import volume_segmantics.utilities.config as cfg
 from torch import nn as nn
 from tqdm import tqdm
 from volume_segmantics.data.dataloaders import get_2d_prediction_dataloader
 from volume_segmantics.model.model_2d import create_model_from_file
 from volume_segmantics.utilities.base_data_utils import Axis
-import vsui_client.vsui_client as vsui_client
+import vsui_client
 
 
 class VolSeg2dPredictor:
     """Class that performs U-Net prediction operations. Does not interact with disk."""
 
     def __init__(self, model_file_path: str, settings: SimpleNamespace) -> None:
+        self.VSUI = vsui_client.get_client()
         self.model_file_path = Path(model_file_path)
         self.settings = settings
         self.model_device_num = int(settings.cuda_device)
         model_tuple = create_model_from_file(
             self.model_file_path, self.model_device_num
         )
         self.model, self.num_labels, self.label_codes = model_tuple
@@ -53,15 +54,15 @@
                     max_prob_idx = torch.argmax(probs, dim=1, keepdim=True)
                     # Extract along axis from outputs
                     probs = torch.gather(probs, 1, max_prob_idx)
                     # Remove the label dimension
                     probs = torch.squeeze(probs, dim=1)
                     probs = utils.crop_tensor_to_array(probs, yx_dims)
                     output_prob_list.append(probs.astype(np.float16))
-                vsui_client.edit_element('Prediction Batch', {"current":i+1, "max": len(data_loader.dataset)/data_loader.batch_size})
+                self.VSUI.edit_element('Prediction Batch', {"current":i+1, "max": len(data_loader.dataset)/data_loader.batch_size})
 
         labels = np.concatenate(output_vol_list)
         labels = utils.rotate_array_to_axis(labels, axis)
         probs = np.concatenate(output_prob_list) if output_prob_list else None
         if probs is not None:
             probs = utils.rotate_array_to_axis(probs, axis)
         return labels, probs
```

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/model/operations/vol_seg_2d_trainer.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/model/operations/vol_seg_2d_trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import csv
 import logging
 import math
 from pathlib import Path
 import sys
-# base64 encoding image
-import io
-import base64
 # -------
 import time
 from types import SimpleNamespace
 from typing import Union
 
 import matplotlib as mpl
 import numpy as np
@@ -31,22 +28,22 @@
 from volume_segmantics.data.pytorch3dunet_metrics import (
     DiceCoefficient,
     MeanIoU,
 )
 from volume_segmantics.model.model_2d import create_model_on_device
 from volume_segmantics.utilities.early_stopping import EarlyStopping
 
-import vsui_client.vsui_client as vsui_client
+import vsui_client
+
 
 class VolSeg2dTrainer:
     """Class that provides methods to train a 2d deep learning model
     and to output figures showing training and validation loss and
     example predictions on random validation images.
     """
-
     def __init__(
         self,
         image_dir_path: Path,
         label_dir_path: Path,
         labels: Union[int, dict],
         settings: SimpleNamespace,
     ):
@@ -54,14 +51,15 @@
 
         Args:
             image_dir_path (Path): Path to directory containing image data slices.
             label_dir_path (Path): Path to directory containing label data slices.
             labels (Union[int, dict]): Either number of labels or dictionary containing label names and associated metadata.
             settings (SimpleNamespace): A training settings object.
         """
+        self.VSUI = vsui_client.get_client()
         self.training_loader, self.validation_loader = get_2d_training_dataloaders(
             image_dir_path, label_dir_path, settings
         )
         self.label_no = labels if isinstance(labels, int) else len(labels)
         self.codes = labels if isinstance(labels, dict) else {}
         self.settings = settings
         # Params for learning rate finder
@@ -145,28 +143,28 @@
             logging.info("Using CrossEntropyLoss")
             loss_criterion = nn.CrossEntropyLoss()
         elif self.settings.loss_criterion == "GeneralizedDiceLoss":
             logging.info("Using GeneralizedDiceLoss")
             loss_criterion = GeneralizedDiceLoss()
         else:
             logging.error("No loss criterion specified, exiting")
-            sys.exit(1)
+            raise ValueError("No loss criterion specified")
         return loss_criterion
 
     def _get_eval_metric(self):
         # Get evaluation metric
         if self.settings.eval_metric == "MeanIoU":
             logging.info("Using MeanIoU")
             eval_metric = MeanIoU()
         elif self.settings.eval_metric == "DiceCoefficient":
             logging.info("Using DiceCoefficient")
             eval_metric = DiceCoefficient()
         else:
             logging.error("No evaluation metric specified, exiting")
-            sys.exit(1)
+            raise ValueError("No evaluation metric specified")
         return eval_metric
 
     def train_model(
         self,
         output_path: Path,
         num_epochs: int,
         patience: int,
@@ -208,27 +206,28 @@
                 output_path, patience, best_score=-min_loss
             )
 
         # Initialise the One Cycle learning rate scheduler
         lr_scheduler = self._create_oc_lr_scheduler(num_epochs, lr_to_use)
 
         for epoch in range(1, num_epochs + 1):
-            vsui_client.edit_element('Epoch', {"current": epoch, "max": num_epochs})
+            self.VSUI.edit_element('Epoch', {"current": epoch, "max": num_epochs})
             self.model.train()
             tic = time.perf_counter()
             logging.info(f"Epoch {epoch} of {num_epochs}")
             for i, batch in enumerate(tqdm(
                 self.training_loader,
                 desc="Training batch",
                 bar_format=cfg.TQDM_BAR_FORMAT,
             )):
-                vsui_client.edit_element('Batch Progress', {"current": i+1, "max": len(self.training_loader.dataset)/self.training_loader.batch_size})
+                self.VSUI.edit_element('Batch Progress', {"current": i+1, "max": len(self.training_loader.dataset)/self.training_loader.batch_size})
                 loss = self._train_one_batch(lr_scheduler, batch)
                 train_losses.append(loss.item())  # record training loss
 
+            # VALIDATION
             self.model.eval()  # prep model for evaluation
             with torch.no_grad():
                 for i, batch in enumerate(tqdm(
                     self.validation_loader,
                     desc="Validation batch",
                     bar_format=cfg.TQDM_BAR_FORMAT,
                 )):  
@@ -246,26 +245,26 @@
                     probs = s_max(output)  # Convert the logits to probs
                     probs = torch.unsqueeze(probs, 2)
                     targets = torch.unsqueeze(targets, 2)
                     eval_score = self.eval_metric(probs, targets)
                     if eval_score.is_cuda:
                         eval_score = eval_score.cpu().detach().numpy()
                     eval_scores.append(eval_score)  # record eval metric
-                    vsui_client.edit_element('Batch Progress', {"current": i+1, "max": len(self.validation_loader.dataset)/self.validation_loader.batch_size})
+                    self.VSUI.edit_element('Batch Progress', {"current": i+1, "max": len(self.validation_loader.dataset)/self.validation_loader.batch_size})
 
             toc = time.perf_counter()
             # calculate average loss/metric over an epoch
             self.avg_train_losses.append(np.average(train_losses))
             self.avg_valid_losses.append(np.average(valid_losses))
             self.avg_eval_scores.append(np.average(eval_scores))
             logging.info(
                 f"Epoch {epoch}. Training loss: {self.avg_train_losses[-1]}, Validation Loss: "
                 f"{self.avg_valid_losses[-1]}. {self.settings.eval_metric}: {self.avg_eval_scores[-1]}"
             )
-            vsui_client.edit_element('Training Loss', {"x": list(range(len(self.avg_train_losses))), "y": self.avg_train_losses})
+            self.VSUI.edit_element('Training Loss', {"x": list(range(len(self.avg_train_losses))), "y": self.avg_train_losses})
             logging.info(f"Time taken for epoch {epoch}: {toc - tic:0.2f} seconds")
             if frozen:
                 plot_title = f"Epoch {epoch} frozen."
             else:
                 plot_title = f"Epoch {epoch} unfrozen."
             self.output_running_prediction_figure(plot_title)
             # clear lists to track next epoch
@@ -276,15 +275,15 @@
             # early_stopping needs the validation loss to check if it has decreased,
             # and if it has, it will make a checkpoint of the current model
             early_stopping(
                 self.avg_valid_losses[-1], self.model, self.optimizer, self.codes
             )
 
             if early_stopping.early_stop:
-                vsui_client.notify('Training Stopping Early', 'info')
+                self.VSUI.notify('Training Stopping Early', 'info')
                 logging.info("Early stopping")
                 break
 
         # load the last checkpoint with the best model
         self._load_in_weights(output_path)
 
     def _load_in_model_and_optimizer(
@@ -324,21 +323,21 @@
 
         self.model.train()
         logging.info(
             f"Training for {self.lr_find_epochs} epochs to create a learning "
             "rate plot."
         )
         for i in range(self.lr_find_epochs):
-            vsui_client.edit_element('Epoch', {"current": i+1, "max": len(list(range(self.lr_find_epochs)))})
+            self.VSUI.edit_element('Epoch', {"current": i+1, "max": len(list(range(self.lr_find_epochs)))})
             for z, batch in enumerate(tqdm(
                 self.training_loader,
                 desc=f"Epoch {i + 1}, batch number",
                 bar_format=cfg.TQDM_BAR_FORMAT,
             )):  
-                vsui_client.edit_element('Batch Progress', {"current": z+1, "max": len(self.training_loader.dataset) / self.training_loader.batch_size})
+                self.VSUI.edit_element('Batch Progress', {"current": z+1, "max": len(self.training_loader.dataset) / self.training_loader.batch_size})
                 loss = self._train_one_batch(lr_scheduler, batch)
                 lr_step = self.optimizer.state_dict()["param_groups"][0]["lr"]
                 lr_find_lr.append(lr_step)
                 if iters == 0:
                     lr_find_loss.append(loss)
                 else:
                     loss = smoothing * loss + (1 - smoothing) * lr_find_loss[-1]
@@ -559,23 +558,22 @@
             )
             output = self.model(inputs)  # Forward pass
             s_max = nn.Softmax(dim=1)
             probs = s_max(output)  # Convert the logits to probs
             labels = torch.argmax(probs, dim=1)  # flatten channels
         
         for i in range(0,2):
-            my_base64_jpgData = vsui_client.encode_image(labels[i].cpu(), title=title)
-            vsui_client.edit_element('Sample Images', {'data': {'slice': i, 'img': my_base64_jpgData}})
+            my_base64_jpgData = self.VSUI.encode_image(labels[i].cpu(), title=title)
+            self.VSUI.edit_element('Sample Images', {'data': {'slice': i, 'img': my_base64_jpgData}})
 
     def output_comparison_figures(self) -> None:
-        print('---------- outputting comparison figures ---------------')
         batch = next(iter(self.validation_loader))  # Get first batch
         with torch.no_grad():
             inputs, targets = utils.prepare_training_batch(
                 batch, self.model_device_num, self.label_no
             )
         for i in range(0,2):
-            my_base64_jpgData = vsui_client.encode_image(inputs[i].squeeze().cpu(), title="Data")
-            vsui_client.edit_element('Sample Images', {'reference': {'slice': i, 'img': my_base64_jpgData}})
+            my_base64_jpgData = self.VSUI.encode_image(inputs[i].squeeze().cpu(), title="Data")
+            self.VSUI.edit_element('Sample Images', {'reference': {'slice': i, 'img': my_base64_jpgData}})
 
-            my_base64_jpgData = vsui_client.encode_image(torch.argmax(targets[i], dim=0).cpu(), title="Ground Truth")
-            vsui_client.edit_element('Sample Images', {'reference': {'slice': i, 'img': my_base64_jpgData}})
+            my_base64_jpgData = self.VSUI.encode_image(torch.argmax(targets[i], dim=0).cpu(), title="Ground Truth")
+            self.VSUI.edit_element('Sample Images', {'reference': {'slice': i, 'img': my_base64_jpgData}})
```

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/model/operations/vol_seg_prediction_manager.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/model/operations/vol_seg_prediction_manager.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/scripts/predict_2d_model.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/predict_2d_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,39 +5,40 @@
 from datetime import date
 from pathlib import Path
 
 import volume_segmantics.utilities.config as cfg
 from volume_segmantics.data import get_settings_data
 from volume_segmantics.model import VolSeg2DPredictionManager
 from volume_segmantics.utilities import get_2d_prediction_parser
-import vsui_client.vsui_client as vsui_client
+from vsui_client import vsui_process, init_vsui
 
 warnings.filterwarnings("ignore", category=UserWarning)
 
 def create_output_path(root_path, data_vol_path):
     pred_out_fn = f"{date.today()}_{data_vol_path.stem}_2d_model_vol_pred.h5"
     return Path(root_path, pred_out_fn)
 
-@vsui_client.vsui_process()
+@vsui_process()
 def main():
     logger = logging.getLogger()
-    handler = vsui_client.RequestHandler()
     logging.basicConfig(
         level=logging.INFO, format=cfg.LOGGING_FMT, datefmt=cfg.LOGGING_DATE_FMT
     )
-    logger.addHandler(handler)
     # Parse Args
     parser = get_2d_prediction_parser()
     args = parser.parse_args()
 
     vsui_id = getattr(args, cfg.VSUI_PROCESS_ID_ARG)
     if vsui_id != "vsui_disabled":
-        vsui_client.set_task_id(vsui_id)
-        vsui_client.set_logging_target('Logs')
-        vsui_client.connect()
+        VSUI = init_vsui(True, vsui_id, 'Logs')
+        VSUI.connect()
+        handler = VSUI.get_handler()
+        logger.addHandler(handler)
+    else:
+        VSUI = init_vsui(False)
 
     # Define paths
     root_path = Path(getattr(args, cfg.DATA_DIR_ARG)).resolve()
     print(f'rootpath: {root_path}')
     settings_path = Path(root_path, cfg.SETTINGS_DIR, cfg.PREDICTION_SETTINGS_FN)
 
     model_file_path = getattr(args, cfg.MODEL_PTH_ARG)
@@ -52,14 +53,14 @@
     print(f'output_path: {output_path}')
 
     # Get settings object
     settings = get_settings_data(settings_path)
     # Create prediction manager and predict
     pred_manager = VolSeg2DPredictionManager(model_file_path, data_vol_path, settings)
     pred_manager.predict_volume_to_path(output_path)
-    vsui_client.notify('prediction completed', 'success')
-    vsui_client.deactivate_task()
-    vsui_client.disconnect()
+    VSUI.notify('prediction completed', 'success')
+    VSUI.deactivate_task()
+    VSUI.disconnect()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/scripts/predict_2d_model_oo.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/predict_2d_model_oo.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 import atexit
 
 import utilities.config as cfg
 from data import get_settings_data
 from model import VolSeg2DPredictionManager
 from utilities import CheckExt
-import vsui_client.vsui_client as vsui_client
+from vsui_client import vsui_process, init_vsui
 
 warnings.filterwarnings("ignore", category=UserWarning)
 
 def init_argparse() -> argparse.ArgumentParser:
     """Custom argument parser for this program.
 
     Returns:
@@ -50,37 +50,33 @@
     )
     return parser
 
 def create_output_path(root_path, data_vol_path):
     pred_out_fn = f"{date.today()}_{data_vol_path.stem}_2d_model_vol_pred.h5"
     return Path(root_path, pred_out_fn)
 
+@vsui_process
 def main():
-    # Disconnect when the process is closed
-    def exit_handler():
-        vsui_client.disconnect()
-
-    atexit.register(exit_handler)
-
     # Logging
     logger = logging.getLogger()
-    handler = vsui_client.RequestHandler()
     logging.basicConfig(
         level=logging.INFO, format=cfg.LOGGING_FMT, datefmt=cfg.LOGGING_DATE_FMT
     )
-    logger.addHandler(handler)
     # Parse Args
     parser = init_argparse()
     args = parser.parse_args()
 
     vsui_id = getattr(args, cfg.VSUI_PROCESS_ID_ARG)
     if vsui_id != "vsui_disabled":
-        vsui_client.set_task_id(vsui_id)
-        vsui_client.set_logging_target('Logs')
-        vsui_client.connect()
+        VSUI = init_vsui(True, vsui_id, 'Logs')
+        VSUI.connect()
+        handler = VSUI.get_handler()
+        logger.addHandler(handler)
+    else:
+        VSUI = init_vsui(False)
 
     # Define paths
     root_path = Path(getattr(args, cfg.DATA_DIR_ARG)).resolve()
     print(f'rootpath: {root_path}')
     settings_path = Path(root_path, cfg.SETTINGS_DIR, cfg.PREDICTION_SETTINGS_FN)
 
     model_file_path = getattr(args, cfg.MODEL_PTH_ARG)
@@ -95,14 +91,14 @@
     print(f'output_path: {output_path}')
 
     # Get settings object
     settings = get_settings_data(settings_path)
     # Create prediction manager and predict
     pred_manager = VolSeg2DPredictionManager(model_file_path, data_vol_path, settings)
     pred_manager.predict_volume_to_path(output_path)
-    vsui_client.notify('prediction completed', 'success')
-    vsui_client.deactivate_task()
-    vsui_client.disconnect()
+    VSUI.notify('prediction completed', 'success')
+    VSUI.deactivate_task()
+    VSUI.disconnect()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/scripts/train_2d_model_oo.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/train_2d_model_oo.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 import atexit
 
 import utilities.config as cfg
 from data import (TrainingDataSlicer, get_settings_data)
 from model import VolSeg2dTrainer
 from utilities import CheckExt
-import vsui_client.vsui_client as vsui_client
+from vsui_client import vsui_process, init_vsui
 
 def init_argparse() -> argparse.ArgumentParser:
     """Custom argument parser for this program.
 
     Returns:
         argparse.ArgumentParser: An argument parser with the appropriate
         command line args contained within.
@@ -46,36 +46,34 @@
         type=str,
         nargs="?",
         default="vsui_disabled",
         help="unique task id for this process in gui"
     )
     return parser
 
+@vsui_process
 def main():
-    def exit_handler():
-        vsui_client.disconnect()
-
-    atexit.register(exit_handler)
-    
     logger = logging.getLogger()
-    handler = vsui_client.RequestHandler()
     logging.basicConfig(
         level=logging.INFO, format=cfg.LOGGING_FMT, datefmt=cfg.LOGGING_DATE_FMT
     )
     logger.addHandler(handler)
     # Parse args and check correct number of volumes given
     parser = init_argparse()
     args = parser.parse_args()
     data_vols = getattr(args, cfg.TRAIN_DATA_ARG)
     label_vols = getattr(args, cfg.LABEL_DATA_ARG)
     vsui_id = getattr(args, cfg.VSUI_PROCESS_ID_ARG)
     if vsui_id != "vsui_disabled":
-        vsui_client.set_task_id(vsui_id)
-        vsui_client.set_logging_target('Logs')
-        vsui_client.connect()
+        VSUI = init_vsui(True, vsui_id, 'Logs')
+        VSUI.connect()
+        handler = VSUI.get_handler()
+        logger.addHandler(handler)
+    else:
+        VSUI = init_vsui(False)
 
     if isinstance(data_vols, str):
         data_vols = [Path(data_vols)]
     if isinstance(label_vols, str):
         label_vols = [Path(label_vols)]
 
     root_path = Path(getattr(args, cfg.DATA_DIR_ARG)).resolve()
@@ -85,15 +83,15 @@
     settings_path = Path(root_path, cfg.SETTINGS_DIR, cfg.TRAIN_SETTINGS_FN)
     settings = get_settings_data(settings_path)
 
     if len(data_vols) != len(label_vols):
         logging.error(
             "Number of data volumes and number of label volumes must be equal!"
         )
-        sys.exit(1)
+        raise ValueError(f"Number of data volumes and number of label volumes must be equal!")
 
     data_im_out_dir = root_path / settings.data_im_dirname  # dir for data imgs
     seg_im_out_dir = root_path / settings.seg_im_out_dirname  # dir for seg imgs
     # Keep track of the number of labels
     max_label_no = 0
     label_codes = None
     # Set up the DataSlicer and slice the data volumes into image files
@@ -111,15 +109,15 @@
     # Train the model, first frozen, then unfrozen
     num_cyc_frozen = settings.num_cyc_frozen
     num_cyc_unfrozen = settings.num_cyc_unfrozen
     model_type = settings.model["type"].name
     model_fn = f"{date.today()}_{model_type}_{settings.model_output_fn}.pytorch"
     model_out = Path(root_path, model_fn)
     trainer.output_comparison_figures()
-    vsui_client.notify('training started', 'info')
+    VSUI.notify('training started', 'info')
     if num_cyc_frozen > 0:
         trainer.train_model(
             model_out, num_cyc_frozen, settings.patience, create=True, frozen=True
         )
     if num_cyc_unfrozen > 0 and num_cyc_frozen > 0:
         trainer.train_model(
             model_out, num_cyc_unfrozen, settings.patience, create=False, frozen=False
@@ -128,14 +126,14 @@
         trainer.train_model(
             model_out, num_cyc_unfrozen, settings.patience, create=True, frozen=False
         )
     trainer.output_loss_fig(model_out)
     trainer.output_prediction_figure(model_out)
     # Clean up all the saved slices
     slicer.clean_up_slices()
-    vsui_client.notify('training completed', 'success')
-    vsui_client.deactivate_task()
-    vsui_client.disconnect()
+    VSUI.notify('training completed', 'success')
+    VSUI.deactivate_task()
+    VSUI.disconnect()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/scripts/volume_segmantics` & `volume_segmantics_vsui-0.3.3/volume_segmantics/scripts/volume_segmantics`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/utilities/arg_parsing.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/arg_parsing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import argparse
 from pathlib import Path
 
 import volume_segmantics.utilities.config as cfg
 
 
 def CheckExt(choices):
@@ -13,29 +14,36 @@
         https://stackoverflow.com/questions/15203829/python-argparse-file-extension-checking
         """
 
         def __call__(self, parser, namespace, fnames, option_string=None):
             # Modified to take in a list of filenames
             if isinstance(fnames, list):
                 for fname in fnames:
-                    self.check_path(parser, fname)
+                    self.check_path(parser, fname, namespace)
             else:
-                self.check_path(parser, fnames)
+                self.check_path(parser, fnames, namespace)
 
             # If all okay, set attribute
             setattr(namespace, self.dest, fnames)
 
-        def check_path(self, parser, fname):
+        def check_path(self, parser, fname, namespace):
+            if fname == 'none':
+                logging.error(f"Must provide data and label volumes")
+                setattr(namespace, 'error', f"Must provide data and label volumes")
+                return None
             fname = Path(fname)
+            print(fname)
             ext = fname.suffix
             if ext not in choices:
-                parser.error(f"Wrong filetype: file {fname} doesn't end with {choices}")
+                logging.error(f"Wrong filetype: file {fname} doesn't end with {choices}")
+                setattr(namespace, 'error', f"Wrong filetype: file {fname} doesn't end with {choices}")
                 # Check that file exists
             if not fname.is_file():
-                parser.error(f"The file {str(fname)} does not appear to exist.")
+                logging.error(f"The file {str(fname)} does not appear to exist.")
+                setattr(namespace, 'error', f"The file {str(fname)} does not appear to exist.")
 
     return Act
 
 
 def get_2d_training_parser() -> argparse.ArgumentParser:
     """Argument parser for scripts that train a 2d network on a 3d volume.
```

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/utilities/base_data_utils.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/base_data_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,27 +43,28 @@
     U_NET = 1
     U_NET_PLUS_PLUS = 2
     FPN = 3
     DEEPLABV3 = 4
     DEEPLABV3_PLUS = 5
     MA_NET = 6
     LINKNET = 7
+    PAN = 8
 
 
 def create_enum_from_setting(setting_str, enum):
     if isinstance(setting_str, Enum):
         return setting_str
     try:
         output_enum = enum[setting_str.upper()]
     except KeyError:
         options = [k.name for k in enum]
         logging.error(
             f"{enum.__name__}: {setting_str} is not valid. Options are {options}."
         )
-        sys.exit(1)
+        raise ValueError(f"{enum.__name__}: {setting_str} is not valid. Options are {options}.")
     return output_enum
 
 
 def get_prediction_quality(settings: SimpleNamespace) -> Enum:
     pred_quality = create_enum_from_setting(settings.quality, Quality)
     return pred_quality
 
@@ -200,15 +201,15 @@
             )
             try:
                 dataset = data_handle["entry/final_result_tomo/data"]
             except KeyError:
                 logging.error(
                     "NXS file: Could not find entry at entry/final_result_tomo/data, exiting!"
                 )
-                sys.exit(1)
+                raise KeyError(f"Could not find data at entry/final_result_tomo/data")
     else:
         dataset = data_handle[hdf5_path]
     input_data_chunking = dataset.chunks
     return dataset[()], input_data_chunking
 
 
 def get_numpy_from_path(
```

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/utilities/cmdline.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/cmdline.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/utilities/config.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/config.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/utilities/early_stopping.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/early_stopping.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.2.8/volume_segmantics/utilities/pytorch3dunet_utils.py` & `volume_segmantics_vsui-0.3.3/volume_segmantics/utilities/pytorch3dunet_utils.py`

 * *Files identical despite different names*

### Comparing `volume_segmantics_vsui-0.2.8/setup.py` & `volume_segmantics_vsui-0.3.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,146 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: volume-segmantics-vsui
+Version: 0.3.3
+Summary: A toolkit for semantic segmentation of volumetric data using pyTorch deep learning models
+Home-page: https://github.com/DiamondLightSource/volume-segmantics
+License: Apache-2.0
+Keywords: segmentation,deep-learning,volumetric,3d
+Author: Oliver King
+Author-email: olly.king@diamond.ac.uk
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Dist: albumentations (>=1.1.0,<2.0.0)
+Requires-Dist: h5py (>=3.0.0,<4.0.0)
+Requires-Dist: imagecodecs
+Requires-Dist: matplotlib (>=3.3.0,<4.0.0)
+Requires-Dist: numpy (>=1.18.0,<2.0.0)
+Requires-Dist: segmentation-models-pytorch (>=0.2.1,<0.3.0)
+Requires-Dist: termplotlib (>=0.3.6,<0.4.0)
+Requires-Dist: torch (>=1.7.1,<2.0.0)
+Requires-Dist: vsui-client (>=1.1.9,<2.0.0)
+Project-URL: Repository, https://github.com/DiamondLightSource/volume-segmantics
+Description-Content-Type: text/markdown
 
-packages = \
-['volume_segmantics',
- 'volume_segmantics.data',
- 'volume_segmantics.model',
- 'volume_segmantics.model.operations',
- 'volume_segmantics.scripts',
- 'volume_segmantics.utilities']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['albumentations<=1.1.0',
- 'h5py>=3.0.0,<4.0.0',
- 'imagecodecs',
- 'matplotlib>=3.3.0,<4.0.0',
- 'numpy>=1.18.0,<2.0.0',
- 'segmentation-models-pytorch>=0.2.1,<0.3.0',
- 'termplotlib>=0.3.6,<0.4.0',
- 'torch>=1.7.1,<1.13.0',
- 'vsui-client>=0.2.0,<0.3.0']
-
-entry_points = \
-{'console_scripts': ['model-predict-2d = '
-                     'volume_segmantics.scripts.predict_2d_model:main',
-                     'model-train-2d = '
-                     'volume_segmantics.scripts.train_2d_model:main']}
-
-setup_kwargs = {
-    'name': 'volume-segmantics-vsui',
-    'version': '0.2.8',
-    'description': 'A toolkit for semantic segmentation of volumetric data using pyTorch deep learning models',
-    'long_description': '# Volume Segmantics\n\nA toolkit for semantic segmentation of volumetric data using PyTorch deep learning models.\n\n[![DOI](https://joss.theoj.org/papers/10.21105/joss.04691/status.svg)](https://doi.org/10.21105/joss.04691) ![example workflow](https://github.com/DiamondLightSource/volume-segmantics/actions/workflows/tests.yml/badge.svg) ![example workflow](https://github.com/DiamondLightSource/volume-segmantics/actions/workflows/release.yml/badge.svg)\n\nVolume Segmantics provides a simple command-line interface and API that allows researchers to quickly train a variety of 2D PyTorch segmentation models (e.g.  U-Net, U-Net++, FPN, DeepLabV3+) on their 3D datasets. These models use pre-trained encoders, enabling fast training on small datasets. Subsequently, the library enables using these trained models to segment larger 3D datasets, automatically merging predictions made in orthogonal planes and rotations to reduce artifacts that may result from predicting 3D segmentation using a 2D network.  \n\nGiven a 3d image volume and corresponding dense labels (the segmentation), a 2d model is trained on image slices taken along the x, y, and z axes. The method is optimised for small training datasets, e.g a single dataset in between $128^3$ and $512^3$ pixels. To achieve this, all models use pre-trained encoders and image augmentations are used to expand the size of the training dataset.\n\nThis work utilises the abilities afforded by the excellent [segmentation-models-pytorch](https://github.com/qubvel/segmentation_models.pytorch) library in combination with augmentations made available via [Albumentations](https://albumentations.ai/). Also the metrics and loss functions used make use of the hard work done by Adrian Wolny in his [pytorch-3dunet](https://github.com/wolny/pytorch-3dunet) repository. \n\n## Requirements\n\nA machine capable of running CUDA enabled PyTorch version 1.7.1 or greater is required. This generally means a reasonably modern NVIDIA GPU. The exact requirements differ according to operating system. For example on Windows you will need Visual Studio Build Tools as well as CUDA Toolkit installed see [the CUDA docs](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html) for more details. \n\n## Installation\n\nThe easiest way to install the package is to first create a new conda environment or virtualenv with python (ideally >= version 3.8) and also pip, then activate the environment and `pip install volume-segmantics`. If a CUDA-enabled build of PyTorch is not being installed by pip, you can try `pip install volume-segmantics --extra-index-url https://download.pytorch.org/whl` this particularity seems to be an issue on Windows. \n\n## Configuration and command line use\n\nAfter installation, two new commands will be available from your terminal whilst your environment is activated, `model-train-2d` and `model-predict-2d`.\n\nThese commands require access to some settings stored in YAML files. These need to be located in a directory named `volseg-settings` within the directory where you are running the commands. The settings files can be copied from [here](https://github.com/DiamondLightSource/volume-segmantics/releases/download/v0.2.8/volseg-settings.zip). \n\nThe file `2d_model_train_settings.yaml` can be edited in order to change training parameters such as number of epochs, loss functions, evaluation metrics and also model and encoder architectures. The file `2d_model_predict_settings.yaml` can be edited to change parameters such as the prediction "quality" e.g "low" quality refers to prediction of the volume segmentation by taking images along a single axis (images in the (x,y) plane). For "medium" and "high" quality, predictions are done along 3 axes and in 12 directions (3 axes, 4 rotations) respectively, before being combined by maximum probability. \n\n### For training a 2d model on a 3d image volume and corresponding labels\nRun the following command. Input files can be in HDF5 or multi-page TIFF format.\n\n```shell\nmodel-train-2d --data path/to/image/data.h5 --labels path/to/corresponding/segmentation/labels.h5\n```\n\nPaths to multiple data and label volumes can be added after the `--data` and `--labels` flags respectively. A model will be trained according to the settings defined in `/volseg-settings/2d_model_train_settings.yaml` and saved to your working directory. In addition, a figure showing "ground truth" segmentation vs model segmentation for some images in the validation set will be saved. \n\n### For 3d volume segmentation prediction using a 2d model\nRun the following command. Input image files can be in HDF5 or multi-page TIFF format.\n\n```shell\nmodel-predict-2d path/to/model_file.pytorch path/to/data_for_prediction.h5\n```\n\nThe input data will be segmented using the input model following the settings specified in `volseg-settings/2d_model_predict_settings.yaml`. An HDF5 file containing the segmented volume will be saved to your working directory.\n\n### Tutorial using example data\n\nA tutorial is available [here](training_data/README.md) that provides a walk-through of how to segment blood vessels from synchrotron X-ray micro-CT data collected on a sample of human placental tissue.\n\n## Currently supported model architectures and encoders\n\nThe model architectures which are currently available and tested are: \n- U-Net\n- U-Net++\n- FPN\n- DeepLabV3\n- DeepLabV3+\n- MA-Net\n- LinkNet.\n\nThe pre-trained encoders that can be used with these architectures are: \n- ResNet-34\n- ResNet50\n- ResNeXt-50_32x4d.\n\n## Using the API\n\nYou can use the functionality of the package in your own program via the API, this is [documented here](https://diamondlightsource.github.io/volume-segmantics/). This interface is the one used by [SuRVoS2](https://github.com/DiamondLightSource/SuRVoS2), a client/server GUI application that allows fast annotation and segmentation of volumetric data. \n\n## Contributing\n\nWe welcome contributions from the community. Please take a look at out [contribution guidelines](https://github.com/DiamondLightSource/volume-segmantics/blob/main/CONTRIBUTING.md) for more information.\n\n## Citation\n\nIf you use this package for you research, please cite:\n\n[King O.N.F, Bellos, D. and Basham, M. (2022). Volume Segmantics: A Python Package for Semantic Segmentation of Volumetric Data Using Pre-trained PyTorch Deep Learning Models. Journal of Open Source Software, 7(78), 4691. doi: 10.21105/joss.04691](https://doi.org/10.21105/joss.04691)\n\n```bibtex\n@article{King2022,\n    doi = {10.21105/joss.04691},\n    url = {https://doi.org/10.21105/joss.04691},\n    year = {2022},\n    publisher = {The Open Journal},\n    volume = {7},\n    number = {78},\n    pages = {4691},\n    author = {Oliver N. F. King and Dimitrios Bellos and Mark Basham},\n    title = {Volume Segmantics: A Python Package for Semantic Segmentation of Volumetric Data Using Pre-trained PyTorch Deep Learning Models},\n    journal = {Journal of Open Source Software} }\n```\n\n## References\n\n**Albumentations**\n\nBuslaev, A., Iglovikov, V.I., Khvedchenya, E., Parinov, A., Druzhinin, M., and Kalinin, A.A. (2020). Albumentations: Fast and Flexible Image Augmentations. Information 11. [https://doi.org/10.3390/info11020125](https://doi.org/10.3390/info11020125)\n\n**Segmentation Models PyTorch**\n\nYakubovskiy, P. (2020). Segmentation Models Pytorch. [GitHub](https://github.com/qubvel/segmentation_models.pytorch)\n\n**PyTorch-3dUnet**\n\nWolny, A., Cerrone, L., Vijayan, A., Tofanelli, R., Barro, A.V., Louveaux, M., Wenzl, C., Strauss, S., Wilson-Sánchez, D., Lymbouridou, R., et al. (2020). Accurate and versatile 3D segmentation of plant tissues at cellular resolution. ELife 9, e57613. [https://doi.org/10.7554/eLife.57613](https://doi.org/10.7554/eLife.57613)\n',
-    'author': 'Oliver King',
-    'author_email': 'olly.king@diamond.ac.uk',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/DiamondLightSource/volume-segmantics',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+# Volume Segmantics
 
+A toolkit for semantic segmentation of volumetric data using PyTorch deep learning models.
+
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04691/status.svg)](https://doi.org/10.21105/joss.04691) ![example workflow](https://github.com/DiamondLightSource/volume-segmantics/actions/workflows/tests.yml/badge.svg) ![example workflow](https://github.com/DiamondLightSource/volume-segmantics/actions/workflows/release.yml/badge.svg)
+
+Volume Segmantics provides a simple command-line interface and API that allows researchers to quickly train a variety of 2D PyTorch segmentation models (e.g.  U-Net, U-Net++, FPN, DeepLabV3+) on their 3D datasets. These models use pre-trained encoders, enabling fast training on small datasets. Subsequently, the library enables using these trained models to segment larger 3D datasets, automatically merging predictions made in orthogonal planes and rotations to reduce artifacts that may result from predicting 3D segmentation using a 2D network.  
+
+Given a 3d image volume and corresponding dense labels (the segmentation), a 2d model is trained on image slices taken along the x, y, and z axes. The method is optimised for small training datasets, e.g a single dataset in between $128^3$ and $512^3$ pixels. To achieve this, all models use pre-trained encoders and image augmentations are used to expand the size of the training dataset.
+
+This work utilises the abilities afforded by the excellent [segmentation-models-pytorch](https://github.com/qubvel/segmentation_models.pytorch) library in combination with augmentations made available via [Albumentations](https://albumentations.ai/). Also the metrics and loss functions used make use of the hard work done by Adrian Wolny in his [pytorch-3dunet](https://github.com/wolny/pytorch-3dunet) repository. 
+
+## Requirements
+
+A machine capable of running CUDA enabled PyTorch version 1.7.1 or greater is required. This generally means a reasonably modern NVIDIA GPU. The exact requirements differ according to operating system. For example on Windows you will need Visual Studio Build Tools as well as CUDA Toolkit installed see [the CUDA docs](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html) for more details. 
+
+## Installation
+
+The easiest way to install the package is to first create a new conda environment or virtualenv with python (ideally >= version 3.8) and also pip, then activate the environment and `pip install volume-segmantics`. If a CUDA-enabled build of PyTorch is not being installed by pip, you can try `pip install volume-segmantics --extra-index-url https://download.pytorch.org/whl` this particularity seems to be an issue on Windows. 
+
+## Configuration and command line use
+
+After installation, two new commands will be available from your terminal whilst your environment is activated, `model-train-2d` and `model-predict-2d`.
+
+These commands require access to some settings stored in YAML files. These need to be located in a directory named `volseg-settings` within the directory where you are running the commands. The settings files can be copied from [here](https://github.com/DiamondLightSource/volume-segmantics/releases/download/v0.3.1/volseg-settings.zip). 
+
+The file `2d_model_train_settings.yaml` can be edited in order to change training parameters such as number of epochs, loss functions, evaluation metrics and also model and encoder architectures. The file `2d_model_predict_settings.yaml` can be edited to change parameters such as the prediction "quality" e.g "low" quality refers to prediction of the volume segmentation by taking images along a single axis (images in the (x,y) plane). For "medium" and "high" quality, predictions are done along 3 axes and in 12 directions (3 axes, 4 rotations) respectively, before being combined by maximum probability. 
+
+### For training a 2d model on a 3d image volume and corresponding labels
+Run the following command. Input files can be in HDF5 or multi-page TIFF format.
+
+```shell
+model-train-2d --data path/to/image/data.h5 --labels path/to/corresponding/segmentation/labels.h5
+```
+
+Paths to multiple data and label volumes can be added after the `--data` and `--labels` flags respectively. A model will be trained according to the settings defined in `/volseg-settings/2d_model_train_settings.yaml` and saved to your working directory. In addition, a figure showing "ground truth" segmentation vs model segmentation for some images in the validation set will be saved. 
+
+### For 3d volume segmentation prediction using a 2d model
+Run the following command. Input image files can be in HDF5 or multi-page TIFF format.
+
+```shell
+model-predict-2d path/to/model_file.pytorch path/to/data_for_prediction.h5
+```
+
+The input data will be segmented using the input model following the settings specified in `volseg-settings/2d_model_predict_settings.yaml`. An HDF5 file containing the segmented volume will be saved to your working directory.
+
+### Tutorial using example data
+
+A tutorial is available [here](training_data/README.md) that provides a walk-through of how to segment blood vessels from synchrotron X-ray micro-CT data collected on a sample of human placental tissue.
+
+## Currently supported model architectures and encoders
+
+The model architectures which are currently available and tested are: 
+- U-Net
+- U-Net++
+- FPN
+- DeepLabV3
+- DeepLabV3+
+- MA-Net
+- LinkNet
+- PAN
+
+The pre-trained encoders that can be used with these architectures are: 
+- ResNet-34
+- ResNet50
+- ResNeXt-50_32x4d
+- Efficientnet-b3
+- Efficientnet-b4
+- Resnest50d\*
+- Resnest101e\*
+
+\* Encoders with asterisk not compatible with PAN.
+
+## Using the API
+
+You can use the functionality of the package in your own program via the API, this is [documented here](https://diamondlightsource.github.io/volume-segmantics/). This interface is the one used by [SuRVoS2](https://github.com/DiamondLightSource/SuRVoS2), a client/server GUI application that allows fast annotation and segmentation of volumetric data. 
+
+## Contributing
+
+We welcome contributions from the community. Please take a look at out [contribution guidelines](https://github.com/DiamondLightSource/volume-segmantics/blob/main/CONTRIBUTING.md) for more information.
+
+## Citation
+
+If you use this package for you research, please cite:
+
+[King O.N.F, Bellos, D. and Basham, M. (2022). Volume Segmantics: A Python Package for Semantic Segmentation of Volumetric Data Using Pre-trained PyTorch Deep Learning Models. Journal of Open Source Software, 7(78), 4691. doi: 10.21105/joss.04691](https://doi.org/10.21105/joss.04691)
+
+```bibtex
+@article{King2022,
+    doi = {10.21105/joss.04691},
+    url = {https://doi.org/10.21105/joss.04691},
+    year = {2022},
+    publisher = {The Open Journal},
+    volume = {7},
+    number = {78},
+    pages = {4691},
+    author = {Oliver N. F. King and Dimitrios Bellos and Mark Basham},
+    title = {Volume Segmantics: A Python Package for Semantic Segmentation of Volumetric Data Using Pre-trained PyTorch Deep Learning Models},
+    journal = {Journal of Open Source Software} }
+```
+
+## References
+
+**Albumentations**
+
+Buslaev, A., Iglovikov, V.I., Khvedchenya, E., Parinov, A., Druzhinin, M., and Kalinin, A.A. (2020). Albumentations: Fast and Flexible Image Augmentations. Information 11. [https://doi.org/10.3390/info11020125](https://doi.org/10.3390/info11020125)
+
+**Segmentation Models PyTorch**
+
+Yakubovskiy, P. (2020). Segmentation Models Pytorch. [GitHub](https://github.com/qubvel/segmentation_models.pytorch)
+
+**PyTorch-3dUnet**
+
+Wolny, A., Cerrone, L., Vijayan, A., Tofanelli, R., Barro, A.V., Louveaux, M., Wenzl, C., Strauss, S., Wilson-Sánchez, D., Lymbouridou, R., et al. (2020). Accurate and versatile 3D segmentation of plant tissues at cellular resolution. ELife 9, e57613. [https://doi.org/10.7554/eLife.57613](https://doi.org/10.7554/eLife.57613)
 
-setup(**setup_kwargs)
```

