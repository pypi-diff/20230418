# Comparing `tmp/i3dFeatureExtraction-0.2.5.tar.gz` & `tmp/i3dFeatureExtraction-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i3dFeatureExtraction-0.2.5.tar", last modified: Tue Apr 18 04:20:52 2023, max compression
+gzip compressed data, was "i3dFeatureExtraction-0.2.6.tar", last modified: Tue Apr 18 05:18:51 2023, max compression
```

## Comparing `i3dFeatureExtraction-0.2.5.tar` & `i3dFeatureExtraction-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 04:20:52.531341 i3dFeatureExtraction-0.2.5/
--rw-rw-rw-   0        0        0     1355 2023-04-17 09:06:40.000000 i3dFeatureExtraction-0.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0      419 2023-04-18 04:20:52.531341 i3dFeatureExtraction-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3196 2023-04-18 04:20:29.000000 i3dFeatureExtraction-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 04:20:52.419896 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/
--rw-rw-rw-   0        0        0     4088 2023-04-18 02:41:47.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/__init__.py
--rw-rw-rw-   0        0        0    10425 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/extract_features.py
--rw-rw-rw-   0        0        0     2294 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/extract_features_org.py
-drwxrwxrwx   0        0        0        0 2023-04-18 04:20:52.480630 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/models/
--rw-rw-rw-   0        0        0        0 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/models/__init__.py
--rw-rw-rw-   0        0        0     2235 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/models/model_builder_video.py
--rw-rw-rw-   0        0        0     3803 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/models/nonlocal_helper.py
--rw-rw-rw-   0        0        0     7644 2023-03-27 13:19:26.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/models/resnet.py
--rw-rw-rw-   0        0        0     3992 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/models/resnet_helper.py
--rw-rw-rw-   0        0        0     3214 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/models/resnet_video_org.py
-drwxrwxrwx   0        0        0        0 2023-04-18 04:20:52.511133 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/utils/
--rw-rw-rw-   0        0        0        0 2023-04-18 02:56:31.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/utils/__init__.py
--rw-rw-rw-   0        0        0     2716 2023-04-18 03:18:53.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/utils/convert_weights.py
--rw-rw-rw-   0        0        0     3223 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/utils/pretrained_existed.py
-drwxrwxrwx   0        0        0        0 2023-04-18 04:20:52.470526 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction.egg-info/
--rw-rw-rw-   0        0        0      419 2023-04-18 04:20:51.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      771 2023-04-18 04:20:52.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 04:20:51.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      677 2023-04-18 04:20:51.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-18 04:20:51.000000 i3dFeatureExtraction-0.2.5/i3dFeatureExtraction.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 04:20:52.531341 i3dFeatureExtraction-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-04-18 04:05:41.000000 i3dFeatureExtraction-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:18:51.698823 i3dFeatureExtraction-0.2.6/
+-rw-rw-rw-   0        0        0     1355 2023-04-17 09:06:40.000000 i3dFeatureExtraction-0.2.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     3510 2023-04-18 05:18:51.698823 i3dFeatureExtraction-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2846 2023-04-18 05:17:57.000000 i3dFeatureExtraction-0.2.6/README.md
+-rw-rw-rw-   0        0        0     3051 2023-04-18 05:17:59.000000 i3dFeatureExtraction-0.2.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-18 05:18:51.661048 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/
+-rw-rw-rw-   0        0        0     4088 2023-04-18 02:41:47.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/__init__.py
+-rw-rw-rw-   0        0        0    10425 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/extract_features.py
+-rw-rw-rw-   0        0        0     2294 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/extract_features_org.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:18:51.698823 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/models/
+-rw-rw-rw-   0        0        0        0 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/models/__init__.py
+-rw-rw-rw-   0        0        0     2235 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/models/model_builder_video.py
+-rw-rw-rw-   0        0        0     3803 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/models/nonlocal_helper.py
+-rw-rw-rw-   0        0        0     7644 2023-03-27 13:19:26.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/models/resnet.py
+-rw-rw-rw-   0        0        0     3992 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/models/resnet_helper.py
+-rw-rw-rw-   0        0        0     3214 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/models/resnet_video_org.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:18:51.698823 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-18 02:56:31.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/utils/__init__.py
+-rw-rw-rw-   0        0        0     2716 2023-04-18 03:18:53.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/utils/convert_weights.py
+-rw-rw-rw-   0        0        0     3223 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/utils/pretrained_existed.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:18:51.683186 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction.egg-info/
+-rw-rw-rw-   0        0        0     3510 2023-04-18 05:18:51.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      782 2023-04-18 05:18:51.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:18:51.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      677 2023-04-18 05:18:51.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-18 05:18:51.000000 i3dFeatureExtraction-0.2.6/i3dFeatureExtraction.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 05:18:51.698823 i3dFeatureExtraction-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      745 2023-04-18 05:06:25.000000 i3dFeatureExtraction-0.2.6/setup.py
```

### Comparing `i3dFeatureExtraction-0.2.5/LICENSE.txt` & `i3dFeatureExtraction-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.5/README.md` & `i3dFeatureExtraction-0.2.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -46,20 +46,14 @@
     outputpath = "directory/to/store/output/numpy/files",
     datasetpath="directory/of/input/videos",
     pretrainedpath = "path/to/i3D/pretrained/weight",
     sample_mode = "oversample/center_crop"
 )
 ```
 
-[//]: # (---)
-
-[//]: # (## Package structure)
-
-[//]: # (This implementation has been transformed into object-oriented programming style with Python classes. The motivation behind the object-oriented transformation was to make the code more modular, reusable, and easier to extend. The following classes have been added to the implementation:)
-
 ---
 
 ## Credits
 This code is based on the following repositories:
 * [pytorch-resnet3d](https://github.com/Tushar-N/pytorch-resnet3d)
 * [pytorch-i3d-feature-extraction](https://github.com/Finspire13/pytorch-i3d-feature-extraction)
 * [E2E-Action-Segmentation/feature_extraction/](https://github.com/nguyenphwork/E2E-Action-Segmentation/tree/main/feature_extraction)
```

### Comparing `i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/__init__.py` & `i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/__init__.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/extract_features.py` & `i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/extract_features.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/extract_features_org.py` & `i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/extract_features_org.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/models/model_builder_video.py` & `i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/models/model_builder_video.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/models/nonlocal_helper.py` & `i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/models/nonlocal_helper.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/models/resnet.py` & `i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/models/resnet.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/models/resnet_helper.py` & `i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/models/resnet_helper.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/models/resnet_video_org.py` & `i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/models/resnet_video_org.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/utils/convert_weights.py` & `i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/utils/convert_weights.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.5/i3dFeatureExtraction/utils/pretrained_existed.py` & `i3dFeatureExtraction-0.2.6/i3dFeatureExtraction/utils/pretrained_existed.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.5/i3dFeatureExtraction.egg-info/SOURCES.txt` & `i3dFeatureExtraction-0.2.6/i3dFeatureExtraction.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE.txt
 README.md
+README.rst
 setup.py
 i3dFeatureExtraction/__init__.py
 i3dFeatureExtraction/extract_features.py
 i3dFeatureExtraction/extract_features_org.py
 i3dFeatureExtraction.egg-info/PKG-INFO
 i3dFeatureExtraction.egg-info/SOURCES.txt
 i3dFeatureExtraction.egg-info/dependency_links.txt
```

### Comparing `i3dFeatureExtraction-0.2.5/i3dFeatureExtraction.egg-info/requires.txt` & `i3dFeatureExtraction-0.2.6/i3dFeatureExtraction.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.5/setup.py` & `i3dFeatureExtraction-0.2.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import setuptools
 
 DESCRIPTION = "This package helps extract i3D features with ResNet-50 backbone given a folder of videos"
 REQUIREMENTS = [i for i in open("requirements.txt").readlines()]
 setuptools.setup(
     name="i3dFeatureExtraction",
-    version="0.2.5",
+    version="0.2.6",
     author="Hao Vy Phan",
     author_email="vyhao03@gmail.com",
     description=DESCRIPTION,
+    long_description = open('README.rst').read(),
+    long_description_content_type='text/x-rst',
     python_requires='>=3.8',
     packages=setuptools.find_packages(),
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: Freely Distributable",
         "Operating System :: Microsoft :: Windows"
     ],
```

