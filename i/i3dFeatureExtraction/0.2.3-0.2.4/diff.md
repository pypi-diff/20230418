# Comparing `tmp/i3dFeatureExtraction-0.2.3.tar.gz` & `tmp/i3dFeatureExtraction-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i3dFeatureExtraction-0.2.3.tar", last modified: Tue Apr 18 02:58:42 2023, max compression
+gzip compressed data, was "i3dFeatureExtraction-0.2.4.tar", last modified: Tue Apr 18 03:20:30 2023, max compression
```

## Comparing `i3dFeatureExtraction-0.2.3.tar` & `i3dFeatureExtraction-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 02:58:42.572126 i3dFeatureExtraction-0.2.3/
--rw-rw-rw-   0        0        0     1355 2023-04-17 09:06:40.000000 i3dFeatureExtraction-0.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0      419 2023-04-18 02:58:42.571100 i3dFeatureExtraction-0.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 02:58:42.540444 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/
--rw-rw-rw-   0        0        0     4088 2023-04-18 02:41:47.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/__init__.py
--rw-rw-rw-   0        0        0    10425 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/extract_features.py
--rw-rw-rw-   0        0        0     2294 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/extract_features_org.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:58:42.567096 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/models/
--rw-rw-rw-   0        0        0        0 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/models/__init__.py
--rw-rw-rw-   0        0        0     2235 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/models/model_builder_video.py
--rw-rw-rw-   0        0        0     3803 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/models/nonlocal_helper.py
--rw-rw-rw-   0        0        0     7644 2023-03-27 13:19:26.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/models/resnet.py
--rw-rw-rw-   0        0        0     3992 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/models/resnet_helper.py
--rw-rw-rw-   0        0        0     3214 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/models/resnet_video_org.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:58:42.570098 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/utils/
--rw-rw-rw-   0        0        0        0 2023-04-18 02:56:31.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/utils/__init__.py
--rw-rw-rw-   0        0        0     2713 2023-03-31 07:30:57.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/utils/convert_weights.py
--rw-rw-rw-   0        0        0     3223 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/utils/pretrained_existed.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:58:42.557666 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction.egg-info/
--rw-rw-rw-   0        0        0      419 2023-04-18 02:58:42.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      761 2023-04-18 02:58:42.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 02:58:42.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      677 2023-04-18 02:58:42.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-18 02:58:42.000000 i3dFeatureExtraction-0.2.3/i3dFeatureExtraction.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 02:58:42.572126 i3dFeatureExtraction-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-04-18 02:58:19.000000 i3dFeatureExtraction-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 03:20:30.653809 i3dFeatureExtraction-0.2.4/
+-rw-rw-rw-   0        0        0     1355 2023-04-17 09:06:40.000000 i3dFeatureExtraction-0.2.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      419 2023-04-18 03:20:30.652807 i3dFeatureExtraction-0.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 03:20:30.627437 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/
+-rw-rw-rw-   0        0        0     4088 2023-04-18 02:41:47.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/__init__.py
+-rw-rw-rw-   0        0        0    10425 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/extract_features.py
+-rw-rw-rw-   0        0        0     2294 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/extract_features_org.py
+drwxrwxrwx   0        0        0        0 2023-04-18 03:20:30.649019 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/models/
+-rw-rw-rw-   0        0        0        0 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/models/__init__.py
+-rw-rw-rw-   0        0        0     2235 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/models/model_builder_video.py
+-rw-rw-rw-   0        0        0     3803 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/models/nonlocal_helper.py
+-rw-rw-rw-   0        0        0     7644 2023-03-27 13:19:26.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/models/resnet.py
+-rw-rw-rw-   0        0        0     3992 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/models/resnet_helper.py
+-rw-rw-rw-   0        0        0     3214 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/models/resnet_video_org.py
+drwxrwxrwx   0        0        0        0 2023-04-18 03:20:30.651807 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-18 02:56:31.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/utils/__init__.py
+-rw-rw-rw-   0        0        0     2716 2023-04-18 03:18:53.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/utils/convert_weights.py
+-rw-rw-rw-   0        0        0     3223 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/utils/pretrained_existed.py
+drwxrwxrwx   0        0        0        0 2023-04-18 03:20:30.641665 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-04-18 03:20:30.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      761 2023-04-18 03:20:30.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 03:20:30.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      677 2023-04-18 03:20:30.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-18 03:20:30.000000 i3dFeatureExtraction-0.2.4/i3dFeatureExtraction.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 03:20:30.653809 i3dFeatureExtraction-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-04-18 03:20:04.000000 i3dFeatureExtraction-0.2.4/setup.py
```

### Comparing `i3dFeatureExtraction-0.2.3/LICENSE.txt` & `i3dFeatureExtraction-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/__init__.py` & `i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/__init__.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/extract_features.py` & `i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/extract_features.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/extract_features_org.py` & `i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/extract_features_org.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/models/model_builder_video.py` & `i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/models/model_builder_video.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/models/nonlocal_helper.py` & `i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/models/nonlocal_helper.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/models/resnet.py` & `i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/models/resnet.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/models/resnet_helper.py` & `i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/models/resnet_helper.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/models/resnet_video_org.py` & `i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/models/resnet_video_org.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/utils/convert_weights.py` & `i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/utils/convert_weights.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pickle
 import torch
 import re, os
 import sys, numpy
+from ..models.resnet import I3Res50
 
 def convert_weights(pkl_weight:str):
 	if not pkl_weight:
 		print("Error pkl weight input.")
 		return None
 	c2_weights = pkl_weight # 'pretrained/i3d_baseline_32x2_IN_pretrain_400k.pkl'
 	pth_weights_out = os.path.dirname(pkl_weight) + '/i3d_r50_kinetics.pth'
@@ -57,16 +58,16 @@
 			layer, block, module = nl_match.groups()
 			layer, block = int(layer), int(block)
 			name = 'nl.%s'%module
 			suffix = suffix_dict[key.split('_')[-1]]
 			new_key = 'layer%d.%d.%s.%s'%(layer-1, block, name, suffix)
 			key_map[new_key] = key
 
-	from models import resnet
-	pth = resnet.I3Res50(num_classes=400, use_nl=True)
+
+	pth = I3Res50(num_classes=400, use_nl=True)
 	state_dict = pth.state_dict()
 
 	new_state_dict = {key: torch.from_numpy(c2[key_map[key]]) for key in state_dict if key in key_map}
 	torch.save(new_state_dict, pth_weights_out)
 	torch.save(key_map, pth_weights_out+'.keymap')
 
 	# check if weight dimensions match
```

### Comparing `i3dFeatureExtraction-0.2.3/i3dFeatureExtraction/utils/pretrained_existed.py` & `i3dFeatureExtraction-0.2.4/i3dFeatureExtraction/utils/pretrained_existed.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.3/i3dFeatureExtraction.egg-info/SOURCES.txt` & `i3dFeatureExtraction-0.2.4/i3dFeatureExtraction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.3/i3dFeatureExtraction.egg-info/requires.txt` & `i3dFeatureExtraction-0.2.4/i3dFeatureExtraction.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.3/setup.py` & `i3dFeatureExtraction-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 DESCRIPTION = "This package helps extract i3D features with ResNet-50 backbone given a folder of videos"
 REQUIREMENTS = [i for i in open("requirements.txt").readlines()]
 setuptools.setup(
     name="i3dFeatureExtraction",
-    version="0.2.3",
+    version="0.2.4",
     author="Hao Vy Phan",
     author_email="vyhao03@gmail.com",
     description=DESCRIPTION,
     python_requires='>=3.8',
     packages=setuptools.find_packages(),
     classifiers = [
         "Programming Language :: Python :: 3",
```

