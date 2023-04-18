# Comparing `tmp/i3dFeatureExtraction-0.2.7.tar.gz` & `tmp/i3dFeatureExtraction-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i3dFeatureExtraction-0.2.7.tar", last modified: Tue Apr 18 07:33:34 2023, max compression
+gzip compressed data, was "i3dFeatureExtraction-0.2.8.tar", last modified: Tue Apr 18 07:44:31 2023, max compression
```

## Comparing `i3dFeatureExtraction-0.2.7.tar` & `i3dFeatureExtraction-0.2.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 07:33:34.828910 i3dFeatureExtraction-0.2.7/
--rw-rw-rw-   0        0        0     1355 2023-04-17 09:06:40.000000 i3dFeatureExtraction-0.2.7/LICENSE.txt
--rw-rw-rw-   0        0        0     3748 2023-04-18 07:33:34.828910 i3dFeatureExtraction-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     3048 2023-04-18 07:16:31.000000 i3dFeatureExtraction-0.2.7/README.md
--rw-rw-rw-   0        0        0     3289 2023-04-18 07:33:19.000000 i3dFeatureExtraction-0.2.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-18 07:33:34.791058 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/
--rw-rw-rw-   0        0        0     4088 2023-04-18 02:41:47.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/__init__.py
--rw-rw-rw-   0        0        0    10425 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/extract_features.py
--rw-rw-rw-   0        0        0     2294 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/extract_features_org.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:33:34.813274 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/models/
--rw-rw-rw-   0        0        0        0 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/models/__init__.py
--rw-rw-rw-   0        0        0     2235 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/models/model_builder_video.py
--rw-rw-rw-   0        0        0     3803 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/models/nonlocal_helper.py
--rw-rw-rw-   0        0        0     7644 2023-03-27 13:19:26.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/models/resnet.py
--rw-rw-rw-   0        0        0     3992 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/models/resnet_helper.py
--rw-rw-rw-   0        0        0     3214 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/models/resnet_video_org.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:33:34.828910 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/utils/
--rw-rw-rw-   0        0        0        0 2023-04-18 02:56:31.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/utils/__init__.py
--rw-rw-rw-   0        0        0     2716 2023-04-18 03:18:53.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/utils/convert_weights.py
--rw-rw-rw-   0        0        0     3223 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/utils/pretrained_existed.py
-drwxrwxrwx   0        0        0        0 2023-04-18 07:33:34.813274 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction.egg-info/
--rw-rw-rw-   0        0        0     3748 2023-04-18 07:33:34.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      782 2023-04-18 07:33:34.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 07:33:34.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      677 2023-04-18 07:33:34.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-18 07:33:34.000000 i3dFeatureExtraction-0.2.7/i3dFeatureExtraction.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 07:33:34.828910 i3dFeatureExtraction-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-04-18 07:22:42.000000 i3dFeatureExtraction-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:44:31.082997 i3dFeatureExtraction-0.2.8/
+-rw-rw-rw-   0        0        0     1355 2023-04-17 09:06:40.000000 i3dFeatureExtraction-0.2.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     3797 2023-04-18 07:44:31.082997 i3dFeatureExtraction-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3048 2023-04-18 07:16:31.000000 i3dFeatureExtraction-0.2.8/README.md
+-rw-rw-rw-   0        0        0     3338 2023-04-18 07:44:02.000000 i3dFeatureExtraction-0.2.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-18 07:44:31.055423 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/
+-rw-rw-rw-   0        0        0     4088 2023-04-18 02:41:47.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/__init__.py
+-rw-rw-rw-   0        0        0    10425 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/extract_features.py
+-rw-rw-rw-   0        0        0     2294 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/extract_features_org.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:44:31.078998 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/
+-rw-rw-rw-   0        0        0        0 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/__init__.py
+-rw-rw-rw-   0        0        0     2235 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/model_builder_video.py
+-rw-rw-rw-   0        0        0     3803 2023-03-27 11:20:56.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/nonlocal_helper.py
+-rw-rw-rw-   0        0        0     7644 2023-03-27 13:19:26.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/resnet.py
+-rw-rw-rw-   0        0        0     3992 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/resnet_helper.py
+-rw-rw-rw-   0        0        0     3214 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/resnet_video_org.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:44:31.081996 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-18 02:56:31.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/utils/__init__.py
+-rw-rw-rw-   0        0        0     2716 2023-04-18 03:18:53.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/utils/convert_weights.py
+-rw-rw-rw-   0        0        0     3223 2023-04-18 02:50:01.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/utils/pretrained_existed.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:44:31.072842 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/
+-rw-rw-rw-   0        0        0     3797 2023-04-18 07:44:30.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      782 2023-04-18 07:44:30.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 07:44:30.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      677 2023-04-18 07:44:30.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-18 07:44:30.000000 i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 07:44:31.082997 i3dFeatureExtraction-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      745 2023-04-18 07:44:16.000000 i3dFeatureExtraction-0.2.8/setup.py
```

### Comparing `i3dFeatureExtraction-0.2.7/LICENSE.txt` & `i3dFeatureExtraction-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.7/PKG-INFO` & `i3dFeatureExtraction-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i3dFeatureExtraction
-Version: 0.2.7
+Version: 0.2.8
 Summary: This package helps extract i3D features with ResNet-50 backbone given a folder of videos
 Author: Hao Vy Phan
 Author-email: vyhao03@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
@@ -97,15 +97,15 @@
 
 --------------
 Structure
 --------------
 
 I am not good at drawing UML diagram but I hope this image helps illustrate the package's structure.
 
-.. image:: UML/i3dExtract.png
+.. image:: https://vyhaoromanletters.s3.us-east-2.amazonaws.com/i3dExtract.png
    :alt: i3dFeatureExtraction - UML Diagram
 
 Credits
 -----------
 
 This code is based on the following repositories:
```

### Comparing `i3dFeatureExtraction-0.2.7/README.md` & `i3dFeatureExtraction-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.7/README.rst` & `i3dFeatureExtraction-0.2.8/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 --------------
 Structure
 --------------
 
 I am not good at drawing UML diagram but I hope this image helps illustrate the package's structure.
 
-.. image:: UML/i3dExtract.png
+.. image:: https://vyhaoromanletters.s3.us-east-2.amazonaws.com/i3dExtract.png
    :alt: i3dFeatureExtraction - UML Diagram
 
 Credits
 -----------
 
 This code is based on the following repositories:
```

### Comparing `i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/__init__.py` & `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/__init__.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/extract_features.py` & `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/extract_features.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/extract_features_org.py` & `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/extract_features_org.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/models/model_builder_video.py` & `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/model_builder_video.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/models/nonlocal_helper.py` & `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/nonlocal_helper.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/models/resnet.py` & `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/resnet.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/models/resnet_helper.py` & `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/resnet_helper.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/models/resnet_video_org.py` & `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/models/resnet_video_org.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/utils/convert_weights.py` & `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/utils/convert_weights.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.7/i3dFeatureExtraction/utils/pretrained_existed.py` & `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction/utils/pretrained_existed.py`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.7/i3dFeatureExtraction.egg-info/PKG-INFO` & `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i3dFeatureExtraction
-Version: 0.2.7
+Version: 0.2.8
 Summary: This package helps extract i3D features with ResNet-50 backbone given a folder of videos
 Author: Hao Vy Phan
 Author-email: vyhao03@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
@@ -97,15 +97,15 @@
 
 --------------
 Structure
 --------------
 
 I am not good at drawing UML diagram but I hope this image helps illustrate the package's structure.
 
-.. image:: UML/i3dExtract.png
+.. image:: https://vyhaoromanletters.s3.us-east-2.amazonaws.com/i3dExtract.png
    :alt: i3dFeatureExtraction - UML Diagram
 
 Credits
 -----------
 
 This code is based on the following repositories:
```

### Comparing `i3dFeatureExtraction-0.2.7/i3dFeatureExtraction.egg-info/SOURCES.txt` & `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.7/i3dFeatureExtraction.egg-info/requires.txt` & `i3dFeatureExtraction-0.2.8/i3dFeatureExtraction.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `i3dFeatureExtraction-0.2.7/setup.py` & `i3dFeatureExtraction-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 DESCRIPTION = "This package helps extract i3D features with ResNet-50 backbone given a folder of videos"
 REQUIREMENTS = [i for i in open("requirements.txt").readlines()]
 setuptools.setup(
     name="i3dFeatureExtraction",
-    version="0.2.7",
+    version="0.2.8",
     author="Hao Vy Phan",
     author_email="vyhao03@gmail.com",
     description=DESCRIPTION,
     long_description = open('README.rst').read(),
     long_description_content_type='text/x-rst',
     python_requires='>=3.8',
     packages=setuptools.find_packages(),
```

