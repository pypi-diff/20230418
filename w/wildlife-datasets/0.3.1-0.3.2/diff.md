# Comparing `tmp/wildlife-datasets-0.3.1.tar.gz` & `tmp/wildlife-datasets-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adamluk3/Projects/wildlife-datasets/dist/.tmp-63zv2_bj/wildlife-datasets-0.3.1.tar", last modified: Mon Apr 17 12:30:40 2023, max compression
+gzip compressed data, was "/home/adamluk3/Projects/wildlife-datasets/dist/.tmp-_3uy5vma/wildlife-datasets-0.3.2.tar", last modified: Tue Apr 18 11:25:14 2023, max compression
```

## Comparing `wildlife-datasets-0.3.1.tar` & `wildlife-datasets-0.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.420299 wildlife-datasets-0.3.1/
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1090 2023-02-15 08:36:46.000000 wildlife-datasets-0.3.1/LICENSE
--rw-rw-r--   0 adamluk3 (436797) ai         (501)     5211 2023-04-17 12:31:37.418565 wildlife-datasets-0.3.1/PKG-INFO
--rw-r--r--   0 adamluk3 (436797) ai         (501)     3077 2023-04-17 10:03:35.000000 wildlife-datasets-0.3.1/README.md
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1645 2023-04-17 12:31:14.000000 wildlife-datasets-0.3.1/pyproject.toml
--rw-rw-r--   0 adamluk3 (436797) ai         (501)       38 2023-04-17 12:31:37.421684 wildlife-datasets-0.3.1/setup.cfg
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.295062 wildlife-datasets-0.3.1/wildlife_datasets/
--rw-r--r--   0 adamluk3 (436797) ai         (501)      133 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.1/wildlife_datasets/__init__.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.330529 wildlife-datasets-0.3.1/wildlife_datasets/analysis/
--rw-r--r--   0 adamluk3 (436797) ai         (501)      107 2023-02-14 10:36:30.000000 wildlife-datasets-0.3.1/wildlife_datasets/analysis/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     5059 2023-03-06 09:03:18.000000 wildlife-datasets-0.3.1/wildlife_datasets/analysis/plots.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2698 2023-02-28 08:53:31.000000 wildlife-datasets-0.3.1/wildlife_datasets/analysis/statistics.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.353342 wildlife-datasets-0.3.1/wildlife_datasets/datasets/
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2784 2023-03-17 15:45:48.000000 wildlife-datasets-0.3.1/wildlife_datasets/datasets/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)    49821 2023-04-17 12:03:18.000000 wildlife-datasets-0.3.1/wildlife_datasets/datasets/datasets.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     8059 2023-03-17 12:53:50.000000 wildlife-datasets-0.3.1/wildlife_datasets/datasets/metadata.csv
--rw-r--r--   0 adamluk3 (436797) ai         (501)      822 2023-02-14 14:45:05.000000 wildlife-datasets-0.3.1/wildlife_datasets/datasets/metadata.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2843 2023-02-10 15:33:13.000000 wildlife-datasets-0.3.1/wildlife_datasets/datasets/utils.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.367023 wildlife-datasets-0.3.1/wildlife_datasets/downloads/
--rw-r--r--   0 adamluk3 (436797) ai         (501)       25 2023-03-11 08:49:06.000000 wildlife-datasets-0.3.1/wildlife_datasets/downloads/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)    24699 2023-03-17 16:06:21.000000 wildlife-datasets-0.3.1/wildlife_datasets/downloads/downloads.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1495 2023-03-16 15:44:33.000000 wildlife-datasets-0.3.1/wildlife_datasets/downloads/utils.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.376419 wildlife-datasets-0.3.1/wildlife_datasets/loader/
--rw-r--r--   0 adamluk3 (436797) ai         (501)       22 2023-02-14 10:26:57.000000 wildlife-datasets-0.3.1/wildlife_datasets/loader/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2958 2023-03-16 15:27:00.000000 wildlife-datasets-0.3.1/wildlife_datasets/loader/loader.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.385221 wildlife-datasets-0.3.1/wildlife_datasets/metrics/
--rw-r--r--   0 adamluk3 (436797) ai         (501)       23 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.1/wildlife_datasets/metrics/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     3269 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.1/wildlife_datasets/metrics/metrics.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.412327 wildlife-datasets-0.3.1/wildlife_datasets/splits/
--rw-r--r--   0 adamluk3 (436797) ai         (501)      191 2023-03-15 15:44:44.000000 wildlife-datasets-0.3.1/wildlife_datasets/splits/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2653 2023-03-07 14:12:11.000000 wildlife-datasets-0.3.1/wildlife_datasets/splits/analysis.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1896 2023-04-17 11:37:36.000000 wildlife-datasets-0.3.1/wildlife_datasets/splits/balanced_split.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)    11625 2023-04-17 12:28:07.000000 wildlife-datasets-0.3.1/wildlife_datasets/splits/identity_split.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1753 2023-03-07 14:02:45.000000 wildlife-datasets-0.3.1/wildlife_datasets/splits/lcg.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     9516 2023-04-17 12:29:03.000000 wildlife-datasets-0.3.1/wildlife_datasets/splits/time_aware_split.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.317283 wildlife-datasets-0.3.1/wildlife_datasets.egg-info/
--rw-rw-r--   0 adamluk3 (436797) ai         (501)     5211 2023-04-17 12:31:37.000000 wildlife-datasets-0.3.1/wildlife_datasets.egg-info/PKG-INFO
--rw-rw-r--   0 adamluk3 (436797) ai         (501)     1077 2023-04-17 12:31:37.000000 wildlife-datasets-0.3.1/wildlife_datasets.egg-info/SOURCES.txt
--rw-rw-r--   0 adamluk3 (436797) ai         (501)        1 2023-04-17 12:31:37.000000 wildlife-datasets-0.3.1/wildlife_datasets.egg-info/dependency_links.txt
--rw-rw-r--   0 adamluk3 (436797) ai         (501)      130 2023-04-17 12:31:37.000000 wildlife-datasets-0.3.1/wildlife_datasets.egg-info/requires.txt
--rw-rw-r--   0 adamluk3 (436797) ai         (501)       18 2023-04-17 12:31:37.000000 wildlife-datasets-0.3.1/wildlife_datasets.egg-info/top_level.txt
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:12.096180 wildlife-datasets-0.3.2/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1090 2023-02-15 08:36:46.000000 wildlife-datasets-0.3.2/LICENSE
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)     5224 2023-04-18 11:26:12.094760 wildlife-datasets-0.3.2/PKG-INFO
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     3090 2023-04-18 10:47:18.000000 wildlife-datasets-0.3.2/README.md
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1645 2023-04-18 11:26:03.000000 wildlife-datasets-0.3.2/pyproject.toml
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)       38 2023-04-18 11:26:12.097306 wildlife-datasets-0.3.2/setup.cfg
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:11.977176 wildlife-datasets-0.3.2/wildlife_datasets/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      133 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.2/wildlife_datasets/__init__.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:12.008744 wildlife-datasets-0.3.2/wildlife_datasets/analysis/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      107 2023-02-14 10:36:30.000000 wildlife-datasets-0.3.2/wildlife_datasets/analysis/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     5059 2023-03-06 09:03:18.000000 wildlife-datasets-0.3.2/wildlife_datasets/analysis/plots.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2698 2023-02-28 08:53:31.000000 wildlife-datasets-0.3.2/wildlife_datasets/analysis/statistics.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:12.031554 wildlife-datasets-0.3.2/wildlife_datasets/datasets/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2784 2023-03-17 15:45:48.000000 wildlife-datasets-0.3.2/wildlife_datasets/datasets/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)    49821 2023-04-17 12:03:18.000000 wildlife-datasets-0.3.2/wildlife_datasets/datasets/datasets.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     8059 2023-03-17 12:53:50.000000 wildlife-datasets-0.3.2/wildlife_datasets/datasets/metadata.csv
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      822 2023-02-14 14:45:05.000000 wildlife-datasets-0.3.2/wildlife_datasets/datasets/metadata.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2843 2023-02-10 15:33:13.000000 wildlife-datasets-0.3.2/wildlife_datasets/datasets/utils.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:12.045010 wildlife-datasets-0.3.2/wildlife_datasets/downloads/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)       25 2023-03-11 08:49:06.000000 wildlife-datasets-0.3.2/wildlife_datasets/downloads/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)    26116 2023-04-18 10:44:32.000000 wildlife-datasets-0.3.2/wildlife_datasets/downloads/downloads.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1495 2023-03-16 15:44:33.000000 wildlife-datasets-0.3.2/wildlife_datasets/downloads/utils.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:12.054015 wildlife-datasets-0.3.2/wildlife_datasets/loader/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)       22 2023-02-14 10:26:57.000000 wildlife-datasets-0.3.2/wildlife_datasets/loader/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2958 2023-03-16 15:27:00.000000 wildlife-datasets-0.3.2/wildlife_datasets/loader/loader.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:12.062970 wildlife-datasets-0.3.2/wildlife_datasets/metrics/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)       23 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.2/wildlife_datasets/metrics/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     3269 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.2/wildlife_datasets/metrics/metrics.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:12.089626 wildlife-datasets-0.3.2/wildlife_datasets/splits/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      191 2023-03-15 15:44:44.000000 wildlife-datasets-0.3.2/wildlife_datasets/splits/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2653 2023-03-07 14:12:11.000000 wildlife-datasets-0.3.2/wildlife_datasets/splits/analysis.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1896 2023-04-17 11:37:36.000000 wildlife-datasets-0.3.2/wildlife_datasets/splits/balanced_split.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)    11625 2023-04-17 12:28:07.000000 wildlife-datasets-0.3.2/wildlife_datasets/splits/identity_split.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1753 2023-03-07 14:02:45.000000 wildlife-datasets-0.3.2/wildlife_datasets/splits/lcg.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     9516 2023-04-17 12:29:03.000000 wildlife-datasets-0.3.2/wildlife_datasets/splits/time_aware_split.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-18 11:26:11.995873 wildlife-datasets-0.3.2/wildlife_datasets.egg-info/
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)     5224 2023-04-18 11:26:11.000000 wildlife-datasets-0.3.2/wildlife_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)     1077 2023-04-18 11:26:11.000000 wildlife-datasets-0.3.2/wildlife_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)        1 2023-04-18 11:26:11.000000 wildlife-datasets-0.3.2/wildlife_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)      130 2023-04-18 11:26:11.000000 wildlife-datasets-0.3.2/wildlife_datasets.egg-info/requires.txt
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)       18 2023-04-18 11:26:11.000000 wildlife-datasets-0.3.2/wildlife_datasets.egg-info/top_level.txt
```

### Comparing `wildlife-datasets-0.3.1/LICENSE` & `wildlife-datasets-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/PKG-INFO` & `wildlife-datasets-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wildlife-datasets
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library for easier access and research of wildlife re-identification datasets
 Author-email: Lukáš Adam <lukas.adam.cr@gmail.com>, Vojtěch Čermák <cermak.vojtech@seznam.cz>
 Maintainer-email: Lukáš Adam <lukas.adam.cr@gmail.com>, Vojtěch Čermák <cermak.vojtech@seznam.cz>
 License: MIT License
         
         Copyright (c) 2023 Lukáš Adam and Vojtěch Čermák
         
@@ -69,15 +69,15 @@
 ## Basic functionality
 
 We show an example of downloading, extracting and processing the MacaqueFaces dataset.
 
 ```
 from wildlife_datasets import analysis, datasets
 
-datasets.MacaqueFaces.get_data('data')
+datasets.MacaqueFaces.get_data('data/MacaqueFaces')
 dataset = datasets.MacaqueFaces('data/MacaqueFaces')
 ```
 
 The class `dataset` contains the summary of the dataset. The content depends on the dataset. Each dataset contains the identity and paths to images. This particular dataset also contains information about the date taken and contrast. Other datasets store information about bounding boxes, segmentation masks, position from which the image was taken, keypoints or various other information such as age or gender.
 
 ```
 dataset.df
```

### Comparing `wildlife-datasets-0.3.1/README.md` & `wildlife-datasets-0.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 ## Basic functionality
 
 We show an example of downloading, extracting and processing the MacaqueFaces dataset.
 
 ```
 from wildlife_datasets import analysis, datasets
 
-datasets.MacaqueFaces.get_data('data')
+datasets.MacaqueFaces.get_data('data/MacaqueFaces')
 dataset = datasets.MacaqueFaces('data/MacaqueFaces')
 ```
 
 The class `dataset` contains the summary of the dataset. The content depends on the dataset. Each dataset contains the identity and paths to images. This particular dataset also contains information about the date taken and contrast. Other datasets store information about bounding boxes, segmentation masks, position from which the image was taken, keypoints or various other information such as age or gender.
 
 ```
 dataset.df
```

### Comparing `wildlife-datasets-0.3.1/pyproject.toml` & `wildlife-datasets-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wildlife-datasets"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Lukáš Adam", email="lukas.adam.cr@gmail.com" },
   { name="Vojtěch Čermák", email="cermak.vojtech@seznam.cz" },
 ]
 maintainers = [
   { name="Lukáš Adam", email="lukas.adam.cr@gmail.com" },
   { name="Vojtěch Čermák", email="cermak.vojtech@seznam.cz" },
```

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/analysis/plots.py` & `wildlife-datasets-0.3.2/wildlife_datasets/analysis/plots.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/analysis/statistics.py` & `wildlife-datasets-0.3.2/wildlife_datasets/analysis/statistics.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/datasets/__init__.py` & `wildlife-datasets-0.3.2/wildlife_datasets/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/datasets/datasets.py` & `wildlife-datasets-0.3.2/wildlife_datasets/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/datasets/metadata.csv` & `wildlife-datasets-0.3.2/wildlife_datasets/datasets/metadata.csv`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/datasets/metadata.py` & `wildlife-datasets-0.3.2/wildlife_datasets/datasets/metadata.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/datasets/utils.py` & `wildlife-datasets-0.3.2/wildlife_datasets/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/downloads/downloads.py` & `wildlife-datasets-0.3.2/wildlife_datasets/downloads/downloads.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,71 @@
 import os
 import shutil
 from . import utils
 
 
 class Downloader():
-    def get_data(self, root, name=None, **kwargs):
-        if name is None:
-            name = self.__class__.__name__
-        print('DATASET %s: DOWNLOADING STARTED.' % name)        
-        self.download(os.path.join(root, name), **kwargs)
-        print('DATASET %s: EXTRACTING STARTED.' % name)
-        self.extract(os.path.join(root, name), **kwargs)
-        print('DATASET %s: FINISHED. If mass downloading, you can remove it from the list.\n' % name)
-
-    def download(self, root, **kwargs):
-        with utils.data_directory(root):
-            self._download(**kwargs)
+    download_warning = '''You are trying to download an already downloaded dataset.
+        This message may have happened to due interrupted download or extract.
+        To force the download use the `force=True` keyword such as
+        get_data(..., force=True) or download(..., force=True).
+        '''
+    download_mark_name = 'already_downloaded'
+        
+    def get_data(self, root, force=False, **kwargs):
+        name = self.__class__.__name__
+        
+        already_downloaded = self.check_downloaded_mark(root)
+        if already_downloaded and not force:
+            print('DATASET %s: DOWNLOADING STARTED.' % name)
+            print(self.download_warning)
+        else:
+            print('DATASET %s: DOWNLOADING STARTED.' % name)
+            self.download(root, force=force, **kwargs)
+            print('DATASET %s: EXTRACTING STARTED.' % name)
+            self.extract(root,  **kwargs)
+            print('DATASET %s: FINISHED.\n' % name)
+
+    def download(self, root, force=False, **kwargs):
+        name = self.__class__.__name__
+
+        already_downloaded = self.check_downloaded_mark(root)
+        if already_downloaded and not force:
+            print('DATASET %s: DOWNLOADING STARTED.' % name)            
+            print(self.download_warning)
+        else:
+            self.remove_download_mark(root)
+            with utils.data_directory(root):
+                self._download(**kwargs)
+            self.add_downloaded_mark(root)
     
     def extract(self, root, **kwargs):
         with utils.data_directory(root):
             self._extract(**kwargs)
 
     def _download(self, *args, **kwargs):
         raise NotImplemented('Needs to be implemented by subclasses.')
     
     def _extract(self, *args, **kwargs):
         raise NotImplemented('Needs to be implemented by subclasses.')
 
+    def check_downloaded_mark(self, root):
+        file_name = os.path.join(root, self.download_mark_name)
+        return os.path.exists(file_name)
+
+    def add_downloaded_mark(self, root):
+        if not os.path.exists(root):
+            os.makedirs(root)
+        file_name = os.path.join(root, self.download_mark_name)
+        open(file_name, 'a').close()
+
+    def remove_download_mark(self, root):
+        file_name = os.path.join(root, self.download_mark_name)
+        if os.path.exists(file_name):
+            os.remove(file_name)
 
 class AAUZebraFish(Downloader):
     archive = 'aau-zebrafish-reid.zip'
 
     def _download(self):
         command = f"datasets download -d 'aalborguniversity/aau-zebrafish-reid'"
         exception_text = '''Kaggle must be setup.
```

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/downloads/utils.py` & `wildlife-datasets-0.3.2/wildlife_datasets/downloads/utils.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/loader/loader.py` & `wildlife-datasets-0.3.2/wildlife_datasets/loader/loader.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/metrics/metrics.py` & `wildlife-datasets-0.3.2/wildlife_datasets/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/splits/analysis.py` & `wildlife-datasets-0.3.2/wildlife_datasets/splits/analysis.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/splits/balanced_split.py` & `wildlife-datasets-0.3.2/wildlife_datasets/splits/balanced_split.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/splits/identity_split.py` & `wildlife-datasets-0.3.2/wildlife_datasets/splits/identity_split.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/splits/lcg.py` & `wildlife-datasets-0.3.2/wildlife_datasets/splits/lcg.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets/splits/time_aware_split.py` & `wildlife-datasets-0.3.2/wildlife_datasets/splits/time_aware_split.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets.egg-info/PKG-INFO` & `wildlife-datasets-0.3.2/wildlife_datasets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wildlife-datasets
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library for easier access and research of wildlife re-identification datasets
 Author-email: Lukáš Adam <lukas.adam.cr@gmail.com>, Vojtěch Čermák <cermak.vojtech@seznam.cz>
 Maintainer-email: Lukáš Adam <lukas.adam.cr@gmail.com>, Vojtěch Čermák <cermak.vojtech@seznam.cz>
 License: MIT License
         
         Copyright (c) 2023 Lukáš Adam and Vojtěch Čermák
         
@@ -69,15 +69,15 @@
 ## Basic functionality
 
 We show an example of downloading, extracting and processing the MacaqueFaces dataset.
 
 ```
 from wildlife_datasets import analysis, datasets
 
-datasets.MacaqueFaces.get_data('data')
+datasets.MacaqueFaces.get_data('data/MacaqueFaces')
 dataset = datasets.MacaqueFaces('data/MacaqueFaces')
 ```
 
 The class `dataset` contains the summary of the dataset. The content depends on the dataset. Each dataset contains the identity and paths to images. This particular dataset also contains information about the date taken and contrast. Other datasets store information about bounding boxes, segmentation masks, position from which the image was taken, keypoints or various other information such as age or gender.
 
 ```
 dataset.df
```

### Comparing `wildlife-datasets-0.3.1/wildlife_datasets.egg-info/SOURCES.txt` & `wildlife-datasets-0.3.2/wildlife_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

