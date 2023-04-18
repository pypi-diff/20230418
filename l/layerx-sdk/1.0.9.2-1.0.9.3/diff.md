# Comparing `tmp/layerx-sdk-1.0.9.2.tar.gz` & `tmp/layerx-sdk-1.0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layerx-sdk-1.0.9.2.tar", last modified: Wed Mar 22 17:06:13 2023, max compression
+gzip compressed data, was "layerx-sdk-1.0.9.3.tar", last modified: Wed Mar 22 23:40:56 2023, max compression
```

## Comparing `layerx-sdk-1.0.9.2.tar` & `layerx-sdk-1.0.9.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 kelumvithana   (501) staff       (20)        0 2023-03-22 17:06:13.753862 layerx-sdk-1.0.9.2/
--rw-r--r--   0 kelumvithana   (501) staff       (20)     5550 2023-03-22 17:06:13.753678 layerx-sdk-1.0.9.2/PKG-INFO
--rw-r--r--   0 kelumvithana   (501) staff       (20)     5022 2022-11-21 13:34:57.000000 layerx-sdk-1.0.9.2/README.md
-drwxr-xr-x   0 kelumvithana   (501) staff       (20)        0 2023-03-22 17:06:13.738169 layerx-sdk-1.0.9.2/layerx/
--rw-r--r--   0 kelumvithana   (501) staff       (20)    38700 2023-03-22 16:49:23.000000 layerx-sdk-1.0.9.2/layerx/__init__.py
-drwxr-xr-x   0 kelumvithana   (501) staff       (20)        0 2023-03-22 17:06:13.748453 layerx-sdk-1.0.9.2/layerx/datalake/
--rw-r--r--   0 kelumvithana   (501) staff       (20)     7312 2023-03-22 16:55:48.000000 layerx-sdk-1.0.9.2/layerx/datalake/__init__.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)     8968 2023-03-20 13:20:53.000000 layerx-sdk-1.0.9.2/layerx/datalake/annotation.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)      686 2023-03-22 16:49:23.000000 layerx-sdk-1.0.9.2/layerx/datalake/constants.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)    15121 2023-03-20 13:20:53.000000 layerx-sdk-1.0.9.2/layerx/datalake/datalakeinterface.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)        0 2022-11-21 13:34:57.000000 layerx-sdk-1.0.9.2/layerx/datalake/dataset.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)     7648 2023-03-22 16:50:29.000000 layerx-sdk-1.0.9.2/layerx/datalake/file_upload.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)     1516 2023-03-20 13:20:53.000000 layerx-sdk-1.0.9.2/layerx/datalake/ground_truth.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)     1119 2023-03-20 13:20:53.000000 layerx-sdk-1.0.9.2/layerx/datalake/keys.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)     3514 2022-11-21 13:34:57.000000 layerx-sdk-1.0.9.2/layerx/datalake/label.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)      417 2022-11-21 13:34:57.000000 layerx-sdk-1.0.9.2/layerx/datalake/logger.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)      849 2023-03-20 13:20:53.000000 layerx-sdk-1.0.9.2/layerx/datalake/model_run.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)     1273 2023-02-01 12:14:07.000000 layerx-sdk-1.0.9.2/layerx/datalake/query.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)      924 2023-03-21 10:34:12.000000 layerx-sdk-1.0.9.2/layerx/datalake/s3_interface.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)     2936 2022-12-02 18:47:29.000000 layerx-sdk-1.0.9.2/layerx/datalake/s3_upload.py
-drwxr-xr-x   0 kelumvithana   (501) staff       (20)        0 2023-03-22 17:06:13.751188 layerx-sdk-1.0.9.2/layerx/dataset/
--rw-r--r--   0 kelumvithana   (501) staff       (20)     2544 2023-03-17 05:54:53.000000 layerx-sdk-1.0.9.2/layerx/dataset/__init__.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)     3142 2023-03-21 10:34:12.000000 layerx-sdk-1.0.9.2/layerx/dataset/dataset.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)     5402 2023-02-16 14:20:29.000000 layerx-sdk-1.0.9.2/layerx/dataset/datasetinterface.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)      417 2023-02-16 14:20:29.000000 layerx-sdk-1.0.9.2/layerx/dataset/logger.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)    15582 2023-03-20 13:20:53.000000 layerx-sdk-1.0.9.2/layerx/dataset/sync.py
-drwxr-xr-x   0 kelumvithana   (501) staff       (20)        0 2023-03-22 17:06:13.752689 layerx-sdk-1.0.9.2/layerx/studio/
--rw-r--r--   0 kelumvithana   (501) staff       (20)     2472 2023-03-22 16:49:23.000000 layerx-sdk-1.0.9.2/layerx/studio/__init__.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)      417 2023-01-27 14:48:40.000000 layerx-sdk-1.0.9.2/layerx/studio/logger.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)     2851 2023-03-22 16:49:23.000000 layerx-sdk-1.0.9.2/layerx/studio/project.py
--rw-r--r--   0 kelumvithana   (501) staff       (20)     4897 2023-02-01 12:14:07.000000 layerx-sdk-1.0.9.2/layerx/studio/studiointerface.py
-drwxr-xr-x   0 kelumvithana   (501) staff       (20)        0 2023-03-22 17:06:13.753444 layerx-sdk-1.0.9.2/layerx_sdk.egg-info/
--rw-r--r--   0 kelumvithana   (501) staff       (20)     5550 2023-03-22 17:06:13.000000 layerx-sdk-1.0.9.2/layerx_sdk.egg-info/PKG-INFO
--rw-r--r--   0 kelumvithana   (501) staff       (20)      854 2023-03-22 17:06:13.000000 layerx-sdk-1.0.9.2/layerx_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 kelumvithana   (501) staff       (20)        1 2023-03-22 17:06:13.000000 layerx-sdk-1.0.9.2/layerx_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 kelumvithana   (501) staff       (20)       28 2023-03-22 17:06:13.000000 layerx-sdk-1.0.9.2/layerx_sdk.egg-info/requires.txt
--rw-r--r--   0 kelumvithana   (501) staff       (20)        7 2023-03-22 17:06:13.000000 layerx-sdk-1.0.9.2/layerx_sdk.egg-info/top_level.txt
--rw-r--r--   0 kelumvithana   (501) staff       (20)       38 2023-03-22 17:06:13.753908 layerx-sdk-1.0.9.2/setup.cfg
--rw-r--r--   0 kelumvithana   (501) staff       (20)     1193 2023-03-22 16:51:00.000000 layerx-sdk-1.0.9.2/setup.py
+drwxr-xr-x   0 kelumvithana   (501) staff       (20)        0 2023-03-22 23:40:56.796836 layerx-sdk-1.0.9.3/
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     5550 2023-03-22 23:40:56.796695 layerx-sdk-1.0.9.3/PKG-INFO
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     5022 2022-11-21 13:34:57.000000 layerx-sdk-1.0.9.3/README.md
+drwxr-xr-x   0 kelumvithana   (501) staff       (20)        0 2023-03-22 23:40:56.786116 layerx-sdk-1.0.9.3/layerx/
+-rw-r--r--   0 kelumvithana   (501) staff       (20)    38700 2023-03-22 16:49:23.000000 layerx-sdk-1.0.9.3/layerx/__init__.py
+drwxr-xr-x   0 kelumvithana   (501) staff       (20)        0 2023-03-22 23:40:56.792148 layerx-sdk-1.0.9.3/layerx/datalake/
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     7321 2023-03-22 23:37:39.000000 layerx-sdk-1.0.9.3/layerx/datalake/__init__.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     8968 2023-03-20 13:20:53.000000 layerx-sdk-1.0.9.3/layerx/datalake/annotation.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)      686 2023-03-22 16:49:23.000000 layerx-sdk-1.0.9.3/layerx/datalake/constants.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)    15121 2023-03-20 13:20:53.000000 layerx-sdk-1.0.9.3/layerx/datalake/datalakeinterface.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)        0 2022-11-21 13:34:57.000000 layerx-sdk-1.0.9.3/layerx/datalake/dataset.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     7648 2023-03-22 16:50:29.000000 layerx-sdk-1.0.9.3/layerx/datalake/file_upload.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     1516 2023-03-20 13:20:53.000000 layerx-sdk-1.0.9.3/layerx/datalake/ground_truth.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     1119 2023-03-20 13:20:53.000000 layerx-sdk-1.0.9.3/layerx/datalake/keys.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     3514 2022-11-21 13:34:57.000000 layerx-sdk-1.0.9.3/layerx/datalake/label.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)      417 2022-11-21 13:34:57.000000 layerx-sdk-1.0.9.3/layerx/datalake/logger.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)      849 2023-03-20 13:20:53.000000 layerx-sdk-1.0.9.3/layerx/datalake/model_run.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     1273 2023-02-01 12:14:07.000000 layerx-sdk-1.0.9.3/layerx/datalake/query.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)      924 2023-03-21 10:34:12.000000 layerx-sdk-1.0.9.3/layerx/datalake/s3_interface.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     2936 2022-12-02 18:47:29.000000 layerx-sdk-1.0.9.3/layerx/datalake/s3_upload.py
+drwxr-xr-x   0 kelumvithana   (501) staff       (20)        0 2023-03-22 23:40:56.794380 layerx-sdk-1.0.9.3/layerx/dataset/
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     2544 2023-03-17 05:54:53.000000 layerx-sdk-1.0.9.3/layerx/dataset/__init__.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     3142 2023-03-21 10:34:12.000000 layerx-sdk-1.0.9.3/layerx/dataset/dataset.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     5402 2023-02-16 14:20:29.000000 layerx-sdk-1.0.9.3/layerx/dataset/datasetinterface.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)      417 2023-02-16 14:20:29.000000 layerx-sdk-1.0.9.3/layerx/dataset/logger.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)    15582 2023-03-20 13:20:53.000000 layerx-sdk-1.0.9.3/layerx/dataset/sync.py
+drwxr-xr-x   0 kelumvithana   (501) staff       (20)        0 2023-03-22 23:40:56.795559 layerx-sdk-1.0.9.3/layerx/studio/
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     2472 2023-03-22 16:49:23.000000 layerx-sdk-1.0.9.3/layerx/studio/__init__.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)      417 2023-01-27 14:48:40.000000 layerx-sdk-1.0.9.3/layerx/studio/logger.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     2851 2023-03-22 16:49:23.000000 layerx-sdk-1.0.9.3/layerx/studio/project.py
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     4897 2023-02-01 12:14:07.000000 layerx-sdk-1.0.9.3/layerx/studio/studiointerface.py
+drwxr-xr-x   0 kelumvithana   (501) staff       (20)        0 2023-03-22 23:40:56.796499 layerx-sdk-1.0.9.3/layerx_sdk.egg-info/
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     5550 2023-03-22 23:40:56.000000 layerx-sdk-1.0.9.3/layerx_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 kelumvithana   (501) staff       (20)      854 2023-03-22 23:40:56.000000 layerx-sdk-1.0.9.3/layerx_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 kelumvithana   (501) staff       (20)        1 2023-03-22 23:40:56.000000 layerx-sdk-1.0.9.3/layerx_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 kelumvithana   (501) staff       (20)       28 2023-03-22 23:40:56.000000 layerx-sdk-1.0.9.3/layerx_sdk.egg-info/requires.txt
+-rw-r--r--   0 kelumvithana   (501) staff       (20)        7 2023-03-22 23:40:56.000000 layerx-sdk-1.0.9.3/layerx_sdk.egg-info/top_level.txt
+-rw-r--r--   0 kelumvithana   (501) staff       (20)       38 2023-03-22 23:40:56.796872 layerx-sdk-1.0.9.3/setup.cfg
+-rw-r--r--   0 kelumvithana   (501) staff       (20)     1193 2023-03-22 23:39:34.000000 layerx-sdk-1.0.9.3/setup.py
```

### Comparing `layerx-sdk-1.0.9.2/PKG-INFO` & `layerx-sdk-1.0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layerx-sdk
-Version: 1.0.9.2
+Version: 1.0.9.3
 Summary: LayerX Python SDK
 Author: LayerX
 Author-email: <support@layerx.ai>
 Keywords: python,datalake,datasetsync,ai,annotation,layerx,machine learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `layerx-sdk-1.0.9.2/README.md` & `layerx-sdk-1.0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/__init__.py` & `layerx-sdk-1.0.9.3/layerx/__init__.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/datalake/__init__.py` & `layerx-sdk-1.0.9.3/layerx/datalake/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class DatalakeClient:
     """
     Python SDK of Datalake
     """
 
     def __init__(self, encoded_key_secret: str, layerx_url: str) -> None:
-        _datalake_url = f'{layerx_url}' #/datalake :3000
+        _datalake_url = f'{layerx_url}/datalake' #/datalake :3000
         self.datalake_interface = DatalakeInterface(encoded_key_secret, _datalake_url)
 
     def upload_annotation_from_cocojson(self, file_path: str):
         """
         available soon
         """
         datalake_logger.debug(f'file_name={file_path}')
```

### Comparing `layerx-sdk-1.0.9.2/layerx/datalake/annotation.py` & `layerx-sdk-1.0.9.3/layerx/datalake/annotation.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/datalake/constants.py` & `layerx-sdk-1.0.9.3/layerx/datalake/constants.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/datalake/datalakeinterface.py` & `layerx-sdk-1.0.9.3/layerx/datalake/datalakeinterface.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/datalake/file_upload.py` & `layerx-sdk-1.0.9.3/layerx/datalake/file_upload.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/datalake/ground_truth.py` & `layerx-sdk-1.0.9.3/layerx/datalake/ground_truth.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/datalake/keys.py` & `layerx-sdk-1.0.9.3/layerx/datalake/keys.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/datalake/label.py` & `layerx-sdk-1.0.9.3/layerx/datalake/label.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/datalake/model_run.py` & `layerx-sdk-1.0.9.3/layerx/datalake/model_run.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/datalake/query.py` & `layerx-sdk-1.0.9.3/layerx/datalake/query.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/datalake/s3_interface.py` & `layerx-sdk-1.0.9.3/layerx/datalake/s3_interface.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/datalake/s3_upload.py` & `layerx-sdk-1.0.9.3/layerx/datalake/s3_upload.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/dataset/__init__.py` & `layerx-sdk-1.0.9.3/layerx/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/dataset/dataset.py` & `layerx-sdk-1.0.9.3/layerx/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/dataset/datasetinterface.py` & `layerx-sdk-1.0.9.3/layerx/dataset/datasetinterface.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/dataset/sync.py` & `layerx-sdk-1.0.9.3/layerx/dataset/sync.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/studio/__init__.py` & `layerx-sdk-1.0.9.3/layerx/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/studio/project.py` & `layerx-sdk-1.0.9.3/layerx/studio/project.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx/studio/studiointerface.py` & `layerx-sdk-1.0.9.3/layerx/studio/studiointerface.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/layerx_sdk.egg-info/PKG-INFO` & `layerx-sdk-1.0.9.3/layerx_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layerx-sdk
-Version: 1.0.9.2
+Version: 1.0.9.3
 Summary: LayerX Python SDK
 Author: LayerX
 Author-email: <support@layerx.ai>
 Keywords: python,datalake,datasetsync,ai,annotation,layerx,machine learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `layerx-sdk-1.0.9.2/layerx_sdk.egg-info/SOURCES.txt` & `layerx-sdk-1.0.9.3/layerx_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `layerx-sdk-1.0.9.2/setup.py` & `layerx-sdk-1.0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.9.2'
+VERSION = '1.0.9.3'
 DESCRIPTION = 'LayerX Python SDK'
 LONG_DESCRIPTION = 'Python API Client to interact with LayerNext stack'
 
 # Setting up
 setup(
     name="layerx-sdk",
     version=VERSION,
```

