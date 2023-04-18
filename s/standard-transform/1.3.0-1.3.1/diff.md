# Comparing `tmp/standard-transform-1.3.0.tar.gz` & `tmp/standard-transform-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard-transform-1.3.0.tar", last modified: Sat Apr 15 06:35:29 2023, max compression
+gzip compressed data, was "standard-transform-1.3.1.tar", last modified: Tue Apr 18 00:00:44 2023, max compression
```

## Comparing `standard-transform-1.3.0.tar` & `standard-transform-1.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-15 06:35:29.905051 standard-transform-1.3.0/
--rw-r--r--   0 caseysm    (501) staff       (20)     1079 2022-11-16 18:20:55.000000 standard-transform-1.3.0/LICENSE
--rw-r--r--   0 caseysm    (501) staff       (20)       63 2023-04-10 23:37:06.000000 standard-transform-1.3.0/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)     8147 2023-04-15 06:35:29.904875 standard-transform-1.3.0/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     7821 2023-04-15 06:33:04.000000 standard-transform-1.3.0/README.md
--rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-03-28 05:17:19.000000 standard-transform-1.3.0/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-04-15 06:35:29.905097 standard-transform-1.3.0/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1597 2023-04-10 23:43:10.000000 standard-transform-1.3.0/setup.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-15 06:35:29.902946 standard-transform-1.3.0/standard_transform/
--rw-r--r--   0 caseysm    (501) staff       (20)      270 2023-04-15 06:35:10.000000 standard-transform-1.3.0/standard_transform/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     7066 2023-04-10 23:37:06.000000 standard-transform-1.3.0/standard_transform/base.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-15 06:35:29.904003 standard-transform-1.3.0/standard_transform/data/
--rw-r--r--   0 caseysm    (501) staff       (20)    11518 2023-04-15 02:44:52.000000 standard-transform-1.3.0/standard_transform/data/minnie_um_streamline.json
--rw-r--r--   0 caseysm    (501) staff       (20)     5384 2023-04-10 23:37:06.000000 standard-transform-1.3.0/standard_transform/data/v1dd_um_streamline.json
--rw-r--r--   0 caseysm    (501) staff       (20)     5320 2023-04-15 05:43:54.000000 standard-transform-1.3.0/standard_transform/datasets.py
--rw-r--r--   0 caseysm    (501) staff       (20)     9256 2023-04-10 23:37:06.000000 standard-transform-1.3.0/standard_transform/streamlines.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1973 2023-02-25 05:35:09.000000 standard-transform-1.3.0/standard_transform/utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-15 06:35:29.903571 standard-transform-1.3.0/standard_transform.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)     8147 2023-04-15 06:35:29.000000 standard-transform-1.3.0/standard_transform.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      556 2023-04-15 06:35:29.000000 standard-transform-1.3.0/standard_transform.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-04-15 06:35:29.000000 standard-transform-1.3.0/standard_transform.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-04-15 06:35:29.000000 standard-transform-1.3.0/standard_transform.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-04-15 06:35:29.000000 standard-transform-1.3.0/standard_transform.egg-info/top_level.txt
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-15 06:35:29.904559 standard-transform-1.3.0/test/
--rw-r--r--   0 caseysm    (501) staff       (20)     1394 2023-04-10 23:37:06.000000 standard-transform-1.3.0/test/test_streamline.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3762 2023-02-25 05:39:09.000000 standard-transform-1.3.0/test/test_tform.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-18 00:00:44.043508 standard-transform-1.3.1/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1079 2022-11-16 18:20:55.000000 standard-transform-1.3.1/LICENSE
+-rw-r--r--   0 caseysm    (501) staff       (20)       63 2023-04-10 23:37:06.000000 standard-transform-1.3.1/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)     8147 2023-04-18 00:00:44.043212 standard-transform-1.3.1/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)     7821 2023-04-15 06:33:04.000000 standard-transform-1.3.1/README.md
+-rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-03-28 05:17:19.000000 standard-transform-1.3.1/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-04-18 00:00:44.043563 standard-transform-1.3.1/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1597 2023-04-10 23:43:10.000000 standard-transform-1.3.1/setup.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-18 00:00:44.040117 standard-transform-1.3.1/standard_transform/
+-rw-r--r--   0 caseysm    (501) staff       (20)      270 2023-04-18 00:00:27.000000 standard-transform-1.3.1/standard_transform/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     7066 2023-04-10 23:37:06.000000 standard-transform-1.3.1/standard_transform/base.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-18 00:00:44.041939 standard-transform-1.3.1/standard_transform/data/
+-rw-r--r--   0 caseysm    (501) staff       (20)    11518 2023-04-15 02:44:52.000000 standard-transform-1.3.1/standard_transform/data/minnie_um_streamline.json
+-rw-r--r--   0 caseysm    (501) staff       (20)     5384 2023-04-10 23:37:06.000000 standard-transform-1.3.1/standard_transform/data/v1dd_um_streamline.json
+-rw-r--r--   0 caseysm    (501) staff       (20)     5320 2023-04-18 00:00:02.000000 standard-transform-1.3.1/standard_transform/datasets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     9256 2023-04-10 23:37:06.000000 standard-transform-1.3.1/standard_transform/streamlines.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1973 2023-02-25 05:35:09.000000 standard-transform-1.3.1/standard_transform/utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-18 00:00:44.041293 standard-transform-1.3.1/standard_transform.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)     8147 2023-04-18 00:00:44.000000 standard-transform-1.3.1/standard_transform.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      556 2023-04-18 00:00:44.000000 standard-transform-1.3.1/standard_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-04-18 00:00:44.000000 standard-transform-1.3.1/standard_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-04-18 00:00:44.000000 standard-transform-1.3.1/standard_transform.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       19 2023-04-18 00:00:44.000000 standard-transform-1.3.1/standard_transform.egg-info/top_level.txt
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-18 00:00:44.042712 standard-transform-1.3.1/test/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1394 2023-04-10 23:37:06.000000 standard-transform-1.3.1/test/test_streamline.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3762 2023-02-25 05:39:09.000000 standard-transform-1.3.1/test/test_tform.py
```

### Comparing `standard-transform-1.3.0/LICENSE` & `standard-transform-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.0/PKG-INFO` & `standard-transform-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-transform
-Version: 1.3.0
+Version: 1.3.1
 Summary: Define and repeat basic affine transformation tasks for datasets
 Home-page: https://github.com/ceesem/standard_transform
 Author: Casey Schneider-Mizell
 Author-email: caseys@alleninstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `standard-transform-1.3.0/README.md` & `standard-transform-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.0/setup.py` & `standard-transform-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.0/standard_transform/base.py` & `standard-transform-1.3.1/standard_transform/base.py`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.0/standard_transform/data/minnie_um_streamline.json` & `standard-transform-1.3.1/standard_transform/data/minnie_um_streamline.json`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.0/standard_transform/data/v1dd_um_streamline.json` & `standard-transform-1.3.1/standard_transform/data/v1dd_um_streamline.json`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.0/standard_transform/datasets.py` & `standard-transform-1.3.1/standard_transform/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         transform_vx,
         streamline_nm,
         streamline_vx,
     ):
         self.name = name
         self._transform_arbitrary = transform_vx
         self.transform_nm = transform_nm()
-        self.trasnform_vx = transform_vx()
+        self.transform_vx = transform_vx()
 
         self._streamline_arbitrary = streamline_vx
         self.streamline_nm = streamline_nm()
         self.streamline_vx = streamline_vx() 
     
     def transform_res(self, resolution):
         """Transform from arbitrary resolution to oriented microns
```

### Comparing `standard-transform-1.3.0/standard_transform/streamlines.py` & `standard-transform-1.3.1/standard_transform/streamlines.py`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.0/standard_transform/utils.py` & `standard-transform-1.3.1/standard_transform/utils.py`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.0/standard_transform.egg-info/PKG-INFO` & `standard-transform-1.3.1/standard_transform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-transform
-Version: 1.3.0
+Version: 1.3.1
 Summary: Define and repeat basic affine transformation tasks for datasets
 Home-page: https://github.com/ceesem/standard_transform
 Author: Casey Schneider-Mizell
 Author-email: caseys@alleninstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `standard-transform-1.3.0/standard_transform.egg-info/SOURCES.txt` & `standard-transform-1.3.1/standard_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.0/test/test_streamline.py` & `standard-transform-1.3.1/test/test_streamline.py`

 * *Files identical despite different names*

### Comparing `standard-transform-1.3.0/test/test_tform.py` & `standard-transform-1.3.1/test/test_tform.py`

 * *Files identical despite different names*

