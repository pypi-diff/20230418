# Comparing `tmp/lungmask-0.2.13.tar.gz` & `tmp/lungmask-0.2.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lungmask-0.2.13.tar", last modified: Thu Feb  9 22:03:33 2023, max compression
+gzip compressed data, was "lungmask-0.2.14.tar", last modified: Tue Apr 18 14:03:51 2023, max compression
```

## Comparing `lungmask-0.2.13.tar` & `lungmask-0.2.14.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 22:03:33.109856 lungmask-0.2.13/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-09 22:03:23.000000 lungmask-0.2.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-02-09 22:03:33.109856 lungmask-0.2.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-02-09 22:03:23.000000 lungmask-0.2.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 22:03:33.109856 lungmask-0.2.13/lungmask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 22:03:23.000000 lungmask-0.2.13/lungmask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-02-09 22:03:23.000000 lungmask-0.2.13/lungmask/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-02-09 22:03:23.000000 lungmask-0.2.13/lungmask/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-02-09 22:03:23.000000 lungmask-0.2.13/lungmask/resunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-02-09 22:03:23.000000 lungmask-0.2.13/lungmask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 22:03:33.109856 lungmask-0.2.13/lungmask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-02-09 22:03:33.000000 lungmask-0.2.13/lungmask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-09 22:03:33.000000 lungmask-0.2.13/lungmask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 22:03:33.000000 lungmask-0.2.13/lungmask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-09 22:03:33.000000 lungmask-0.2.13/lungmask.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-09 22:03:33.000000 lungmask-0.2.13/lungmask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-09 22:03:33.000000 lungmask-0.2.13/lungmask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 22:03:33.109856 lungmask-0.2.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-02-09 22:03:23.000000 lungmask-0.2.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:03:51.331893 lungmask-0.2.14/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 14:03:36.000000 lungmask-0.2.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-18 14:03:51.331893 lungmask-0.2.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-18 14:03:36.000000 lungmask-0.2.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:03:51.331893 lungmask-0.2.14/lungmask/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 14:03:37.000000 lungmask-0.2.14/lungmask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-18 14:03:37.000000 lungmask-0.2.14/lungmask/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 2023-04-18 14:03:37.000000 lungmask-0.2.14/lungmask/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-18 14:03:37.000000 lungmask-0.2.14/lungmask/resunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-04-18 14:03:37.000000 lungmask-0.2.14/lungmask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:03:51.331893 lungmask-0.2.14/lungmask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-18 14:03:51.000000 lungmask-0.2.14/lungmask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-18 14:03:51.000000 lungmask-0.2.14/lungmask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:03:51.000000 lungmask-0.2.14/lungmask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 14:03:51.000000 lungmask-0.2.14/lungmask.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 14:03:51.000000 lungmask-0.2.14/lungmask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 14:03:51.000000 lungmask-0.2.14/lungmask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-18 14:03:37.000000 lungmask-0.2.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:03:51.331893 lungmask-0.2.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-18 14:03:37.000000 lungmask-0.2.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:03:51.331893 lungmask-0.2.14/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-18 14:03:37.000000 lungmask-0.2.14/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-18 14:03:37.000000 lungmask-0.2.14/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-18 14:03:37.000000 lungmask-0.2.14/tests/test_utils.py
```

### Comparing `lungmask-0.2.13/LICENSE` & `lungmask-0.2.14/LICENSE`

 * *Files identical despite different names*

### Comparing `lungmask-0.2.13/PKG-INFO` & `lungmask-0.2.14/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: lungmask
-Version: 0.2.13
+Version: 0.2.14
 Summary: Package for automated lung segmentation in CT
 Home-page: https://github.com/JoHof/lungmask
 Author: Johannes Hofmanninger
-Author-email: johannes.hofmanninger@meduniwien.ac.at
+Author-email: johannes.hofmanninger@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Automated lung segmentation in CT under presence of severe pathologies
 
 This package provides trained U-net models for lung segmentation. For now, four models are available:
 
 - U-net(R231): This model was trained on a large and diverse dataset that covers a wide range of visual variabiliy. The model performs segmentation on individual slices, extracts right-left lung seperately includes airpockets, tumors and effusions. The trachea will not be included in the lung segmentation. https://doi.org/10.1186/s41747-020-00173-2
 
-- U-net(LTRCLobes): This model was trained on a subset of the [LTRC](https://ltrcpublic.com) dataset. The model performs segmentation of individual lung-lobes but yields limited performance when dense pathologies are present or when fissures are not visible at every slice. 
+- U-net(LTRCLobes): This model was trained on a subset of the [LTRC](https://ltrcpublic.com) dataset. The model performs segmentation of individual lung-lobes but yields limited performance when dense pathologies are present or when fissures are not visible at every slice.
 
 - U-net(LTRCLobes_R231): This will run the R231 and LTRCLobes model and fuse the results. False negatives from LTRCLobes will be filled by R231 predictions and mapped to a neighbor label. False positives from LTRCLobes will be removed. The fusing process is computationally intensive and can, depdending on the data and results, take up to several minutes per volume.
 
 - [U-net(R231CovidWeb)](#COVID-19-Web)
 
 
 **Examples of the two models applied**. **Left:** U-net(R231), will distinguish between left and right lung and include very dense areas such as effusions (third row), tumor or severe fibrosis (fourth row) . **Right:** U-net(LTRLobes), will distinguish between lung lobes but will not include very dense areas. **LTRCLobes_R231** will fuse LTRCLobes and R231 results. **R231CovidWeb** is trained with aditional COVID-19 data.
@@ -69,41 +69,42 @@
 ```
 lungmask -h
 ```
 
 ### As a python module:
 
 ```
-from lungmask import mask
+from lungmask import LMInferer
 import SimpleITK as sitk
 
+inferer = LMInferer()
+
 input_image = sitk.ReadImage(INPUT)
-segmentation = mask.apply(input_image)  # default model is U-net(R231)
+segmentation = inferer.apply(input_image)  # default model is U-net(R231)
 ```
 input_image has to be a SimpleITK object.
 
 Load an alternative model like so:
 ```
-model = mask.get_model('unet','LTRCLobes')
-segmentation = mask.apply(input_image, model)
+inferer = LMInferer(modelname="R231CovidWeb")
 ```
 
-To use the model fusing capability for LTRCLobes_R231 use:
+To use the model fusing capability for (e.g. LTRCLobes_R231) use:
 ```
-segmentation = mask.apply_fused(input_image)
+inferer = LMInferer(modelname='LTRCLobes', fillmodel='R231')
 ```
 
 #### Numpy array support
 As of version 0.2.9, numpy arrays are supported as input volumes. This mode assumes the input numpy array has the following format for each axis:
 * first axis containing slices
 * second axis with chest to back
-* third axis with right to left 
+* third axis with right to left
 
 ## Limitations
-The model works on full slices only. The slice to process has to show the full lung and the lung has to be surrounded by tissue in order to get segmented. However, the model is quite stable to cases with a cropped field of view as long as the lung is surrounded by tissue. 
+The model works on full slices only. The slice to process has to show the full lung and the lung has to be surrounded by tissue in order to get segmented. However, the model is quite stable to cases with a cropped field of view as long as the lung is surrounded by tissue.
 
 ## COVID-19 Web
 ```
 lungmask INPUT OUTPUT --modelname R231CovidWeb
 ```
 The regular U-net(R231) model works very well for COVID-19 CT scans. However, collections of slices and case reports from the web are often cropped, annotated or encoded in regular image formats so that the original hounsfield unit (HU) values can only be estimated. The training data of the U-net(R231CovidWeb) model was augmented with COVID-19 slices that were mapped back from regular imaging formats to HU. The data was collected and prepared by MedSeg (http://medicalsegmentation.com/covid19/). While the regular U-net(R231) showed very good results for these images there may be cases for which this model will yield slighty improved segmentations. Note that you have to map images back to HU when using images from the web. This [blog post](https://medium.com/@hbjenssen/covid-19-radiology-data-collection-and-preparation-for-artificial-intelligence-4ecece97bb5b) describes how you can do that. Alternatively you can set the ```--noHU``` tag.
 ![alt text](figures/example_covid.jpg "COVID examples")
```

### Comparing `lungmask-0.2.13/README.md` & `lungmask-0.2.14/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automated lung segmentation in CT under presence of severe pathologies
 
 This package provides trained U-net models for lung segmentation. For now, four models are available:
 
 - U-net(R231): This model was trained on a large and diverse dataset that covers a wide range of visual variabiliy. The model performs segmentation on individual slices, extracts right-left lung seperately includes airpockets, tumors and effusions. The trachea will not be included in the lung segmentation. https://doi.org/10.1186/s41747-020-00173-2
 
-- U-net(LTRCLobes): This model was trained on a subset of the [LTRC](https://ltrcpublic.com) dataset. The model performs segmentation of individual lung-lobes but yields limited performance when dense pathologies are present or when fissures are not visible at every slice. 
+- U-net(LTRCLobes): This model was trained on a subset of the [LTRC](https://ltrcpublic.com) dataset. The model performs segmentation of individual lung-lobes but yields limited performance when dense pathologies are present or when fissures are not visible at every slice.
 
 - U-net(LTRCLobes_R231): This will run the R231 and LTRCLobes model and fuse the results. False negatives from LTRCLobes will be filled by R231 predictions and mapped to a neighbor label. False positives from LTRCLobes will be removed. The fusing process is computationally intensive and can, depdending on the data and results, take up to several minutes per volume.
 
 - [U-net(R231CovidWeb)](#COVID-19-Web)
 
 
 **Examples of the two models applied**. **Left:** U-net(R231), will distinguish between left and right lung and include very dense areas such as effusions (third row), tumor or severe fibrosis (fourth row) . **Right:** U-net(LTRLobes), will distinguish between lung lobes but will not include very dense areas. **LTRCLobes_R231** will fuse LTRCLobes and R231 results. **R231CovidWeb** is trained with aditional COVID-19 data.
@@ -56,41 +56,42 @@
 ```
 lungmask -h
 ```
 
 ### As a python module:
 
 ```
-from lungmask import mask
+from lungmask import LMInferer
 import SimpleITK as sitk
 
+inferer = LMInferer()
+
 input_image = sitk.ReadImage(INPUT)
-segmentation = mask.apply(input_image)  # default model is U-net(R231)
+segmentation = inferer.apply(input_image)  # default model is U-net(R231)
 ```
 input_image has to be a SimpleITK object.
 
 Load an alternative model like so:
 ```
-model = mask.get_model('unet','LTRCLobes')
-segmentation = mask.apply(input_image, model)
+inferer = LMInferer(modelname="R231CovidWeb")
 ```
 
-To use the model fusing capability for LTRCLobes_R231 use:
+To use the model fusing capability for (e.g. LTRCLobes_R231) use:
 ```
-segmentation = mask.apply_fused(input_image)
+inferer = LMInferer(modelname='LTRCLobes', fillmodel='R231')
 ```
 
 #### Numpy array support
 As of version 0.2.9, numpy arrays are supported as input volumes. This mode assumes the input numpy array has the following format for each axis:
 * first axis containing slices
 * second axis with chest to back
-* third axis with right to left 
+* third axis with right to left
 
 ## Limitations
-The model works on full slices only. The slice to process has to show the full lung and the lung has to be surrounded by tissue in order to get segmented. However, the model is quite stable to cases with a cropped field of view as long as the lung is surrounded by tissue. 
+The model works on full slices only. The slice to process has to show the full lung and the lung has to be surrounded by tissue in order to get segmented. However, the model is quite stable to cases with a cropped field of view as long as the lung is surrounded by tissue.
 
 ## COVID-19 Web
 ```
 lungmask INPUT OUTPUT --modelname R231CovidWeb
 ```
 The regular U-net(R231) model works very well for COVID-19 CT scans. However, collections of slices and case reports from the web are often cropped, annotated or encoded in regular image formats so that the original hounsfield unit (HU) values can only be estimated. The training data of the U-net(R231CovidWeb) model was augmented with COVID-19 slices that were mapped back from regular imaging formats to HU. The data was collected and prepared by MedSeg (http://medicalsegmentation.com/covid19/). While the regular U-net(R231) showed very good results for these images there may be cases for which this model will yield slighty improved segmentations. Note that you have to map images back to HU when using images from the web. This [blog post](https://medium.com/@hbjenssen/covid-19-radiology-data-collection-and-preparation-for-artificial-intelligence-4ecece97bb5b) describes how you can do that. Alternatively you can set the ```--noHU``` tag.
 ![alt text](figures/example_covid.jpg "COVID examples")
```

### Comparing `lungmask-0.2.13/lungmask/__main__.py` & `lungmask-0.2.14/lungmask/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,136 @@
-import sys
 import argparse
 import logging
-from lungmask import mask
-from lungmask import utils
 import os
-import SimpleITK as sitk
-import pkg_resources
+import sys
+
 import numpy as np
+import pkg_resources  # type: ignore
+import SimpleITK as sitk
+
+from lungmask import mask, utils
 
 
 def path(string):
     if os.path.exists(string):
         return string
     else:
-        sys.exit(f'File not found: {string}')
+        sys.exit(f"File not found: {string}")
 
 
 def main():
     version = pkg_resources.require("lungmask")[0].version
-    
-    parser = argparse.ArgumentParser()
-    parser.add_argument('input', metavar='input', type=path, help='Path to the input image, can be a folder for dicoms')
-    parser.add_argument('output', metavar='output', type=str, help='Filepath for output lungmask')
-    parser.add_argument('--modeltype', help='Default: unet', type=str, choices=['unet'], default='unet')
-    parser.add_argument('--modelname', help="spcifies the trained model, Default: R231", type=str, choices=['R231','LTRCLobes','LTRCLobes_R231','R231CovidWeb'], default='R231')
-    parser.add_argument('--modelpath', help="spcifies the path to the trained model", default=None)
-    parser.add_argument('--classes', help="spcifies the number of output classes of the model", default=3)
-    parser.add_argument('--cpu', help="Force using the CPU even when a GPU is available, will override batchsize to 1", action='store_true')
-    parser.add_argument('--nopostprocess', help="Deactivates postprocessing (removal of unconnected components and hole filling", action='store_true')
-    parser.add_argument('--noHU', help="For processing of images that are not encoded in hounsfield units (HU). E.g. png or jpg images from the web. Be aware, results may be substantially worse on these images", action='store_true')
-    parser.add_argument('--batchsize', type=int, help="Number of slices processed simultaneously. Lower number requires less memory but may be slower.", default=20)
-    parser.add_argument('--version', help="Shows the current version of lungmask", action='version', version=version)
+
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter
+    )
+    parser.add_argument(
+        "input",
+        metavar="input",
+        type=path,
+        help="Path to the input image, can be a folder for dicoms",
+    )
+    parser.add_argument(
+        "output", metavar="output", type=str, help="Filepath for output lungmask"
+    )
+    parser.add_argument(
+        "--modeltype", help="Default: unet", type=str, choices=["unet"], default="unet"
+    )
+    parser.add_argument(
+        "--modelname",
+        help="spcifies the trained model, Default: R231",
+        type=str,
+        choices=["R231", "LTRCLobes", "LTRCLobes_R231", "R231CovidWeb"],
+        default="R231",
+    )
+    parser.add_argument(
+        "--modelpath", help="spcifies the path to the trained model", default=None
+    )
+    parser.add_argument(
+        "--classes",
+        help="spcifies the number of output classes of the model",
+        default=3,
+    )
+    parser.add_argument(
+        "--cpu",
+        help="Force using the CPU even when a GPU is available, will override batchsize to 1",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--nopostprocess",
+        help="Deactivates postprocessing (removal of unconnected components and hole filling)",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--noHU",
+        help="For processing of images that are not encoded in hounsfield units (HU). E.g. png or jpg images from the web. Be aware, results may be substantially worse on these images",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--batchsize",
+        type=int,
+        help="Number of slices processed simultaneously. Lower number requires less memory but may be slower.",
+        default=20,
+    )
+    parser.add_argument(
+        "--noprogress",
+        action="store_true",
+        help="If set, no tqdm progress bar will be shown",
+    )
+    parser.add_argument(
+        "--version",
+        help="Shows the current version of lungmask",
+        action="version",
+        version=version,
+    )
 
     argsin = sys.argv[1:]
     args = parser.parse_args(argsin)
-    
+
     batchsize = args.batchsize
     if args.cpu:
         batchsize = 1
 
-    logging.info(f'Load model')
-    
-    input_image = utils.get_input_image(args.input)
-    logging.info(f'Infer lungmask')
-    if args.modelname == 'LTRCLobes_R231':
-        assert args.modelpath is None, "Modelpath can not be specified for LTRCLobes_R231 mode"
-        result = mask.apply_fused(input_image, force_cpu=args.cpu, batch_size=batchsize, volume_postprocessing=not(args.nopostprocess), noHU=args.noHU)
+    logging.info("Load model")
+
+    input_image = utils.load_input_image(args.input, disable_tqdm=args.noprogress)
+    logging.info("Infer lungmask")
+    if args.modelname == "LTRCLobes_R231":
+        assert (
+            args.modelpath is None
+        ), "Modelpath can not be specified for LTRCLobes_R231 mode"
+        result = mask.apply_fused(
+            input_image,
+            force_cpu=args.cpu,
+            batch_size=batchsize,
+            volume_postprocessing=not (args.nopostprocess),
+            noHU=args.noHU,
+            tqdm_disable=args.noprogress,
+        )
     else:
-        model = mask.get_model(args.modeltype, args.modelname, args.modelpath, args.classes)
-        result = mask.apply(input_image, model, force_cpu=args.cpu, batch_size=batchsize, volume_postprocessing=not(args.nopostprocess), noHU=args.noHU)
-        
+        model = mask.get_model(args.modelname, args.modelpath, args.classes)
+        result = mask.apply(
+            input_image,
+            model,
+            force_cpu=args.cpu,
+            batch_size=batchsize,
+            volume_postprocessing=not (args.nopostprocess),
+            noHU=args.noHU,
+            tqdm_disable=args.noprogress,
+        )
+
     if args.noHU:
-        file_ending = args.output.split('.')[-1]
+        file_ending = args.output.split(".")[-1]
         print(file_ending)
-        if file_ending in ['jpg','jpeg','png']:
-            result = (result/(result.max())*255).astype(np.uint8)
+        if file_ending in ["jpg", "jpeg", "png"]:
+            result = (result / (result.max()) * 255).astype(np.uint8)
         result = result[0]
-             
-    result_out= sitk.GetImageFromArray(result)
+
+    result_out = sitk.GetImageFromArray(result)
     result_out.CopyInformation(input_image)
-    logging.info(f'Save result to: {args.output}')
-    sys.exit(sitk.WriteImage(result_out, args.output))
+    logging.info(f"Save result to: {args.output}")
+    sitk.WriteImage(result_out, args.output)
 
 
 if __name__ == "__main__":
-    print('called as script')
+    print("called as script")
     main()
```

### Comparing `lungmask-0.2.13/lungmask/resunet.py` & `lungmask-0.2.14/lungmask/resunet.py`

 * *Files identical despite different names*

### Comparing `lungmask-0.2.13/lungmask/utils.py` & `lungmask-0.2.14/lungmask/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,284 +1,368 @@
-import scipy.ndimage as ndimage
-import skimage.measure
-import numpy as np
-from torch.utils.data import Dataset
+import logging
 import os
 import sys
-import SimpleITK as sitk
-import pydicom as pyd
-import logging
-from tqdm import tqdm
+from typing import Tuple
+
 import fill_voids
+import numpy as np
+import pydicom as pyd
+import SimpleITK as sitk
+import skimage.measure
 import skimage.morphology
+from scipy import ndimage
+from torch.utils.data import Dataset
+from tqdm import tqdm
 
 
-def preprocess(img, label=None, resolution=[192, 192]):
+def preprocess(
+    img: np.ndarray, resolution: list = [192, 192]
+) -> Tuple[np.ndarray, np.ndarray]:
+    """Preprocesses the image by clipping, cropping and resizing. Clipping at -1024 and 600 HU, cropping to the body
+
+    Args:
+        img (np.ndarray): Image to be preprocessed
+        resolution (list, optional): Target size after preprocessing. Defaults to [192, 192].
+
+    Returns:
+        Tuple[np.ndarray, np.ndarray]: Preprocessed image and the cropping bounding box
+    """
     imgmtx = np.copy(img)
-    lblsmtx = np.copy(label)
-
-    imgmtx[imgmtx < -1024] = -1024
-    imgmtx[imgmtx > 600] = 600
+    imgmtx = np.clip(imgmtx, -1024, 600)
     cip_xnew = []
     cip_box = []
-    cip_mask = []
-    for i in range(imgmtx.shape[0]):
-        if label is None:
-            (im, m, box) = crop_and_resize(imgmtx[i, :, :], width=resolution[0], height=resolution[1])
-        else:
-            (im, m, box) = crop_and_resize(imgmtx[i, :, :], mask=lblsmtx[i, :, :], width=resolution[0],
-                                           height=resolution[1])
-            cip_mask.append(m)
+    for imslice in imgmtx:
+        im, box = crop_and_resize(imslice, width=resolution[0], height=resolution[1])
         cip_xnew.append(im)
         cip_box.append(box)
-    if label is None:
-        return np.asarray(cip_xnew), cip_box
-    else:
-        return np.asarray(cip_xnew), cip_box, np.asarray(cip_mask)
+    return np.asarray(cip_xnew), cip_box
 
 
-def simple_bodymask(img):
+def simple_bodymask(img: np.ndarray) -> np.ndarray:
+    """Computes a simple bodymask by thresholding the image at -500 HU and then filling holes and removing small objects
+
+    Args:
+        img (np.ndarray): CT image (single slice) in HU
+
+    Returns:
+        np.ndarray: Binary mask of the body
+    """
+
+    # Here are some heuristics to get a body mask
     maskthreshold = -500
     oshape = img.shape
-    img = ndimage.zoom(img, 128/np.asarray(img.shape), order=0)
+    img = ndimage.zoom(img, 128 / np.asarray(img.shape), order=0)
     bodymask = img > maskthreshold
     bodymask = ndimage.binary_closing(bodymask)
-    bodymask = ndimage.binary_fill_holes(bodymask, structure=np.ones((3, 3))).astype(int)
+    bodymask = ndimage.binary_fill_holes(bodymask, structure=np.ones((3, 3))).astype(
+        int
+    )
     bodymask = ndimage.binary_erosion(bodymask, iterations=2)
     bodymask = skimage.measure.label(bodymask.astype(int), connectivity=1)
     regions = skimage.measure.regionprops(bodymask.astype(int))
     if len(regions) > 0:
         max_region = np.argmax(list(map(lambda x: x.area, regions))) + 1
         bodymask = bodymask == max_region
         bodymask = ndimage.binary_dilation(bodymask, iterations=2)
-    real_scaling = np.asarray(oshape)/128
+    real_scaling = np.asarray(oshape) / 128
     return ndimage.zoom(bodymask, real_scaling, order=0)
 
 
-def crop_and_resize(img, mask=None, width=192, height=192):
+def crop_and_resize(
+    img: np.ndarray, width: int = 192, height: int = 192
+) -> Tuple[np.ndarray, np.ndarray]:
+    """Crops the image to the body and resizes it to the specified size
+
+    Args:
+        img (np.ndarray): Image to be cropped and resized
+        width (int, optional): Target width to be resized to. Defaults to 192.
+        height (int, optional): Target height to be resized to. Defaults to 192.
+
+    Returns:
+        Tuple[np.ndarray, np.ndarray]: resized image and the cropping bounding box
+    """
     bmask = simple_bodymask(img)
     # img[bmask==0] = -1024 # this line removes background outside of the lung.
     # However, it has been shown problematic with narrow circular field of views that touch the lung.
     # Possibly doing more harm than help
     reg = skimage.measure.regionprops(skimage.measure.label(bmask))
     if len(reg) > 0:
         bbox = np.asarray(reg[0].bbox)
     else:
         bbox = (0, 0, bmask.shape[0], bmask.shape[1])
-    img = img[bbox[0]:bbox[2], bbox[1]:bbox[3]]
-    img = ndimage.zoom(img, np.asarray([width, height]) / np.asarray(img.shape), order=1)
-    if not mask is None:
-        mask = mask[bbox[0]:bbox[2], bbox[1]:bbox[3]]
-        mask = ndimage.zoom(mask, np.asarray([width, height]) / np.asarray(mask.shape), order=0)
-        # mask = ndimage.binary_closing(mask,iterations=5)
-    return img, mask, bbox
-
-
-## For some reasons skimage.transform leads to edgy mask borders compared to ndimage.zoom
-# def reshape_mask(mask, tbox, origsize):
-#     res = np.ones(origsize) * 0
-#     resize = [tbox[2] - tbox[0], tbox[3] - tbox[1]]
-#     imgres = skimage.transform.resize(mask, resize, order=0, mode='constant', cval=0, anti_aliasing=False, preserve_range=True)
-#     res[tbox[0]:tbox[2], tbox[1]:tbox[3]] = imgres
-#     return res
-
-
-def reshape_mask(mask, tbox, origsize):
+    img = img[bbox[0] : bbox[2], bbox[1] : bbox[3]]
+    img = ndimage.zoom(
+        img, np.asarray([width, height]) / np.asarray(img.shape), order=1
+    )
+    return img, bbox
+
+
+def reshape_mask(mask: np.ndarray, tbox: np.ndarray, origsize: tuple) -> np.ndarray:
+    """Reshapes the mask to the original size given bounding box and original size
+
+    Args:
+        mask (np.ndarray): Mask to be resampled (nearest neighbor)
+        tbox (np.ndarray): Bounding box in original image covering field of view of the mask
+        origsize (tuple): Original images size
+
+    Returns:
+        np.ndarray: Resampled mask in original image space
+    """
     res = np.ones(origsize) * 0
     resize = [tbox[2] - tbox[0], tbox[3] - tbox[1]]
     imgres = ndimage.zoom(mask, resize / np.asarray(mask.shape), order=0)
-    res[tbox[0]:tbox[2], tbox[1]:tbox[3]] = imgres
+    res[tbox[0] : tbox[2], tbox[1] : tbox[3]] = imgres
     return res
 
 
-class LungLabelsDS_inf(Dataset):
-    def __init__(self, ds):
-        self.dataset = ds
-
-    def __len__(self):
-        return len(self.dataset)
-
-    def __getitem__(self, idx):
-        return self.dataset[idx, None, :, :].astype(np.float32)
-
-
-def read_dicoms(path, primary=True, original=True):
+def read_dicoms(path, primary=True, original=True, disable_tqdm=False):
     allfnames = []
     for dir, _, fnames in os.walk(path):
         [allfnames.append(os.path.join(dir, fname)) for fname in fnames]
 
     dcm_header_info = []
-    dcm_parameters = []
-    unique_set = []  # need this because too often there are duplicates of dicom files with different names
+    unique_set = (
+        []
+    )  # need this because too often there are duplicates of dicom files with different names
     i = 0
-    for fname in tqdm(allfnames):
+    for fname in tqdm(allfnames, disable=disable_tqdm):
         filename_ = os.path.splitext(os.path.split(fname)[1])
         i += 1
-        if filename_[0] != 'DICOMDIR':
+        if filename_[0] != "DICOMDIR":
             try:
-                dicom_header = pyd.dcmread(fname, defer_size=100, stop_before_pixels=True, force=True)
+                dicom_header = pyd.dcmread(
+                    fname, defer_size=100, stop_before_pixels=True, force=True
+                )
                 if dicom_header is not None:
-                    if 'ImageType' in dicom_header:
+                    if "ImageType" in dicom_header:
                         if primary:
-                            is_primary = all([x in dicom_header.ImageType for x in ['PRIMARY']])
+                            is_primary = all(
+                                [x in dicom_header.ImageType for x in ["PRIMARY"]]
+                            )
                         else:
                             is_primary = True
 
                         if original:
-                            is_original = all([x in dicom_header.ImageType for x in ['ORIGINAL']])
+                            is_original = all(
+                                [x in dicom_header.ImageType for x in ["ORIGINAL"]]
+                            )
                         else:
                             is_original = True
 
-                        # if 'ConvolutionKernel' in dicom_header:
-                        #     ck = dicom_header.ConvolutionKernel
-                        # else:
-                        #     ck = 'unknown'
-                        if is_primary and is_original and 'LOCALIZER' not in dicom_header.ImageType:
-                            h_info_wo_name = [dicom_header.StudyInstanceUID, dicom_header.SeriesInstanceUID,
-                                              dicom_header.ImagePositionPatient]
-                            h_info = [dicom_header.StudyInstanceUID, dicom_header.SeriesInstanceUID, fname,
-                                      dicom_header.ImagePositionPatient]
+                        if (
+                            is_primary
+                            and is_original
+                            and "LOCALIZER" not in dicom_header.ImageType
+                        ):
+                            h_info_wo_name = [
+                                dicom_header.StudyInstanceUID,
+                                dicom_header.SeriesInstanceUID,
+                                dicom_header.ImagePositionPatient,
+                            ]
+                            h_info = [
+                                dicom_header.StudyInstanceUID,
+                                dicom_header.SeriesInstanceUID,
+                                fname,
+                                dicom_header.ImagePositionPatient,
+                            ]
                             if h_info_wo_name not in unique_set:
                                 unique_set.append(h_info_wo_name)
                                 dcm_header_info.append(h_info)
-                                # kvp = None
-                                # if 'KVP' in dicom_header:
-                                #     kvp = dicom_header.KVP
-                                # dcm_parameters.append([ck, kvp,dicom_header.SliceThickness])
-            except:
-                logging.error("Unexpected error:", sys.exc_info()[0])
+
+            except Exception as e:
+                logging.error("Unexpected error:", e)
                 logging.warning("Doesn't seem to be DICOM, will be skipped: ", fname)
 
     conc = [x[1] for x in dcm_header_info]
     sidx = np.argsort(conc)
     conc = np.asarray(conc)[sidx]
     dcm_header_info = np.asarray(dcm_header_info, dtype=object)[sidx]
-    # dcm_parameters = np.asarray(dcm_parameters)[sidx]
     vol_unique = np.unique(conc, return_index=1, return_inverse=1)  # unique volumes
     n_vol = len(vol_unique[1])
     if n_vol == 1:
-        logging.info('There is ' + str(n_vol) + ' volume in the study')
+        logging.info("There is " + str(n_vol) + " volume in the study")
     else:
-        logging.info('There are ' + str(n_vol) + ' volumes in the study')
+        logging.info("There are " + str(n_vol) + " volumes in the study")
 
     relevant_series = []
     relevant_volumes = []
 
     for i in range(len(vol_unique[1])):
         curr_vol = i
         info_idxs = np.where(vol_unique[2] == curr_vol)[0]
         vol_files = dcm_header_info[info_idxs, 2]
-        positions = np.asarray([np.asarray(x[2]) for x in dcm_header_info[info_idxs, 3]])
+        positions = np.asarray(
+            [np.asarray(x[2]) for x in dcm_header_info[info_idxs, 3]]
+        )
         slicesort_idx = np.argsort(positions)
         vol_files = vol_files[slicesort_idx]
         relevant_series.append(vol_files)
         reader = sitk.ImageSeriesReader()
         reader.SetFileNames(vol_files)
         vol = reader.Execute()
         relevant_volumes.append(vol)
 
     return relevant_volumes
 
 
-def get_input_image(path):
+def load_input_image(path: str, disable_tqdm=False) -> sitk.Image:
+    """Loads image, if path points to a file, file will be loaded. If path points ot a folder, a DICOM series will be loaded. If multiple series are present, the largest series (higher number of slices) will be loaded.
+
+    Args:
+        path (str): File or folderpath to be loaded. If folder, DICOM series is expected
+        disable_tqdm (bool, optional): Disable tqdm progress bar. Defaults to False.
+
+    Returns:
+        sitk.Image: Loaded image
+    """
     if os.path.isfile(path):
-        logging.info(f'Read input: {path}')
+        logging.info(f"Read input: {path}")
         input_image = sitk.ReadImage(path)
     else:
-        logging.info(f'Looking for dicoms in {path}')
-        dicom_vols = read_dicoms(path, original=False, primary=False)
+        logging.info(f"Looking for dicoms in {path}")
+        dicom_vols = read_dicoms(
+            path, original=False, primary=False, disable_tqdm=disable_tqdm
+        )
         if len(dicom_vols) < 1:
-            sys.exit('No dicoms found!')
+            sys.exit("No dicoms found!")
         if len(dicom_vols) > 1:
-            logging.warning("There are more than one volume in the path, will take the largest one")
-        input_image = dicom_vols[np.argmax([np.prod(v.GetSize()) for v in dicom_vols], axis=0)]
+            logging.warning(
+                "There are more than one volume in the path, will take the largest one"
+            )
+        input_image = dicom_vols[
+            np.argmax([np.prod(v.GetSize()) for v in dicom_vols], axis=0)
+        ]
     return input_image
 
 
-def postprocessing(label_image, spare=[]):
-    '''some post-processing mapping small label patches to the neighbout whith which they share the
-        largest border. All connected components smaller than min_area will be removed
-    '''
+def postprocessing(
+    label_image: np.ndarray,
+    spare: list = [],
+    disable_tqdm: bool = False,
+    skip_below: int = 3,
+) -> np.ndarray:
+    """some post-processing mapping small label patches to the neighbout whith which they share the
+        largest border. Only largest connected components (CC) for each label will be kept. If a label is member of the spare list it will be mapped to neighboring labels and not present in the final labelling.
+
+    Args:
+        label_image (np.ndarray): Label image (int) to be processed
+        spare (list, optional): Labels that are used for mapping to neighbors but not considered for final labelling. This is used for label fusion with a filling model. Defaults to [].
+        disable_tqdm (bool, optional): If true, tqdm will be diabled. Defaults to False.
+        skip_below (int, optional): If a CC is smaller than this value. It will not be merged but removed. This is for performance optimization.
+
+    Returns:
+        np.ndarray: Postprocessed volume
+    """
 
-    # merge small components to neighbours
+    # CC analysis
     regionmask = skimage.measure.label(label_image)
     origlabels = np.unique(label_image)
-    origlabels_maxsub = np.zeros((max(origlabels) + 1,), dtype=np.uint32)  # will hold the largest component for a label
+    origlabels_maxsub = np.zeros(
+        (max(origlabels) + 1,), dtype=np.uint32
+    )  # will hold the largest component for a label
     regions = skimage.measure.regionprops(regionmask, label_image)
     regions.sort(key=lambda x: x.area)
     regionlabels = [x.label for x in regions]
 
     # will hold mapping from regionlabels to original labels
     region_to_lobemap = np.zeros((len(regionlabels) + 1,), dtype=np.uint8)
     for r in regions:
         r_max_intensity = int(r.max_intensity)
         if r.area > origlabels_maxsub[r_max_intensity]:
             origlabels_maxsub[r_max_intensity] = r.area
             region_to_lobemap[r.label] = r_max_intensity
 
-    for r in tqdm(regions):
+    for r in tqdm(regions, disable=disable_tqdm):
         r_max_intensity = int(r.max_intensity)
-        if (r.area < origlabels_maxsub[r_max_intensity] or r_max_intensity in spare) and r.area>2: # area>2 improves runtime because small areas 1 and 2 voxel will be ignored
+        if (
+            r.area < origlabels_maxsub[r_max_intensity] or r_max_intensity in spare
+        ) and r.area >= skip_below:  # area>2 improves runtime because small areas 1 and 2 voxel will be ignored
             bb = bbox_3D(regionmask == r.label)
-            sub = regionmask[bb[0]:bb[1], bb[2]:bb[3], bb[4]:bb[5]]
+            sub = regionmask[bb[0] : bb[1], bb[2] : bb[3], bb[4] : bb[5]]
             dil = ndimage.binary_dilation(sub == r.label)
             neighbours, counts = np.unique(sub[dil], return_counts=True)
             mapto = r.label
             maxmap = 0
             myarea = 0
             for ix, n in enumerate(neighbours):
                 if n != 0 and n != r.label and counts[ix] > maxmap and n not in spare:
                     maxmap = counts[ix]
                     mapto = n
                     myarea = r.area
             regionmask[regionmask == r.label] = mapto
+
             # print(str(region_to_lobemap[r.label]) + ' -> ' + str(region_to_lobemap[mapto])) # for debugging
-            if regions[regionlabels.index(mapto)].area == origlabels_maxsub[
-                int(regions[regionlabels.index(mapto)].max_intensity)]:
-                origlabels_maxsub[int(regions[regionlabels.index(mapto)].max_intensity)] += myarea
-            regions[regionlabels.index(mapto)].__dict__['_cache']['area'] += myarea
+            if (
+                regions[regionlabels.index(mapto)].area
+                == origlabels_maxsub[
+                    int(regions[regionlabels.index(mapto)].max_intensity)
+                ]
+            ):
+                origlabels_maxsub[
+                    int(regions[regionlabels.index(mapto)].max_intensity)
+                ] += myarea
+            regions[regionlabels.index(mapto)].__dict__["_cache"]["area"] += myarea
 
     outmask_mapped = region_to_lobemap[regionmask]
     outmask_mapped[np.isin(outmask_mapped, spare)] = 0
 
     if outmask_mapped.shape[0] == 1:
-        # holefiller = lambda x: ndimage.morphology.binary_fill_holes(x[0])[None, :, :] # This is bad for slices that show the liver
-        holefiller = lambda x: skimage.morphology.area_closing(x[0].astype(int), area_threshold=64)[None, :, :] == 1
+        holefiller = (
+            lambda x: skimage.morphology.area_closing(
+                x[0].astype(int), area_threshold=64
+            )[None, :, :]
+            == 1
+        )
     else:
         holefiller = fill_voids.fill
 
     outmask = np.zeros(outmask_mapped.shape, dtype=np.uint8)
     for i in np.unique(outmask_mapped)[1:]:
         outmask[holefiller(keep_largest_connected_component(outmask_mapped == i))] = i
 
     return outmask
 
 
 def bbox_3D(labelmap, margin=2):
-    shape = labelmap.shape
-    r = np.any(labelmap, axis=(1, 2))
-    c = np.any(labelmap, axis=(0, 2))
-    z = np.any(labelmap, axis=(0, 1))
-
-    rmin, rmax = np.where(r)[0][[0, -1]]
-    rmin -= margin if rmin >= margin else rmin
-    rmax += margin if rmax <= shape[0] - margin else rmax
-    cmin, cmax = np.where(c)[0][[0, -1]]
-    cmin -= margin if cmin >= margin else cmin
-    cmax += margin if cmax <= shape[1] - margin else cmax
-    zmin, zmax = np.where(z)[0][[0, -1]]
-    zmin -= margin if zmin >= margin else zmin
-    zmax += margin if zmax <= shape[2] - margin else zmax
-    
-    if rmax-rmin == 0:
-        rmax = rmin+1
-
-    return np.asarray([rmin, rmax, cmin, cmax, zmin, zmax])
+    """Compute bounding box of a 3D labelmap.
 
-
-def keep_largest_connected_component(mask):
+    Args:
+        labelmap (np.ndarray): Input labelmap
+        margin (int, optional): Margin to add to the bounding box. Defaults to 2.
+
+    Returns:
+        np.ndarray: Bounding box as [zmin, zmax, ymin, ymax, xmin, xmax]
+    """
+    shape = labelmap.shape
+    dimensions = np.arange(len(shape))
+    bmins = []
+    bmaxs = []
+    margin = [margin] * len(dimensions)
+    for dim, dim_margin, dim_shape in zip(dimensions, margin, shape):
+        margin_label = np.any(labelmap, axis=tuple(dimensions[dimensions != dim]))
+        bmin, bmax = np.where(margin_label)[0][[0, -1]]
+        bmin -= dim_margin
+        bmax += dim_margin + 1
+        bmin = max(bmin, 0)
+        bmax = min(bmax, dim_shape)
+        bmins.append(bmin)
+        bmaxs.append(bmax)
+
+    bbox = np.array(list(zip(bmins, bmaxs))).flatten()
+    return bbox
+
+
+def keep_largest_connected_component(mask: np.ndarray) -> np.ndarray:
+    """Keeps largest connected component (CC)
+
+    Args:
+        mask (np.ndarray): Input label map
+
+    Returns:
+        np.ndarray: Binary label map with largest CC
+    """
     mask = skimage.measure.label(mask)
     regions = skimage.measure.regionprops(mask)
     resizes = np.asarray([x.area for x in regions])
     max_region = np.argsort(resizes)[-1] + 1
     mask = mask == max_region
     return mask
```

### Comparing `lungmask-0.2.13/lungmask.egg-info/PKG-INFO` & `lungmask-0.2.14/lungmask.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: lungmask
-Version: 0.2.13
+Version: 0.2.14
 Summary: Package for automated lung segmentation in CT
 Home-page: https://github.com/JoHof/lungmask
 Author: Johannes Hofmanninger
-Author-email: johannes.hofmanninger@meduniwien.ac.at
+Author-email: johannes.hofmanninger@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Automated lung segmentation in CT under presence of severe pathologies
 
 This package provides trained U-net models for lung segmentation. For now, four models are available:
 
 - U-net(R231): This model was trained on a large and diverse dataset that covers a wide range of visual variabiliy. The model performs segmentation on individual slices, extracts right-left lung seperately includes airpockets, tumors and effusions. The trachea will not be included in the lung segmentation. https://doi.org/10.1186/s41747-020-00173-2
 
-- U-net(LTRCLobes): This model was trained on a subset of the [LTRC](https://ltrcpublic.com) dataset. The model performs segmentation of individual lung-lobes but yields limited performance when dense pathologies are present or when fissures are not visible at every slice. 
+- U-net(LTRCLobes): This model was trained on a subset of the [LTRC](https://ltrcpublic.com) dataset. The model performs segmentation of individual lung-lobes but yields limited performance when dense pathologies are present or when fissures are not visible at every slice.
 
 - U-net(LTRCLobes_R231): This will run the R231 and LTRCLobes model and fuse the results. False negatives from LTRCLobes will be filled by R231 predictions and mapped to a neighbor label. False positives from LTRCLobes will be removed. The fusing process is computationally intensive and can, depdending on the data and results, take up to several minutes per volume.
 
 - [U-net(R231CovidWeb)](#COVID-19-Web)
 
 
 **Examples of the two models applied**. **Left:** U-net(R231), will distinguish between left and right lung and include very dense areas such as effusions (third row), tumor or severe fibrosis (fourth row) . **Right:** U-net(LTRLobes), will distinguish between lung lobes but will not include very dense areas. **LTRCLobes_R231** will fuse LTRCLobes and R231 results. **R231CovidWeb** is trained with aditional COVID-19 data.
@@ -69,41 +69,42 @@
 ```
 lungmask -h
 ```
 
 ### As a python module:
 
 ```
-from lungmask import mask
+from lungmask import LMInferer
 import SimpleITK as sitk
 
+inferer = LMInferer()
+
 input_image = sitk.ReadImage(INPUT)
-segmentation = mask.apply(input_image)  # default model is U-net(R231)
+segmentation = inferer.apply(input_image)  # default model is U-net(R231)
 ```
 input_image has to be a SimpleITK object.
 
 Load an alternative model like so:
 ```
-model = mask.get_model('unet','LTRCLobes')
-segmentation = mask.apply(input_image, model)
+inferer = LMInferer(modelname="R231CovidWeb")
 ```
 
-To use the model fusing capability for LTRCLobes_R231 use:
+To use the model fusing capability for (e.g. LTRCLobes_R231) use:
 ```
-segmentation = mask.apply_fused(input_image)
+inferer = LMInferer(modelname='LTRCLobes', fillmodel='R231')
 ```
 
 #### Numpy array support
 As of version 0.2.9, numpy arrays are supported as input volumes. This mode assumes the input numpy array has the following format for each axis:
 * first axis containing slices
 * second axis with chest to back
-* third axis with right to left 
+* third axis with right to left
 
 ## Limitations
-The model works on full slices only. The slice to process has to show the full lung and the lung has to be surrounded by tissue in order to get segmented. However, the model is quite stable to cases with a cropped field of view as long as the lung is surrounded by tissue. 
+The model works on full slices only. The slice to process has to show the full lung and the lung has to be surrounded by tissue in order to get segmented. However, the model is quite stable to cases with a cropped field of view as long as the lung is surrounded by tissue.
 
 ## COVID-19 Web
 ```
 lungmask INPUT OUTPUT --modelname R231CovidWeb
 ```
 The regular U-net(R231) model works very well for COVID-19 CT scans. However, collections of slices and case reports from the web are often cropped, annotated or encoded in regular image formats so that the original hounsfield unit (HU) values can only be estimated. The training data of the U-net(R231CovidWeb) model was augmented with COVID-19 slices that were mapped back from regular imaging formats to HU. The data was collected and prepared by MedSeg (http://medicalsegmentation.com/covid19/). While the regular U-net(R231) showed very good results for these images there may be cases for which this model will yield slighty improved segmentations. Note that you have to map images back to HU when using images from the web. This [blog post](https://medium.com/@hbjenssen/covid-19-radiology-data-collection-and-preparation-for-artificial-intelligence-4ecece97bb5b) describes how you can do that. Alternatively you can set the ```--noHU``` tag.
 ![alt text](figures/example_covid.jpg "COVID examples")
```

### Comparing `lungmask-0.2.13/setup.py` & `lungmask-0.2.14/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 import setuptools
 
-with open("README.md", "r", encoding='utf-8') as fh:
+with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lungmask",
-    version="0.2.13",
+    version="0.2.14",
     author="Johannes Hofmanninger",
-    author_email="johannes.hofmanninger@meduniwien.ac.at",
+    author_email="johannes.hofmanninger@gmail.com",
     description="Package for automated lung segmentation in CT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JoHof/lungmask",
     packages=setuptools.find_packages(),
-    entry_points={
-        'console_scripts': [
-            'lungmask = lungmask.__main__:main'
-        ]
-    },
+    entry_points={"console_scripts": ["lungmask = lungmask.__main__:main"]},
     install_requires=[
-        'pydicom',
-        'numpy',
-        'torch',
-        'scipy',
-        'SimpleITK',
-        'tqdm',
-        'scikit-image',
-        'fill_voids'
+        "pydicom",
+        "numpy",
+        "torch",
+        "scipy",
+        "SimpleITK",
+        "tqdm",
+        "scikit-image",
+        "fill_voids",
+        "more-itertools",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Operating System :: OS Independent"
+        "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires=">=3.6",
 )
```

