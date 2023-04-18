# Comparing `tmp/waveprop-0.0.3.tar.gz` & `tmp/waveprop-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waveprop-0.0.3.tar", last modified: Fri Jan  6 16:41:30 2023, max compression
+gzip compressed data, was "waveprop-0.0.4.tar", last modified: Tue Apr 18 13:03:23 2023, max compression
```

## Comparing `waveprop-0.0.3.tar` & `waveprop-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2023-01-06 16:41:30.649477 waveprop-0.0.3/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     1068 2022-09-07 22:10:39.000000 waveprop-0.0.3/LICENSE
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)       41 2022-09-07 22:17:27.000000 waveprop-0.0.3/MANIFEST.in
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    10453 2023-01-06 16:41:30.649477 waveprop-0.0.3/PKG-INFO
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    10040 2023-01-06 16:41:03.000000 waveprop-0.0.3/README.md
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)       38 2023-01-06 16:41:30.649477 waveprop-0.0.3/setup.cfg
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)      977 2023-01-06 16:40:03.000000 waveprop-0.0.3/setup.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2023-01-06 16:41:30.649477 waveprop-0.0.3/waveprop/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)        0 2022-09-07 22:10:39.000000 waveprop-0.0.3/waveprop/__init__.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     5155 2022-09-07 22:10:39.000000 waveprop-0.0.3/waveprop/color.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     4682 2022-09-07 22:10:39.000000 waveprop-0.0.3/waveprop/condition.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    13252 2023-01-06 16:38:43.000000 waveprop-0.0.3/waveprop/dataset_util.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     2912 2022-09-07 22:10:39.000000 waveprop-0.0.3/waveprop/devices.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     2841 2022-09-07 22:10:39.000000 waveprop-0.0.3/waveprop/fraunhofer.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    12063 2022-09-07 22:10:39.000000 waveprop-0.0.3/waveprop/fresnel.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     1453 2022-09-07 22:10:39.000000 waveprop-0.0.3/waveprop/holography.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)      433 2022-09-07 22:10:39.000000 waveprop-0.0.3/waveprop/io.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2023-01-06 16:41:30.649477 waveprop-0.0.3/waveprop/lookup/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    12067 2022-09-07 22:10:39.000000 waveprop-0.0.3/waveprop/lookup/cie-cmf.txt
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     9601 2022-09-07 22:10:39.000000 waveprop-0.0.3/waveprop/lookup/illuminant_d65.txt
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)      987 2023-01-06 16:38:43.000000 waveprop-0.0.3/waveprop/noise.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     4866 2023-01-06 16:38:43.000000 waveprop-0.0.3/waveprop/pytorch_util.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    30434 2022-09-07 22:10:39.000000 waveprop-0.0.3/waveprop/rs.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     6382 2023-01-06 16:38:43.000000 waveprop-0.0.3/waveprop/simulation.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    17749 2022-09-07 22:10:39.000000 waveprop-0.0.3/waveprop/slm.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     1871 2022-09-07 22:10:39.000000 waveprop-0.0.3/waveprop/spherical.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    18235 2023-01-06 16:38:43.000000 waveprop-0.0.3/waveprop/util.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2023-01-06 16:41:30.649477 waveprop-0.0.3/waveprop.egg-info/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    10453 2023-01-06 16:41:30.000000 waveprop-0.0.3/waveprop.egg-info/PKG-INFO
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)      583 2023-01-06 16:41:30.000000 waveprop-0.0.3/waveprop.egg-info/SOURCES.txt
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)        1 2023-01-06 16:41:30.000000 waveprop-0.0.3/waveprop.egg-info/dependency_links.txt
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)       89 2023-01-06 16:41:30.000000 waveprop-0.0.3/waveprop.egg-info/requires.txt
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)        9 2023-01-06 16:41:30.000000 waveprop-0.0.3/waveprop.egg-info/top_level.txt
+drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2023-04-18 13:03:23.234928 waveprop-0.0.4/
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1068 2022-12-29 21:13:18.000000 waveprop-0.0.4/LICENSE
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)       41 2022-12-29 21:13:18.000000 waveprop-0.0.4/MANIFEST.in
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)    10489 2023-04-18 13:03:23.234928 waveprop-0.0.4/PKG-INFO
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)    10040 2023-04-18 12:55:35.000000 waveprop-0.0.4/README.md
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)       38 2023-04-18 13:03:23.234928 waveprop-0.0.4/setup.cfg
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      977 2023-04-18 13:03:09.000000 waveprop-0.0.4/setup.py
+drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2023-04-18 13:03:23.234928 waveprop-0.0.4/waveprop/
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)        0 2021-09-03 14:33:06.000000 waveprop-0.0.4/waveprop/__init__.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     5155 2022-12-29 21:13:18.000000 waveprop-0.0.4/waveprop/color.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4682 2022-12-29 21:13:18.000000 waveprop-0.0.4/waveprop/condition.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)    13343 2023-04-18 12:59:24.000000 waveprop-0.0.4/waveprop/dataset_util.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2912 2022-12-29 21:13:18.000000 waveprop-0.0.4/waveprop/devices.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     2841 2022-12-29 21:13:18.000000 waveprop-0.0.4/waveprop/fraunhofer.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)    12063 2022-12-29 21:58:55.000000 waveprop-0.0.4/waveprop/fresnel.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1453 2022-12-29 21:13:18.000000 waveprop-0.0.4/waveprop/holography.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      433 2022-12-29 21:13:18.000000 waveprop-0.0.4/waveprop/io.py
+drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2023-04-18 13:03:23.234928 waveprop-0.0.4/waveprop/lookup/
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)    12067 2021-10-08 09:21:37.000000 waveprop-0.0.4/waveprop/lookup/cie-cmf.txt
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     9601 2021-10-08 10:44:58.000000 waveprop-0.0.4/waveprop/lookup/illuminant_d65.txt
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      987 2023-04-18 12:55:35.000000 waveprop-0.0.4/waveprop/noise.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     4866 2023-04-18 12:55:35.000000 waveprop-0.0.4/waveprop/pytorch_util.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)    30434 2022-12-29 21:58:55.000000 waveprop-0.0.4/waveprop/rs.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     6382 2023-04-18 12:58:27.000000 waveprop-0.0.4/waveprop/simulation.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)    17749 2022-12-29 21:13:18.000000 waveprop-0.0.4/waveprop/slm.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)     1871 2022-12-29 21:13:18.000000 waveprop-0.0.4/waveprop/spherical.py
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)    18235 2023-04-18 12:58:27.000000 waveprop-0.0.4/waveprop/util.py
+drwxrwxr-x   0 bezzam    (1001) bezzam    (1001)        0 2023-04-18 13:03:23.234928 waveprop-0.0.4/waveprop.egg-info/
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)    10489 2023-04-18 13:03:23.000000 waveprop-0.0.4/waveprop.egg-info/PKG-INFO
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)      583 2023-04-18 13:03:23.000000 waveprop-0.0.4/waveprop.egg-info/SOURCES.txt
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)        1 2023-04-18 13:03:23.000000 waveprop-0.0.4/waveprop.egg-info/dependency_links.txt
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)       89 2023-04-18 13:03:23.000000 waveprop-0.0.4/waveprop.egg-info/requires.txt
+-rw-rw-r--   0 bezzam    (1001) bezzam    (1001)        9 2023-04-18 13:03:23.000000 waveprop-0.0.4/waveprop.egg-info/top_level.txt
```

### Comparing `waveprop-0.0.3/LICENSE` & `waveprop-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/PKG-INFO` & `waveprop-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: waveprop
-Version: 0.0.3
+Version: 0.0.4
 Summary: Functions and scripts to simulate free-space optical wave propagation.
 Home-page: https://github.com/ebezzam/waveprop
 Author: Eric Bezzam
 Author-email: ebezzam@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # waveprop: Diffraction-based wave propagation simulator with PyTorch support
@@ -208,7 +210,8 @@
     - Monochromatic: https://github.com/rafael-fuente/Diffraction-Simulations--Angular-Spectrum-Method/blob/5b3610643b97ab6b81c80ef4c8aa5b0d9501f314/diffractsim/monochromatic_simulator.py#L191
     - Polychromatic: https://github.com/rafael-fuente/Diffraction-Simulations--Angular-Spectrum-Method/blob/5b3610643b97ab6b81c80ef4c8aa5b0d9501f314/diffractsim/polychromatic_simulator.py#L190
   
 
 ## License
 
 MIT
+
```

### Comparing `waveprop-0.0.3/README.md` & `waveprop-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/setup.py` & `waveprop-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="waveprop",
-    version="0.0.3",
+    version="0.0.4",
     author="Eric Bezzam",
     author_email="ebezzam@gmail.com",
     description="Functions and scripts to simulate free-space optical wave propagation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ebezzam/waveprop",
     # download_url = "https://github.com/ebezzam/waveprop/archive/refs/tags/v0.0.1.tar.gz",
```

### Comparing `waveprop-0.0.3/waveprop/color.py` & `waveprop-0.0.4/waveprop/color.py`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/waveprop/condition.py` & `waveprop-0.0.4/waveprop/condition.py`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/waveprop/dataset_util.py` & `waveprop-0.0.4/waveprop/dataset_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import pandas as pd
 from torch.utils.data import Dataset
 from torchvision import transforms, datasets
 import torch.nn.functional as F
 from PIL import Image
 import os
 import numpy as np
 import glob
-from waveprop.devices import sensor_dict
 from waveprop.simulation import FarFieldSimulator
 from abc import abstractmethod
 
 
 class Datasets(object):
     MNIST = "MNIST"
     CIFAR10 = "CIFAR"
@@ -332,15 +330,19 @@
         grayscale
         device
         scale
         kwargs
         """
 
         self.root_dir = root_dir
-        self.df = pd.read_csv(captions_file)
+        try:
+            import pandas as pd
+            self.df = pd.read_csv(captions_file)
+        except ImportError:
+            raise ImportError("Please install pandas to use this dataset")
         self.device = device
 
         transform_list = []
         if vflip:
             transform_list.append(transforms.RandomVerticalFlip(p=1.0))
         if grayscale:
             transform_list.append(transforms.Grayscale())
```

### Comparing `waveprop-0.0.3/waveprop/devices.py` & `waveprop-0.0.4/waveprop/devices.py`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/waveprop/fraunhofer.py` & `waveprop-0.0.4/waveprop/fraunhofer.py`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/waveprop/fresnel.py` & `waveprop-0.0.4/waveprop/fresnel.py`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/waveprop/holography.py` & `waveprop-0.0.4/waveprop/holography.py`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/waveprop/lookup/cie-cmf.txt` & `waveprop-0.0.4/waveprop/lookup/cie-cmf.txt`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/waveprop/lookup/illuminant_d65.txt` & `waveprop-0.0.4/waveprop/lookup/illuminant_d65.txt`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/waveprop/noise.py` & `waveprop-0.0.4/waveprop/noise.py`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/waveprop/pytorch_util.py` & `waveprop-0.0.4/waveprop/pytorch_util.py`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/waveprop/rs.py` & `waveprop-0.0.4/waveprop/rs.py`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/waveprop/simulation.py` & `waveprop-0.0.4/waveprop/simulation.py`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/waveprop/slm.py` & `waveprop-0.0.4/waveprop/slm.py`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/waveprop/spherical.py` & `waveprop-0.0.4/waveprop/spherical.py`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/waveprop/util.py` & `waveprop-0.0.4/waveprop/util.py`

 * *Files identical despite different names*

### Comparing `waveprop-0.0.3/waveprop.egg-info/PKG-INFO` & `waveprop-0.0.4/waveprop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: waveprop
-Version: 0.0.3
+Version: 0.0.4
 Summary: Functions and scripts to simulate free-space optical wave propagation.
 Home-page: https://github.com/ebezzam/waveprop
 Author: Eric Bezzam
 Author-email: ebezzam@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # waveprop: Diffraction-based wave propagation simulator with PyTorch support
@@ -208,7 +210,8 @@
     - Monochromatic: https://github.com/rafael-fuente/Diffraction-Simulations--Angular-Spectrum-Method/blob/5b3610643b97ab6b81c80ef4c8aa5b0d9501f314/diffractsim/monochromatic_simulator.py#L191
     - Polychromatic: https://github.com/rafael-fuente/Diffraction-Simulations--Angular-Spectrum-Method/blob/5b3610643b97ab6b81c80ef4c8aa5b0d9501f314/diffractsim/polychromatic_simulator.py#L190
   
 
 ## License
 
 MIT
+
```

### Comparing `waveprop-0.0.3/waveprop.egg-info/SOURCES.txt` & `waveprop-0.0.4/waveprop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

