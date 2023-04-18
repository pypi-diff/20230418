# Comparing `tmp/tmart-1.3.3.tar.gz` & `tmp/tmart-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmart-1.3.3.tar", last modified: Mon Apr 10 04:22:56 2023, max compression
+gzip compressed data, was "tmart-1.3.5.tar", last modified: Tue Apr 18 04:12:39 2023, max compression
```

## Comparing `tmart-1.3.3.tar` & `tmart-1.3.5.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-10 04:22:56.718859 tmart-1.3.3/
--rw-r--r--   0 yw         (501) staff       (20)       45 2022-09-20 16:15:46.000000 tmart-1.3.3/MANIFEST.in
--rw-r--r--   0 yw         (501) staff       (20)     3803 2023-04-10 04:22:56.718645 tmart-1.3.3/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)     3181 2023-04-03 04:04:03.000000 tmart-1.3.3/README.md
--rw-r--r--   0 yw         (501) staff       (20)       38 2023-04-10 04:22:56.718929 tmart-1.3.3/setup.cfg
--rw-r--r--   0 yw         (501) staff       (20)     1966 2023-04-10 04:22:07.000000 tmart-1.3.3/setup.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-10 04:22:56.703521 tmart-1.3.3/tests/
--rw-r--r--   0 yw         (501) staff       (20)      246 2023-03-29 21:18:48.000000 tmart-1.3.3/tests/test_AEC.py
--rw-r--r--   0 yw         (501) staff       (20)     3048 2023-01-03 02:43:30.000000 tmart-1.3.3/tests/test_E_diffuse.py
--rw-r--r--   0 yw         (501) staff       (20)     2310 2023-01-03 03:48:03.000000 tmart-1.3.3/tests/test_L_sky.py
--rw-r--r--   0 yw         (501) staff       (20)     1827 2023-03-25 22:34:08.000000 tmart-1.3.3/tests/test_basic.py
--rw-r--r--   0 yw         (501) staff       (20)     1327 2022-09-21 16:59:26.000000 tmart-1.3.3/tests/test_basic_import.py
--rw-r--r--   0 yw         (501) staff       (20)     3197 2022-09-17 14:43:02.000000 tmart-1.3.3/tests/test_calcref.py
--rw-r--r--   0 yw         (501) staff       (20)     2993 2023-03-25 22:34:08.000000 tmart-1.3.3/tests/test_quickstart.py
--rw-r--r--   0 yw         (501) staff       (20)     3113 2022-09-26 04:25:24.000000 tmart-1.3.3/tests/test_specular_contribution.py
--rw-r--r--   0 yw         (501) staff       (20)     3228 2022-09-27 15:07:16.000000 tmart-1.3.3/tests/test_typical_ocean.py
--rw-r--r--   0 yw         (501) staff       (20)     3021 2022-10-03 05:42:50.000000 tmart-1.3.3/tests/test_whales_SR.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-10 04:22:56.705925 tmart-1.3.3/tmart/
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-10 04:22:56.707344 tmart-1.3.3/tmart/AEC/
--rw-r--r--   0 yw         (501) staff       (20)      382 2023-04-08 19:19:35.000000 tmart-1.3.3/tmart/AEC/__init__.py
--rw-r--r--   0 yw         (501) staff       (20)     5614 2023-04-09 15:01:43.000000 tmart-1.3.3/tmart/AEC/get_parameters.py
--rw-r--r--   0 yw         (501) staff       (20)     2727 2023-04-09 23:00:04.000000 tmart-1.3.3/tmart/AEC/reflectance_correction.py
--rw-r--r--   0 yw         (501) staff       (20)     2320 2023-04-08 22:49:14.000000 tmart-1.3.3/tmart/Aerosol.py
--rw-r--r--   0 yw         (501) staff       (20)    10526 2023-04-08 22:49:20.000000 tmart-1.3.3/tmart/Atmosphere.py
--rw-r--r--   0 yw         (501) staff       (20)    10104 2023-04-08 22:49:24.000000 tmart-1.3.3/tmart/Surface.py
--rw-r--r--   0 yw         (501) staff       (20)    13619 2023-04-08 22:50:39.000000 tmart-1.3.3/tmart/Tmart.py
--rw-r--r--   0 yw         (501) staff       (20)    41660 2023-04-08 22:50:38.000000 tmart-1.3.3/tmart/Tmart2.py
--rw-r--r--   0 yw         (501) staff       (20)      522 2023-04-08 22:49:15.000000 tmart-1.3.3/tmart/__init__.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-10 04:22:56.710465 tmart-1.3.3/tmart/ancillary/
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-10 04:22:56.717321 tmart-1.3.3/tmart/ancillary/aerosolSPF/
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:20:25.000000 tmart-1.3.3/tmart/ancillary/aerosolSPF/BiomassBurning.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:49:56.000000 tmart-1.3.3/tmart/ancillary/aerosolSPF/Continental.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:55:10.000000 tmart-1.3.3/tmart/ancillary/aerosolSPF/Desert.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 16:59:28.000000 tmart-1.3.3/tmart/ancillary/aerosolSPF/Maritime.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:21:44.000000 tmart-1.3.3/tmart/ancillary/aerosolSPF/Stratospheric.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:53:59.000000 tmart-1.3.3/tmart/ancillary/aerosolSPF/Urban.csv
--rw-r--r--   0 yw         (501) staff       (20)     1763 2022-12-14 22:44:42.000000 tmart-1.3.3/tmart/ancillary/conifer_forest.csv
--rw-r--r--   0 yw         (501) staff       (20)      838 2022-12-14 22:45:12.000000 tmart-1.3.3/tmart/ancillary/dry_beach_sand.csv
--rw-r--r--   0 yw         (501) staff       (20)     1618 2022-12-14 22:45:48.000000 tmart-1.3.3/tmart/ancillary/lawn_grass.csv
--rw-r--r--   0 yw         (501) staff       (20)      794 2021-08-03 20:21:41.000000 tmart-1.3.3/tmart/ancillary/soil.csv
--rw-r--r--   0 yw         (501) staff       (20)     1190 2021-08-03 20:22:22.000000 tmart-1.3.3/tmart/ancillary/vegetation.csv
--rw-r--r--   0 yw         (501) staff       (20)      284 2021-08-03 20:21:58.000000 tmart-1.3.3/tmart/ancillary/water.csv
--rw-r--r--   0 yw         (501) staff       (20)      707 2022-02-08 17:04:47.000000 tmart-1.3.3/tmart/ancillary/water_chl1.csv
--rw-r--r--   0 yw         (501) staff       (20)     1015 2022-12-14 22:46:19.000000 tmart-1.3.3/tmart/ancillary/wet_beach_sand.csv
--rw-r--r--   0 yw         (501) staff       (20)      181 2023-03-31 22:46:09.000000 tmart-1.3.3/tmart/ancillary/whitecap_factor.csv
--rw-r--r--   0 yw         (501) staff       (20)     2684 2023-04-08 22:50:41.000000 tmart-1.3.3/tmart/tm_OT.py
--rw-r--r--   0 yw         (501) staff       (20)    11784 2023-04-08 22:49:35.000000 tmart-1.3.3/tmart/tm_calcref.py
--rw-r--r--   0 yw         (501) staff       (20)     4094 2023-04-08 22:49:45.000000 tmart-1.3.3/tmart/tm_geometry.py
--rw-r--r--   0 yw         (501) staff       (20)    19399 2023-04-08 22:49:52.000000 tmart-1.3.3/tmart/tm_intersect.py
--rw-r--r--   0 yw         (501) staff       (20)    11289 2023-04-08 22:50:00.000000 tmart-1.3.3/tmart/tm_move.py
--rw-r--r--   0 yw         (501) staff       (20)     8649 2023-04-08 22:50:40.000000 tmart-1.3.3/tmart/tm_sampling.py
--rw-r--r--   0 yw         (501) staff       (20)    20018 2023-04-08 22:50:39.000000 tmart-1.3.3/tmart/tm_water.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-10 04:22:56.706662 tmart-1.3.3/tmart.egg-info/
--rw-r--r--   0 yw         (501) staff       (20)     3803 2023-04-10 04:22:56.000000 tmart-1.3.3/tmart.egg-info/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)     1275 2023-04-10 04:22:56.000000 tmart-1.3.3/tmart.egg-info/SOURCES.txt
--rw-r--r--   0 yw         (501) staff       (20)        1 2023-04-10 04:22:56.000000 tmart-1.3.3/tmart.egg-info/dependency_links.txt
--rw-r--r--   0 yw         (501) staff       (20)       50 2023-04-10 04:22:56.000000 tmart-1.3.3/tmart.egg-info/requires.txt
--rw-r--r--   0 yw         (501) staff       (20)        6 2023-04-10 04:22:56.000000 tmart-1.3.3/tmart.egg-info/top_level.txt
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-18 04:12:39.030787 tmart-1.3.5/
+-rw-r--r--   0 yw         (501) staff       (20)       45 2022-09-20 16:15:46.000000 tmart-1.3.5/MANIFEST.in
+-rw-r--r--   0 yw         (501) staff       (20)     3891 2023-04-18 04:12:39.030585 tmart-1.3.5/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     3269 2023-04-13 02:42:26.000000 tmart-1.3.5/README.md
+-rw-r--r--   0 yw         (501) staff       (20)       38 2023-04-18 04:12:39.030847 tmart-1.3.5/setup.cfg
+-rw-r--r--   0 yw         (501) staff       (20)     1966 2023-04-18 04:12:02.000000 tmart-1.3.5/setup.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-18 04:12:39.007312 tmart-1.3.5/tests/
+-rw-r--r--   0 yw         (501) staff       (20)      246 2023-03-29 21:18:48.000000 tmart-1.3.5/tests/test_AEC.py
+-rw-r--r--   0 yw         (501) staff       (20)     3048 2023-01-03 02:43:30.000000 tmart-1.3.5/tests/test_E_diffuse.py
+-rw-r--r--   0 yw         (501) staff       (20)     2310 2023-01-03 03:48:03.000000 tmart-1.3.5/tests/test_L_sky.py
+-rw-r--r--   0 yw         (501) staff       (20)     1827 2023-03-25 22:34:08.000000 tmart-1.3.5/tests/test_basic.py
+-rw-r--r--   0 yw         (501) staff       (20)     1327 2022-09-21 16:59:26.000000 tmart-1.3.5/tests/test_basic_import.py
+-rw-r--r--   0 yw         (501) staff       (20)     3197 2022-09-17 14:43:02.000000 tmart-1.3.5/tests/test_calcref.py
+-rw-r--r--   0 yw         (501) staff       (20)     2993 2023-03-25 22:34:08.000000 tmart-1.3.5/tests/test_quickstart.py
+-rw-r--r--   0 yw         (501) staff       (20)     3113 2022-09-26 04:25:24.000000 tmart-1.3.5/tests/test_specular_contribution.py
+-rw-r--r--   0 yw         (501) staff       (20)     3228 2022-09-27 15:07:16.000000 tmart-1.3.5/tests/test_typical_ocean.py
+-rw-r--r--   0 yw         (501) staff       (20)     3021 2022-10-03 05:42:50.000000 tmart-1.3.5/tests/test_whales_SR.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-18 04:12:39.016323 tmart-1.3.5/tmart/
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-18 04:12:39.018388 tmart-1.3.5/tmart/AEC/
+-rw-r--r--   0 yw         (501) staff       (20)      449 2023-04-12 06:15:34.000000 tmart-1.3.5/tmart/AEC/__init__.py
+-rw-r--r--   0 yw         (501) staff       (20)     5017 2023-04-18 02:10:19.000000 tmart-1.3.5/tmart/AEC/get_parameters.py
+-rw-r--r--   0 yw         (501) staff       (20)     1411 2023-04-12 07:00:02.000000 tmart-1.3.5/tmart/AEC/read_PRISMA_north.py
+-rw-r--r--   0 yw         (501) staff       (20)     2864 2023-04-12 04:52:05.000000 tmart-1.3.5/tmart/AEC/read_PRISMA_vaa.py
+-rw-r--r--   0 yw         (501) staff       (20)     3140 2023-04-18 01:29:46.000000 tmart-1.3.5/tmart/AEC/reflectance_correction.py
+-rw-r--r--   0 yw         (501) staff       (20)     2320 2023-04-08 22:49:14.000000 tmart-1.3.5/tmart/Aerosol.py
+-rw-r--r--   0 yw         (501) staff       (20)    10526 2023-04-08 22:49:20.000000 tmart-1.3.5/tmart/Atmosphere.py
+-rw-r--r--   0 yw         (501) staff       (20)    10104 2023-04-08 22:49:24.000000 tmart-1.3.5/tmart/Surface.py
+-rw-r--r--   0 yw         (501) staff       (20)    13619 2023-04-08 22:50:39.000000 tmart-1.3.5/tmart/Tmart.py
+-rw-r--r--   0 yw         (501) staff       (20)    41660 2023-04-08 22:50:38.000000 tmart-1.3.5/tmart/Tmart2.py
+-rw-r--r--   0 yw         (501) staff       (20)      522 2023-04-08 22:49:15.000000 tmart-1.3.5/tmart/__init__.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-18 04:12:39.022246 tmart-1.3.5/tmart/ancillary/
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-18 04:12:39.029112 tmart-1.3.5/tmart/ancillary/aerosolSPF/
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:20:25.000000 tmart-1.3.5/tmart/ancillary/aerosolSPF/BiomassBurning.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:49:56.000000 tmart-1.3.5/tmart/ancillary/aerosolSPF/Continental.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:55:10.000000 tmart-1.3.5/tmart/ancillary/aerosolSPF/Desert.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 16:59:28.000000 tmart-1.3.5/tmart/ancillary/aerosolSPF/Maritime.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:21:44.000000 tmart-1.3.5/tmart/ancillary/aerosolSPF/Stratospheric.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:53:59.000000 tmart-1.3.5/tmart/ancillary/aerosolSPF/Urban.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1763 2022-12-14 22:44:42.000000 tmart-1.3.5/tmart/ancillary/conifer_forest.csv
+-rw-r--r--   0 yw         (501) staff       (20)      838 2022-12-14 22:45:12.000000 tmart-1.3.5/tmart/ancillary/dry_beach_sand.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1618 2022-12-14 22:45:48.000000 tmart-1.3.5/tmart/ancillary/lawn_grass.csv
+-rw-r--r--   0 yw         (501) staff       (20)      794 2021-08-03 20:21:41.000000 tmart-1.3.5/tmart/ancillary/soil.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1190 2021-08-03 20:22:22.000000 tmart-1.3.5/tmart/ancillary/vegetation.csv
+-rw-r--r--   0 yw         (501) staff       (20)      284 2021-08-03 20:21:58.000000 tmart-1.3.5/tmart/ancillary/water.csv
+-rw-r--r--   0 yw         (501) staff       (20)      707 2022-02-08 17:04:47.000000 tmart-1.3.5/tmart/ancillary/water_chl1.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1015 2022-12-14 22:46:19.000000 tmart-1.3.5/tmart/ancillary/wet_beach_sand.csv
+-rw-r--r--   0 yw         (501) staff       (20)      181 2023-03-31 22:46:09.000000 tmart-1.3.5/tmart/ancillary/whitecap_factor.csv
+-rw-r--r--   0 yw         (501) staff       (20)     2684 2023-04-08 22:50:41.000000 tmart-1.3.5/tmart/tm_OT.py
+-rw-r--r--   0 yw         (501) staff       (20)    11784 2023-04-08 22:49:35.000000 tmart-1.3.5/tmart/tm_calcref.py
+-rw-r--r--   0 yw         (501) staff       (20)     4094 2023-04-08 22:49:45.000000 tmart-1.3.5/tmart/tm_geometry.py
+-rw-r--r--   0 yw         (501) staff       (20)    19399 2023-04-08 22:49:52.000000 tmart-1.3.5/tmart/tm_intersect.py
+-rw-r--r--   0 yw         (501) staff       (20)    11289 2023-04-08 22:50:00.000000 tmart-1.3.5/tmart/tm_move.py
+-rw-r--r--   0 yw         (501) staff       (20)     8649 2023-04-08 22:50:40.000000 tmart-1.3.5/tmart/tm_sampling.py
+-rw-r--r--   0 yw         (501) staff       (20)    20018 2023-04-08 22:50:39.000000 tmart-1.3.5/tmart/tm_water.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-18 04:12:39.017042 tmart-1.3.5/tmart.egg-info/
+-rw-r--r--   0 yw         (501) staff       (20)     3891 2023-04-18 04:12:38.000000 tmart-1.3.5/tmart.egg-info/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     1335 2023-04-18 04:12:38.000000 tmart-1.3.5/tmart.egg-info/SOURCES.txt
+-rw-r--r--   0 yw         (501) staff       (20)        1 2023-04-18 04:12:38.000000 tmart-1.3.5/tmart.egg-info/dependency_links.txt
+-rw-r--r--   0 yw         (501) staff       (20)       50 2023-04-18 04:12:38.000000 tmart-1.3.5/tmart.egg-info/requires.txt
+-rw-r--r--   0 yw         (501) staff       (20)        6 2023-04-18 04:12:38.000000 tmart-1.3.5/tmart.egg-info/top_level.txt
```

### Comparing `tmart-1.3.3/PKG-INFO` & `tmart-1.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmart
-Version: 1.3.3
+Version: 1.3.5
 Summary: Radiative transfer modelling for aquatic remote sensing
 Author: Yulun Wu
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # T-Mart: Topography-adjusted Monte-carlo Adjacency-effect Radiative Transfer Code
 
 ## Description 
 
-T-Mart solves the radiative transfer in a 3D ocean-atmosphere system through a Monte-Carlo approach. T-Mart features arbitrary surface models which allow simulating and correcting for the adjacnecy effect in aquatic remote sensing. 
+T-Mart solves the radiative transfer in a 3D surface-atmosphere system through a Monte-Carlo approach. T-Mart features arbitrary surface models which allow simulating and correcting for the adjacnecy effect in aquatic remote sensing. 
 
 
 ## Links
 
 
 Home page: <a href="https://github.com/yulunwu8/tmart" target="_blank">https://github.com/yulunwu8/tmart</a>
 
@@ -117,10 +117,11 @@
 
 ```
 
 
 
 ## Other
 
+T-Mart can calculate reflectances of various units, see Table 1 in Wu et al. (2023). 
 
 For questions and suggestions (which I'm always open to!), please email Yulun at [yulunwu8@gmail.com](mailto:yulunwu8@gmail.com)
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: tmart Version: 1.3.3 Summary: Radiative transfer
+Metadata-Version: 2.1 Name: tmart Version: 1.3.5 Summary: Radiative transfer
 modelling for aquatic remote sensing Author: Yulun Wu Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
 Atmospheric Science Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown # T-Mart: Topography-adjusted Monte-carlo Adjacency-effect
 Radiative Transfer Code ## Description T-Mart solves the radiative transfer in
-a 3D ocean-atmosphere system through a Monte-Carlo approach. T-Mart features
+a 3D surface-atmosphere system through a Monte-Carlo approach. T-Mart features
 arbitrary surface models which allow simulating and correcting for the
 adjacnecy effect in aquatic remote sensing. ## Links Home page: https://
 github.com/yulunwu8/tmart User guide: https://tmart-rtm.github.io ##
 Publication Wu, Y., Knudby, A., & Lapen, D. (2023). Topography-Adjusted Monte
 Carlo Simulation of the Adjacency Effect in Remote Sensing of Coastal and
 Inland Waters. *Journal of Quantitative Spectroscopy and Radiative Transfer*,
 108589. https://doi.org/10.1016/j.jqsrt.2023.108589 ## Installation 1 - Create
@@ -37,10 +37,11 @@
 v) ``` Output should be similar to this: ``` ========= Initiating T-Mart
 ========= Number of photons: 10000 Using 10 core(s) Number of job(s): 100
 Wavelength: 400 target_pt_direction: [180, 0] sun_dir: [0, 0]
 ===================================== Tasks remaining = 102 Tasks remaining =
 72 Tasks remaining = 42 Tasks remaining = 12
 ===================================== Calculating radiative properties... R_atm
 0.12760589889823587 R_dir 0.06046419017201067 R_env 0.012888590547129805
-R_total 0.20095867961737635 ``` ## Other For questions and suggestions (which
-I'm always open to!), please email Yulun at [yulunwu8@gmail.com](mailto:
+R_total 0.20095867961737635 ``` ## Other T-Mart can calculate reflectances of
+various units, see Table 1 in Wu et al. (2023). For questions and suggestions
+(which I'm always open to!), please email Yulun at [yulunwu8@gmail.com](mailto:
 yulunwu8@gmail.com)
```

### Comparing `tmart-1.3.3/README.md` & `tmart-1.3.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # T-Mart: Topography-adjusted Monte-carlo Adjacency-effect Radiative Transfer Code
 
 ## Description 
 
-T-Mart solves the radiative transfer in a 3D ocean-atmosphere system through a Monte-Carlo approach. T-Mart features arbitrary surface models which allow simulating and correcting for the adjacnecy effect in aquatic remote sensing. 
+T-Mart solves the radiative transfer in a 3D surface-atmosphere system through a Monte-Carlo approach. T-Mart features arbitrary surface models which allow simulating and correcting for the adjacnecy effect in aquatic remote sensing. 
 
 
 ## Links
 
 
 Home page: <a href="https://github.com/yulunwu8/tmart" target="_blank">https://github.com/yulunwu8/tmart</a>
 
@@ -102,10 +102,11 @@
 
 ```
 
 
 
 ## Other
 
+T-Mart can calculate reflectances of various units, see Table 1 in Wu et al. (2023). 
 
 For questions and suggestions (which I'm always open to!), please email Yulun at [yulunwu8@gmail.com](mailto:yulunwu8@gmail.com)
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # T-Mart: Topography-adjusted Monte-carlo Adjacency-effect Radiative Transfer
-Code ## Description T-Mart solves the radiative transfer in a 3D ocean-
+Code ## Description T-Mart solves the radiative transfer in a 3D surface-
 atmosphere system through a Monte-Carlo approach. T-Mart features arbitrary
 surface models which allow simulating and correcting for the adjacnecy effect
 in aquatic remote sensing. ## Links Home page: https://github.com/yulunwu8/
 tmart User guide: https://tmart-rtm.github.io ## Publication Wu, Y., Knudby,
 A., & Lapen, D. (2023). Topography-Adjusted Monte Carlo Simulation of the
 Adjacency Effect in Remote Sensing of Coastal and Inland Waters. *Journal of
 Quantitative Spectroscopy and Radiative Transfer*, 108589. https://doi.org/
@@ -28,10 +28,11 @@
 k, v in R.items(): print(k, ' ' , v) ``` Output should be similar to this: ```
 ========= Initiating T-Mart ========= Number of photons: 10000 Using 10 core(s)
 Number of job(s): 100 Wavelength: 400 target_pt_direction: [180, 0] sun_dir:
 [0, 0] ===================================== Tasks remaining = 102 Tasks
 remaining = 72 Tasks remaining = 42 Tasks remaining = 12
 ===================================== Calculating radiative properties... R_atm
 0.12760589889823587 R_dir 0.06046419017201067 R_env 0.012888590547129805
-R_total 0.20095867961737635 ``` ## Other For questions and suggestions (which
-I'm always open to!), please email Yulun at [yulunwu8@gmail.com](mailto:
+R_total 0.20095867961737635 ``` ## Other T-Mart can calculate reflectances of
+various units, see Table 1 in Wu et al. (2023). For questions and suggestions
+(which I'm always open to!), please email Yulun at [yulunwu8@gmail.com](mailto:
 yulunwu8@gmail.com)
```

### Comparing `tmart-1.3.3/setup.py` & `tmart-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tmart",                     # This is the name of the package
-    version="1.3.3",                       
+    version="1.3.5",                       
     author="Yulun Wu",                     # Full name of the author
     description="Radiative transfer modelling for aquatic remote sensing",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     # packages=setuptools.find_packages(),    # List of all python modules to be installed
     packages = ['tmart','tmart.AEC','tmart.ancillary','tmart.ancillary.aerosolSPF'],
     include_package_data=True,
```

### Comparing `tmart-1.3.3/tests/test_E_diffuse.py` & `tmart-1.3.5/tests/test_E_diffuse.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tests/test_L_sky.py` & `tmart-1.3.5/tests/test_L_sky.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tests/test_basic.py` & `tmart-1.3.5/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tests/test_basic_import.py` & `tmart-1.3.5/tests/test_basic_import.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tests/test_calcref.py` & `tmart-1.3.5/tests/test_calcref.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tests/test_quickstart.py` & `tmart-1.3.5/tests/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tests/test_specular_contribution.py` & `tmart-1.3.5/tests/test_specular_contribution.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tests/test_typical_ocean.py` & `tmart-1.3.5/tests/test_typical_ocean.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tests/test_whales_SR.py` & `tmart-1.3.5/tests/test_whales_SR.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/AEC/get_parameters.py` & `tmart-1.3.5/tmart/AEC/get_parameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -132,55 +132,14 @@
                                     cell_size = 200,
                                     window_size=5)
     
     # print(test)
     test1 = test['conv_window_1']
 
 
-'''
-
-### Test AEC
-
-# image_test = image_reflectance.copy()
-
-image_test = np.full((window_size_x, window_size_y), 0.39378) # unitless    
-
-
-# image_test[:,6:] = 0.5
-
-image_test[5,5] = 0
-
-import scipy.signal
-
-filter_kernel = np.flip(conv_window_1) # it's flipped in convolve by default
-R_conv = scipy.signal.convolve2d(image_test, filter_kernel,
-                              mode='same', boundary='fill', fillvalue=image_test.mean())
-
-
-# print(R_conv)
-
-# centre 
-centre_R_conv = R_conv[int(R_conv.shape[0]/2),int(R_conv.shape[1]/2)]
-print('\ncentre_R_conv:')
-print(centre_R_conv)
-
-
-'''
-
-
-
-
-
-
-
-
-
-
-
-
```

### Comparing `tmart-1.3.3/tmart/AEC/reflectance_correction.py` & `tmart-1.3.5/tmart/AEC/reflectance_correction.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,26 @@
 
 
 ### Correct for the non-linearity of the ratio of environmental irradiance to surface reflectance for homogeneous Lambertian surfaces. 
 
 from Py6S import *
 
 def reflectance_correction(image, wl_RC, 
-                           tm_vza, tm_vaa, tm_sza, tm_saa, 
+                           tm_vza = 0, tm_vaa = 0, tm_sza = 0, tm_saa = 0, 
                            atm_profile = None, 
                            aerosol_type = 'Maritime', aot550 = 0):
     
     import numpy as np
     import sys
     
+    
+    # An unknown bug of 6S unable to handle 551nm
+    if wl_RC == 0.551: wl_RC = 0.55
+    
+    
     mean_image = np.mean(image)
     
     # SixS
     s = SixS()
     
     s.geometry = Geometry.User()
     s.geometry.solar_z = tm_sza
@@ -60,45 +65,61 @@
     for SR in list_SR:
         s.ground_reflectance = GroundReflectance.HomogeneousLambertian(SR)
         s.run()
         list_R_dir.append(s.outputs.values['pixel_reflectance'])
     
     list_R_dir
     
-    
     array_R_dir = np.array(list_R_dir)
     array_SR = np.array(list_SR)
     array_ratio = array_R_dir / array_SR
     
     fit_ratio_SR = np.polyfit(array_SR , array_ratio, 2)
     p = np.poly1d(fit_ratio_SR)
-    
     mean_ratio = p(mean_image)
-    
     ratio = p(image)
     
     correction = ratio / mean_ratio
     
     # do not correct pixels brighter than mean 
     correction[correction>1] = 1
     
-    
     image_out = image * correction
     
     max_correction = correction.min()
+    
+    # max_correction = np.nanmin(correction)
+    
     max_correction_percent = str(round((1 - max_correction)*100, 2))
     
     print('Maximum change: ' + max_correction_percent + '%')
     
     
     return image_out
 
 
 
 
+# if __name__ == "__main__":
+#     import numpy as np
+#     import netCDF4 as nc4
+#     file = 'test.nc'
+#     with nc4.Dataset(file, 'r')  as dset:
+#         a_test = dset['rhot_551'][:]
+#     test = reflectance_correction(a_test, 0.551)
+    
+    
+
+    
+
+
+
+
+
+
```

### Comparing `tmart-1.3.3/tmart/Aerosol.py` & `tmart-1.3.5/tmart/Aerosol.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/Atmosphere.py` & `tmart-1.3.5/tmart/Atmosphere.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/Surface.py` & `tmart-1.3.5/tmart/Surface.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/Tmart.py` & `tmart-1.3.5/tmart/Tmart.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/Tmart2.py` & `tmart-1.3.5/tmart/Tmart2.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/__init__.py` & `tmart-1.3.5/tmart/__init__.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/ancillary/aerosolSPF/BiomassBurning.csv` & `tmart-1.3.5/tmart/ancillary/aerosolSPF/BiomassBurning.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/ancillary/aerosolSPF/Continental.csv` & `tmart-1.3.5/tmart/ancillary/aerosolSPF/Continental.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/ancillary/aerosolSPF/Desert.csv` & `tmart-1.3.5/tmart/ancillary/aerosolSPF/Desert.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/ancillary/aerosolSPF/Maritime.csv` & `tmart-1.3.5/tmart/ancillary/aerosolSPF/Maritime.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/ancillary/aerosolSPF/Stratospheric.csv` & `tmart-1.3.5/tmart/ancillary/aerosolSPF/Stratospheric.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/ancillary/aerosolSPF/Urban.csv` & `tmart-1.3.5/tmart/ancillary/aerosolSPF/Urban.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/ancillary/conifer_forest.csv` & `tmart-1.3.5/tmart/ancillary/conifer_forest.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/ancillary/dry_beach_sand.csv` & `tmart-1.3.5/tmart/ancillary/dry_beach_sand.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/ancillary/lawn_grass.csv` & `tmart-1.3.5/tmart/ancillary/lawn_grass.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/ancillary/soil.csv` & `tmart-1.3.5/tmart/ancillary/soil.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/ancillary/vegetation.csv` & `tmart-1.3.5/tmart/ancillary/vegetation.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/ancillary/water_chl1.csv` & `tmart-1.3.5/tmart/ancillary/water_chl1.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/ancillary/wet_beach_sand.csv` & `tmart-1.3.5/tmart/ancillary/wet_beach_sand.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/tm_OT.py` & `tmart-1.3.5/tmart/tm_OT.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/tm_calcref.py` & `tmart-1.3.5/tmart/tm_calcref.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/tm_geometry.py` & `tmart-1.3.5/tmart/tm_geometry.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/tm_intersect.py` & `tmart-1.3.5/tmart/tm_intersect.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/tm_move.py` & `tmart-1.3.5/tmart/tm_move.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/tm_sampling.py` & `tmart-1.3.5/tmart/tm_sampling.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart/tm_water.py` & `tmart-1.3.5/tmart/tm_water.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.3/tmart.egg-info/PKG-INFO` & `tmart-1.3.5/tmart.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmart
-Version: 1.3.3
+Version: 1.3.5
 Summary: Radiative transfer modelling for aquatic remote sensing
 Author: Yulun Wu
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # T-Mart: Topography-adjusted Monte-carlo Adjacency-effect Radiative Transfer Code
 
 ## Description 
 
-T-Mart solves the radiative transfer in a 3D ocean-atmosphere system through a Monte-Carlo approach. T-Mart features arbitrary surface models which allow simulating and correcting for the adjacnecy effect in aquatic remote sensing. 
+T-Mart solves the radiative transfer in a 3D surface-atmosphere system through a Monte-Carlo approach. T-Mart features arbitrary surface models which allow simulating and correcting for the adjacnecy effect in aquatic remote sensing. 
 
 
 ## Links
 
 
 Home page: <a href="https://github.com/yulunwu8/tmart" target="_blank">https://github.com/yulunwu8/tmart</a>
 
@@ -117,10 +117,11 @@
 
 ```
 
 
 
 ## Other
 
+T-Mart can calculate reflectances of various units, see Table 1 in Wu et al. (2023). 
 
 For questions and suggestions (which I'm always open to!), please email Yulun at [yulunwu8@gmail.com](mailto:yulunwu8@gmail.com)
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: tmart Version: 1.3.3 Summary: Radiative transfer
+Metadata-Version: 2.1 Name: tmart Version: 1.3.5 Summary: Radiative transfer
 modelling for aquatic remote sensing Author: Yulun Wu Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
 Atmospheric Science Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown # T-Mart: Topography-adjusted Monte-carlo Adjacency-effect
 Radiative Transfer Code ## Description T-Mart solves the radiative transfer in
-a 3D ocean-atmosphere system through a Monte-Carlo approach. T-Mart features
+a 3D surface-atmosphere system through a Monte-Carlo approach. T-Mart features
 arbitrary surface models which allow simulating and correcting for the
 adjacnecy effect in aquatic remote sensing. ## Links Home page: https://
 github.com/yulunwu8/tmart User guide: https://tmart-rtm.github.io ##
 Publication Wu, Y., Knudby, A., & Lapen, D. (2023). Topography-Adjusted Monte
 Carlo Simulation of the Adjacency Effect in Remote Sensing of Coastal and
 Inland Waters. *Journal of Quantitative Spectroscopy and Radiative Transfer*,
 108589. https://doi.org/10.1016/j.jqsrt.2023.108589 ## Installation 1 - Create
@@ -37,10 +37,11 @@
 v) ``` Output should be similar to this: ``` ========= Initiating T-Mart
 ========= Number of photons: 10000 Using 10 core(s) Number of job(s): 100
 Wavelength: 400 target_pt_direction: [180, 0] sun_dir: [0, 0]
 ===================================== Tasks remaining = 102 Tasks remaining =
 72 Tasks remaining = 42 Tasks remaining = 12
 ===================================== Calculating radiative properties... R_atm
 0.12760589889823587 R_dir 0.06046419017201067 R_env 0.012888590547129805
-R_total 0.20095867961737635 ``` ## Other For questions and suggestions (which
-I'm always open to!), please email Yulun at [yulunwu8@gmail.com](mailto:
+R_total 0.20095867961737635 ``` ## Other T-Mart can calculate reflectances of
+various units, see Table 1 in Wu et al. (2023). For questions and suggestions
+(which I'm always open to!), please email Yulun at [yulunwu8@gmail.com](mailto:
 yulunwu8@gmail.com)
```

### Comparing `tmart-1.3.3/tmart.egg-info/SOURCES.txt` & `tmart-1.3.5/tmart.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 tmart.egg-info/PKG-INFO
 tmart.egg-info/SOURCES.txt
 tmart.egg-info/dependency_links.txt
 tmart.egg-info/requires.txt
 tmart.egg-info/top_level.txt
 tmart/AEC/__init__.py
 tmart/AEC/get_parameters.py
+tmart/AEC/read_PRISMA_north.py
+tmart/AEC/read_PRISMA_vaa.py
 tmart/AEC/reflectance_correction.py
 tmart/ancillary/conifer_forest.csv
 tmart/ancillary/dry_beach_sand.csv
 tmart/ancillary/lawn_grass.csv
 tmart/ancillary/soil.csv
 tmart/ancillary/vegetation.csv
 tmart/ancillary/water.csv
```

