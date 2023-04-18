# Comparing `tmp/i3dFeatureExtraction-0.2.1.tar.gz` & `tmp/i3dFeatureExtraction-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i3dFeatureExtraction-0.2.1.tar", last modified: Tue Apr 18 01:44:08 2023, max compression
+gzip compressed data, was "i3dFeatureExtraction-0.2.2.tar", last modified: Tue Apr 18 02:51:46 2023, max compression
```

## Comparing `i3dFeatureExtraction-0.2.1.tar` & `i3dFeatureExtraction-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 01:44:08.702154 i3dFeatureExtraction-0.2.1/
--rw-rw-rw-   0        0        0     1355 2023-04-17 09:06:40.000000 i3dFeatureExtraction-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0      419 2023-04-18 01:44:08.702154 i3dFeatureExtraction-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 01:44:08.670901 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/
--rw-rw-rw-   0        0        0     4087 2023-04-17 09:23:51.000000 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/__init__.py
--rw-rw-rw-   0        0        0    10423 2023-04-17 01:43:12.000000 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/extract_features.py
--rw-rw-rw-   0        0        0     2294 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/extract_features_org.py
--rw-rw-rw-   0        0        0     2136 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/extract_main.py
-drwxrwxrwx   0        0        0        0 2023-04-18 01:44:08.702154 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/models/
--rw-rw-rw-   0        0        0        0 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/models/__init__.py
--rw-rw-rw-   0        0        0     2235 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/models/model_builder_video.py
--rw-rw-rw-   0        0        0     3803 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/models/nonlocal_helper.py
--rw-rw-rw-   0        0        0     7644 2023-03-27 13:19:26.000000 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/models/resnet.py
--rw-rw-rw-   0        0        0     3998 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/models/resnet_helper.py
--rw-rw-rw-   0        0        0     3220 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/models/resnet_video_org.py
-drwxrwxrwx   0        0        0        0 2023-04-18 01:44:08.686526 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction.egg-info/
--rw-rw-rw-   0        0        0      419 2023-04-18 01:44:08.000000 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      664 2023-04-18 01:44:08.000000 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 01:44:08.000000 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      677 2023-04-18 01:44:08.000000 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-18 01:44:08.000000 i3dFeatureExtraction-0.2.1/i3dFeatureExtraction.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 01:44:08.702154 i3dFeatureExtraction-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-04-18 01:43:19.000000 i3dFeatureExtraction-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:51:46.282461 i3dFeatureExtraction-0.2.2/
+-rw-rw-rw-   0        0        0     1355 2023-04-17 09:06:40.000000 i3dFeatureExtraction-0.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      419 2023-04-18 02:51:46.281461 i3dFeatureExtraction-0.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 02:51:46.250461 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/
+-rw-rw-rw-   0        0        0     4088 2023-04-18 02:41:47.000000 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/__init__.py
+-rw-rw-rw-   0        0        0    10425 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/extract_features.py
+-rw-rw-rw-   0        0        0     2294 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/extract_features_org.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:51:46.280679 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/models/
+-rw-rw-rw-   0        0        0        0 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/models/__init__.py
+-rw-rw-rw-   0        0        0     2235 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/models/model_builder_video.py
+-rw-rw-rw-   0        0        0     3803 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/models/nonlocal_helper.py
+-rw-rw-rw-   0        0        0     7644 2023-03-27 13:19:26.000000 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/models/resnet.py
+-rw-rw-rw-   0        0        0     3992 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/models/resnet_helper.py
+-rw-rw-rw-   0        0        0     3214 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/models/resnet_video_org.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:51:46.271462 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-04-18 02:51:45.000000 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-04-18 02:51:46.000000 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 02:51:45.000000 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      677 2023-04-18 02:51:45.000000 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-18 02:51:45.000000 i3dFeatureExtraction-0.2.2/i3dFeatureExtraction.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 02:51:46.282461 i3dFeatureExtraction-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-04-18 02:51:19.000000 i3dFeatureExtraction-0.2.2/setup.py
```

### Comparing `i3dFeatureExtraction-0.2.1/LICENSE.txt` & `i3dFeatureExtraction-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/__init__.py` & `i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import torch.nn.functional as F
 import torch.optim as optim
 from torch.optim import lr_scheduler
 from torch.autograd import Variable
 import torchvision
 import os
 
-from extract_features import I3DFeaturesExtractor
+from .extract_features import I3DFeaturesExtractor
 
 class FeatureExtraction:
     def __init__(self, datasetpath="samplevideos/", outputpath="output", 
                  pretrainedpath="pretrained/i3d_r50_kinetics.pth",
                  frequency=16, batch_size=20, sample_mode="oversample"):
         self.datasetpath = datasetpath
         self.outputpath = outputpath
```

### Comparing `i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/extract_features.py` & `i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/extract_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import numpy as np
 import torch
 from natsort import natsorted
 from PIL import Image
-from models.resnet import i3_res50
+from .models.resnet import i3_res50
 from torch.autograd import Variable
 import ffmpeg
-from utils.pretrained_existed import get_pth_weight
+from .utils.pretrained_existed import get_pth_weight
 
 
 class I3DFeaturesExtractor:
     def __init__(self, freq=16, sample_mode='oversample',
                  batch_size=20, 
                  pretrainedpath = "pretrained/i3d_r50_kinetics.pth"):
         os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
```

### Comparing `i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/extract_features_org.py` & `i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/extract_features_org.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/models/model_builder_video.py` & `i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/models/model_builder_video.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/models/nonlocal_helper.py` & `i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/models/nonlocal_helper.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/models/resnet.py` & `i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/models/resnet.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/models/resnet_helper.py` & `i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/models/resnet_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-import models.nonlocal_helper as nonlocal_helper
+import .nonlocal_helper as nonlocal_helper
 
 
 # 3d bottleneck
 # 3d conv in the first conv (3x1x1)
 def bottleneck_transformation_3d(
         model, blob_in, dim_in, dim_out, stride, prefix, dim_inner, group=1,
         use_temp_conv=1, temp_stride=1):
```

### Comparing `i3dFeatureExtraction-0.2.1/i3dFeatureExtraction/models/resnet_video_org.py` & `i3dFeatureExtraction-0.2.2/i3dFeatureExtraction/models/resnet_video_org.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import models.resnet_helper as resnet_helper
+import .resnet_helper as resnet_helper
 import numpy as np
 
 
 def create_model(model, data, labels, split, use_nl):
     group = 1
     width_per_group = 64
     batch_size = 8
```

### Comparing `i3dFeatureExtraction-0.2.1/i3dFeatureExtraction.egg-info/SOURCES.txt` & `i3dFeatureExtraction-0.2.2/i3dFeatureExtraction.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE.txt
 setup.py
 i3dFeatureExtraction/__init__.py
 i3dFeatureExtraction/extract_features.py
 i3dFeatureExtraction/extract_features_org.py
-i3dFeatureExtraction/extract_main.py
 i3dFeatureExtraction.egg-info/PKG-INFO
 i3dFeatureExtraction.egg-info/SOURCES.txt
 i3dFeatureExtraction.egg-info/dependency_links.txt
 i3dFeatureExtraction.egg-info/requires.txt
 i3dFeatureExtraction.egg-info/top_level.txt
 i3dFeatureExtraction/models/__init__.py
 i3dFeatureExtraction/models/model_builder_video.py
```

### Comparing `i3dFeatureExtraction-0.2.1/i3dFeatureExtraction.egg-info/requires.txt` & `i3dFeatureExtraction-0.2.2/i3dFeatureExtraction.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.1/setup.py` & `i3dFeatureExtraction-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 DESCRIPTION = "This package helps extract i3D features with ResNet-50 backbone given a folder of videos"
 REQUIREMENTS = [i for i in open("requirements.txt").readlines()]
 setuptools.setup(
     name="i3dFeatureExtraction",
-    version="0.2.1",
+    version="0.2.2",
     author="Hao Vy Phan",
     author_email="vyhao03@gmail.com",
     description=DESCRIPTION,
     python_requires='>=3.8',
     packages=setuptools.find_packages(),
     classifiers = [
         "Programming Language :: Python :: 3",
```

