# Comparing `tmp/piq-0.7.0.tar.gz` & `tmp/piq-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piq-0.7.0.tar", last modified: Wed Apr 27 21:03:34 2022, max compression
+gzip compressed data, was "piq-0.7.1.tar", last modified: Tue Apr 18 17:47:37 2023, max compression
```

## Comparing `piq-0.7.0.tar` & `piq-0.7.1.tar`

### file list

```diff
@@ -1,82 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 21:03:34.461697 piq-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-27 21:03:26.000000 piq-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15629 2022-04-27 21:03:34.461697 piq-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15154 2022-04-27 21:03:26.000000 piq-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 21:03:34.453697 piq-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-27 21:03:26.000000 piq-0.7.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-04-27 21:03:26.000000 piq-0.7.0/examples/feature_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     8408 2022-04-27 21:03:26.000000 piq-0.7.0/examples/image_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 21:03:34.453697 piq-0.7.0/piq/
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-04-27 21:03:26.000000 piq-0.7.0/piq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2335 2022-04-27 21:03:26.000000 piq-0.7.0/piq/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    11329 2022-04-27 21:03:26.000000 piq-0.7.0/piq/brisque.py
--rw-r--r--   0 runner    (1001) docker     (121)    11860 2022-04-27 21:03:26.000000 piq-0.7.0/piq/dss.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 21:03:34.457697 piq-0.7.0/piq/feature_extractors/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-04-27 21:03:26.000000 piq-0.7.0/piq/feature_extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12615 2022-04-27 21:03:26.000000 piq-0.7.0/piq/feature_extractors/fid_inception.py
--rw-r--r--   0 runner    (1001) docker     (121)     6770 2022-04-27 21:03:26.000000 piq-0.7.0/piq/fid.py
--rw-r--r--   0 runner    (1001) docker     (121)    19546 2022-04-27 21:03:26.000000 piq-0.7.0/piq/fsim.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 21:03:34.457697 piq-0.7.0/piq/functional/
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-04-27 21:03:26.000000 piq-0.7.0/piq/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3879 2022-04-27 21:03:26.000000 piq-0.7.0/piq/functional/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4992 2022-04-27 21:03:26.000000 piq-0.7.0/piq/functional/colour_conversion.py
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-04-27 21:03:26.000000 piq-0.7.0/piq/functional/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-04-27 21:03:26.000000 piq-0.7.0/piq/functional/layers.py
--rw-r--r--   0 runner    (1001) docker     (121)    12631 2022-04-27 21:03:26.000000 piq-0.7.0/piq/functional/resize.py
--rw-r--r--   0 runner    (1001) docker     (121)    11727 2022-04-27 21:03:26.000000 piq-0.7.0/piq/gmsd.py
--rw-r--r--   0 runner    (1001) docker     (121)     9624 2022-04-27 21:03:26.000000 piq-0.7.0/piq/gs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8043 2022-04-27 21:03:26.000000 piq-0.7.0/piq/haarpsi.py
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-04-27 21:03:26.000000 piq-0.7.0/piq/isc.py
--rw-r--r--   0 runner    (1001) docker     (121)    19632 2022-04-27 21:03:26.000000 piq-0.7.0/piq/iw_ssim.py
--rw-r--r--   0 runner    (1001) docker     (121)     8341 2022-04-27 21:03:26.000000 piq-0.7.0/piq/kid.py
--rw-r--r--   0 runner    (1001) docker     (121)     9019 2022-04-27 21:03:26.000000 piq-0.7.0/piq/mdsi.py
--rw-r--r--   0 runner    (1001) docker     (121)    13895 2022-04-27 21:03:26.000000 piq-0.7.0/piq/ms_ssim.py
--rw-r--r--   0 runner    (1001) docker     (121)    15134 2022-04-27 21:03:26.000000 piq-0.7.0/piq/msid.py
--rw-r--r--   0 runner    (1001) docker     (121)    20112 2022-04-27 21:03:26.000000 piq-0.7.0/piq/perceptual.py
--rw-r--r--   0 runner    (1001) docker     (121)     8828 2022-04-27 21:03:26.000000 piq-0.7.0/piq/pieapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     4752 2022-04-27 21:03:26.000000 piq-0.7.0/piq/pr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-04-27 21:03:26.000000 piq-0.7.0/piq/psnr.py
--rw-r--r--   0 runner    (1001) docker     (121)    11359 2022-04-27 21:03:26.000000 piq-0.7.0/piq/srsim.py
--rw-r--r--   0 runner    (1001) docker     (121)    12516 2022-04-27 21:03:26.000000 piq-0.7.0/piq/ssim.py
--rw-r--r--   0 runner    (1001) docker     (121)     3549 2022-04-27 21:03:26.000000 piq-0.7.0/piq/tv.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 21:03:34.457697 piq-0.7.0/piq/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-04-27 21:03:26.000000 piq-0.7.0/piq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5375 2022-04-27 21:03:26.000000 piq-0.7.0/piq/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     6845 2022-04-27 21:03:26.000000 piq-0.7.0/piq/vif.py
--rw-r--r--   0 runner    (1001) docker     (121)    10912 2022-04-27 21:03:26.000000 piq-0.7.0/piq/vsi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 21:03:34.457697 piq-0.7.0/piq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15629 2022-04-27 21:03:34.000000 piq-0.7.0/piq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-04-27 21:03:34.000000 piq-0.7.0/piq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-27 21:03:34.000000 piq-0.7.0/piq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-04-27 21:03:34.000000 piq-0.7.0/piq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-04-27 21:03:34.000000 piq-0.7.0/piq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-27 21:03:34.461697 piq-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-04-27 21:03:26.000000 piq-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 21:03:34.461697 piq-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-27 21:03:26.000000 piq-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-04-27 21:03:26.000000 piq-0.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    16858 2022-04-27 21:03:26.000000 piq-0.7.0/tests/results_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (121)     4382 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_brisque.py
--rw-r--r--   0 runner    (1001) docker     (121)     7370 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_dss.py
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)     2494 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_fid.py
--rw-r--r--   0 runner    (1001) docker     (121)     6152 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_fsim.py
--rw-r--r--   0 runner    (1001) docker     (121)    11096 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_gmsd.py
--rw-r--r--   0 runner    (1001) docker     (121)     2655 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_gs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4593 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_haarpsi.py
--rw-r--r--   0 runner    (1001) docker     (121)     4474 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_is.py
--rw-r--r--   0 runner    (1001) docker     (121)    11947 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_iw_ssim.py
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_kid.py
--rw-r--r--   0 runner    (1001) docker     (121)     5004 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_mdsi.py
--rw-r--r--   0 runner    (1001) docker     (121)     9826 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_ms_ssim.py
--rw-r--r--   0 runner    (1001) docker     (121)     3525 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_msid.py
--rw-r--r--   0 runner    (1001) docker     (121)     8694 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_perceptual.py
--rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_pieapp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_pr.py
--rw-r--r--   0 runner    (1001) docker     (121)     4086 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_psnr.py
--rw-r--r--   0 runner    (1001) docker     (121)     7909 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_srsim.py
--rw-r--r--   0 runner    (1001) docker     (121)    11695 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_ssim.py
--rw-r--r--   0 runner    (1001) docker     (121)     1686 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_tv.py
--rw-r--r--   0 runner    (1001) docker     (121)     4749 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5323 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_vif.py
--rw-r--r--   0 runner    (1001) docker     (121)     3466 2022-04-27 21:03:26.000000 piq-0.7.0/tests/test_vsi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:47:37.079668 piq-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 17:47:25.000000 piq-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-04-18 17:47:37.079668 piq-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-04-18 17:47:25.000000 piq-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:47:37.075668 piq-0.7.1/piq/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-18 17:47:25.000000 piq-0.7.1/piq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-18 17:47:25.000000 piq-0.7.1/piq/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-04-18 17:47:25.000000 piq-0.7.1/piq/brisque.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-04-18 17:47:25.000000 piq-0.7.1/piq/dss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:47:37.075668 piq-0.7.1/piq/feature_extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-18 17:47:25.000000 piq-0.7.1/piq/feature_extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-04-18 17:47:25.000000 piq-0.7.1/piq/feature_extractors/fid_inception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-04-18 17:47:25.000000 piq-0.7.1/piq/fid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-04-18 17:47:25.000000 piq-0.7.1/piq/fsim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:47:37.075668 piq-0.7.1/piq/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-18 17:47:25.000000 piq-0.7.1/piq/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-18 17:47:25.000000 piq-0.7.1/piq/functional/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-18 17:47:25.000000 piq-0.7.1/piq/functional/colour_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-18 17:47:25.000000 piq-0.7.1/piq/functional/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-18 17:47:25.000000 piq-0.7.1/piq/functional/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-18 17:47:25.000000 piq-0.7.1/piq/functional/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-04-18 17:47:25.000000 piq-0.7.1/piq/gmsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-18 17:47:25.000000 piq-0.7.1/piq/gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-04-18 17:47:25.000000 piq-0.7.1/piq/haarpsi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-18 17:47:25.000000 piq-0.7.1/piq/isc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19736 2023-04-18 17:47:25.000000 piq-0.7.1/piq/iw_ssim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-18 17:47:25.000000 piq-0.7.1/piq/kid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-04-18 17:47:25.000000 piq-0.7.1/piq/mdsi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-04-18 17:47:25.000000 piq-0.7.1/piq/ms_ssim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-04-18 17:47:25.000000 piq-0.7.1/piq/msid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20112 2023-04-18 17:47:25.000000 piq-0.7.1/piq/perceptual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-18 17:47:25.000000 piq-0.7.1/piq/pieapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-18 17:47:25.000000 piq-0.7.1/piq/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-18 17:47:25.000000 piq-0.7.1/piq/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-04-18 17:47:25.000000 piq-0.7.1/piq/srsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-04-18 17:47:25.000000 piq-0.7.1/piq/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-18 17:47:25.000000 piq-0.7.1/piq/tv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:47:37.075668 piq-0.7.1/piq/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-18 17:47:25.000000 piq-0.7.1/piq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-18 17:47:25.000000 piq-0.7.1/piq/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-04-18 17:47:25.000000 piq-0.7.1/piq/vif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-04-18 17:47:25.000000 piq-0.7.1/piq/vsi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:47:37.075668 piq-0.7.1/piq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-04-18 17:47:37.000000 piq-0.7.1/piq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-18 17:47:37.000000 piq-0.7.1/piq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:47:37.000000 piq-0.7.1/piq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 17:47:37.000000 piq-0.7.1/piq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-18 17:47:37.000000 piq-0.7.1/piq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 17:47:37.079668 piq-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-18 17:47:25.000000 piq-0.7.1/setup.py
```

### Comparing `piq-0.7.0/LICENSE` & `piq-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `piq-0.7.0/PKG-INFO` & `piq-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: piq
-Version: 0.7.0
+Version: 0.7.1
 Summary: Measures and metrics for image2image tasks. PyTorch.
 Home-page: https://github.com/photosynthesis-team/piq
 Author: Sergey Kastryulin
 Author-email: snk4tr@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
@@ -51,18 +49,18 @@
 The library contains a set of measures and metrics that is continually getting extended.
 For measures/metrics that can be used as loss functions, corresponding PyTorch modules are implemented.
 
 We provide:
 
 * Unified interface, which is easy to use and extend.
 * Written on pure PyTorch with bare minima of additional dependencies.
-* Extensive user input validation. You code will not crash in the middle of the training.
+* Extensive user input validation. Your code will not crash in the middle of the training.
 * Fast (GPU computations available) and reliable.
 * Most metrics can be backpropagated for model optimization.
-* Supports python 3.6-3.8.
+* Supports python 3.7-3.10.
 
 PIQ was initially named `PhotoSynthesis.Metrics <https://pypi.org/project/photosynthesis-metrics/0.4.0/>`_.
 
 .. intro-section-end
 
 .. installation-section-start
 
@@ -330,20 +328,31 @@
 
 Citation
 --------
 If you use PIQ in your project, please, cite it as follows.
 
 .. code-block:: tex
 
+   @misc{kastryulin2022piq,
+     title = {PyTorch Image Quality: Metrics for Image Quality Assessment},
+     url = {https://arxiv.org/abs/2208.14818},
+     author = {Kastryulin, Sergey and Zakirov, Jamil and Prokopenko, Denis and Dylov, Dmitry V.},
+     doi = {10.48550/ARXIV.2208.14818},
+     publisher = {arXiv},
+     year = {2022}
+   }
+
+.. code-block:: tex
+
    @misc{piq,
      title={{PyTorch Image Quality}: Metrics and Measure for Image Quality Assessment},
      url={https://github.com/photosynthesis-team/piq},
      note={Open-source software available at https://github.com/photosynthesis-team/piq},
      author={Sergey Kastryulin and Dzhamil Zakirov and Denis Prokopenko},
-     year={2019},
+     year={2019}
    }
 
 .. citation-section-end
 
 .. contacts-section-start
 
 Contacts
@@ -352,9 +361,7 @@
 **Sergey Kastryulin** - `@snk4tr <https://github.com/snk4tr>`_ - ``snk4tr@gmail.com``
 
 **Jamil Zakirov** - `@zakajd <https://github.com/zakajd>`_ - ``djamilzak@gmail.com``
 
 **Denis Prokopenko** - `@denproc <https://github.com/denproc>`_ - ``d.prokopenko@outlook.com``
 
 .. contacts-section-end
-
-
```

### Comparing `piq-0.7.0/README.rst` & `piq-0.7.1/piq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: piq
+Version: 0.7.1
+Summary: Measures and metrics for image2image tasks. PyTorch.
+Home-page: https://github.com/photosynthesis-team/piq
+Author: Sergey Kastryulin
+Author-email: snk4tr@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 
 .. image:: https://raw.githubusercontent.com/photosynthesis-team/piq/master/docs/source/_static/piq_logo_main.png
     :target: https://github.com/photosynthesis-team/piq
 
 ..
 
   PyTorch Image Quality (PIQ) is not endorsed by Facebook, Inc.;
@@ -36,18 +49,18 @@
 The library contains a set of measures and metrics that is continually getting extended.
 For measures/metrics that can be used as loss functions, corresponding PyTorch modules are implemented.
 
 We provide:
 
 * Unified interface, which is easy to use and extend.
 * Written on pure PyTorch with bare minima of additional dependencies.
-* Extensive user input validation. You code will not crash in the middle of the training.
+* Extensive user input validation. Your code will not crash in the middle of the training.
 * Fast (GPU computations available) and reliable.
 * Most metrics can be backpropagated for model optimization.
-* Supports python 3.6-3.8.
+* Supports python 3.7-3.10.
 
 PIQ was initially named `PhotoSynthesis.Metrics <https://pypi.org/project/photosynthesis-metrics/0.4.0/>`_.
 
 .. intro-section-end
 
 .. installation-section-start
 
@@ -315,20 +328,31 @@
 
 Citation
 --------
 If you use PIQ in your project, please, cite it as follows.
 
 .. code-block:: tex
 
+   @misc{kastryulin2022piq,
+     title = {PyTorch Image Quality: Metrics for Image Quality Assessment},
+     url = {https://arxiv.org/abs/2208.14818},
+     author = {Kastryulin, Sergey and Zakirov, Jamil and Prokopenko, Denis and Dylov, Dmitry V.},
+     doi = {10.48550/ARXIV.2208.14818},
+     publisher = {arXiv},
+     year = {2022}
+   }
+
+.. code-block:: tex
+
    @misc{piq,
      title={{PyTorch Image Quality}: Metrics and Measure for Image Quality Assessment},
      url={https://github.com/photosynthesis-team/piq},
      note={Open-source software available at https://github.com/photosynthesis-team/piq},
      author={Sergey Kastryulin and Dzhamil Zakirov and Denis Prokopenko},
-     year={2019},
+     year={2019}
    }
 
 .. citation-section-end
 
 .. contacts-section-start
 
 Contacts
```

### Comparing `piq-0.7.0/piq/__init__.py` & `piq-0.7.1/piq/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 from .ssim import ssim, SSIMLoss
 from .ms_ssim import multi_scale_ssim, MultiScaleSSIMLoss
 from .msid import MSID
 from .fid import FID
 from .kid import KID
 from .pr import PR
```

### Comparing `piq-0.7.0/piq/base.py` & `piq-0.7.1/piq/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,34 +25,40 @@
         Args:
             loader: Should return dict with key `images` in it
             feature_extractor: model used to generate image features, if None use `InceptionNetV3` model.
                 Model should return a list with features from one of the network layers.
             out_features: size of `feature_extractor` output
             device: Device on which to compute inference of the model
         """
-
         if feature_extractor is None:
             print('WARNING: default feature extractor (InceptionNet V2) is used.')
             feature_extractor = InceptionV3()
         else:
             assert isinstance(feature_extractor, torch.nn.Module), \
                 f"Feature extractor must be PyTorch module. Got {type(feature_extractor)}"
+
         feature_extractor.to(device)
         feature_extractor.eval()
 
         total_feats = []
         for batch in loader:
             images = batch['images']
             N = images.shape[0]
             images = images.float().to(device)
 
             # Get features
             features = feature_extractor(images)
             # TODO(jamil 26.03.20): Add support for more than one feature map
             assert len(features) == 1, \
                 f"feature_encoder must return list with features from one layer. Got {len(features)}"
-            total_feats.append(features[0].view(N, -1))
 
+            features = features[0].view(N, -1)
+            features = features.cpu()
+            total_feats.append(features)
+            torch.cuda.empty_cache()
+
+        feature_extractor.cpu()
+        torch.cuda.empty_cache()
         return torch.cat(total_feats, dim=0)
 
     def compute_metric(self, x_features: torch.Tensor, y_features: torch.Tensor) -> torch.Tensor:
         raise NotImplementedError("This function should be defined for each children class")
```

### Comparing `piq-0.7.0/piq/brisque.py` & `piq-0.7.1/piq/brisque.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     indexes = (ro_hat_norm - r_table).abs().argmin(dim=-1)
     solution = gamma[indexes]
     return solution, left_sigma.squeeze(dim=-1), right_sigma.squeeze(dim=-1)
 
 
 def _natural_scene_statistics(luma: torch.Tensor, kernel_size: int = 7, sigma: float = 7. / 6) -> torch.Tensor:
     kernel = gaussian_filter(kernel_size=kernel_size,
-                             sigma=sigma, dtype=luma.dtype).view(1, 1, kernel_size, kernel_size).to(luma)
+                             sigma=sigma, dtype=luma.dtype, device=luma.device).view(1, 1, kernel_size, kernel_size)
     C = 1
     mu = F.conv2d(luma, kernel, padding=kernel_size // 2)
     mu_sq = mu ** 2
     std = F.conv2d(luma ** 2, kernel, padding=kernel_size // 2)
     std = (std - mu_sq).abs().sqrt()
 
     luma_nrmlzd = (luma - mu) / (std + C)
@@ -205,18 +205,18 @@
                                    [0.244, 1.641], [-0.123586, 0.179083], [0.000152, 0.710456],
                                    [0.000975, 0.470984], [0.249, 1.555], [-0.135687, 0.100858],
                                    [0.000174, 0.684173], [0.000913, 0.534174], [0.258, 1.561],
                                    [-0.143408, 0.100486], [0.000179, 0.685696], [0.000888, 0.536508],
                                    [0.471, 3.264], [0.012809, 0.703171], [0.218, 1.046],
                                    [-0.094876, 0.187459], [1.5e-005, 0.442057], [0.001272, 0.40803],
                                    [0.222, 1.042], [-0.115772, 0.162604], [1.6e-005, 0.444362],
-                                   [0.001374, 0.40243], [0.227, 0.996],
-                                   [-0.117188, 0.09832299999999999], [3e-005, 0.531903],
-                                   [0.001122, 0.369589], [0.228, 0.99], [-0.12243, 0.098658],
-                                   [2.8e-005, 0.530092], [0.001118, 0.370399]]).to(features)
+                                   [0.001374, 0.40243], [0.227, 0.996], [-0.117188, 0.09832299999999999],
+                                   [3e-005, 0.531903], [0.001122, 0.369589], [0.228, 0.99], [-0.12243, 0.098658],
+                                   [2.8e-005, 0.530092],
+                                   [0.001118, 0.370399]], device=features.device, dtype=features.dtype)
 
     scaled_features = lower_bound + (upper_bound - lower_bound) * (features - feature_ranges[..., 0]) / (
             feature_ranges[..., 1] - feature_ranges[..., 0])
 
     return scaled_features
 
 
@@ -232,9 +232,9 @@
 
     # gamma and rho are SVM model parameters taken from official implementation of BRISQUE on MATLAB
     # Source: https://live.ece.utexas.edu/research/Quality/index_algorithms.htm
     gamma = 0.05
     rho = -153.591
     sv.t_()
     kernel_features = _rbf_kernel(features=features, sv=sv, gamma=gamma)
-    score = kernel_features @ sv_coef.to(dtype=features.dtype)
+    score = kernel_features @ sv_coef.type(features.dtype)
     return score - rho
```

### Comparing `piq-0.7.0/piq/dss.py` & `piq-0.7.1/piq/dss.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 import math
 import functools
 import torch
 
 import torch.nn.functional as F
 
-from typing import Union
+from typing import Union, Optional
 from torch.nn.modules.loss import _Loss
 
 from piq.utils import _validate_input, _reduce
 from piq.functional import gaussian_filter, rgb2yiq
 
 
 def dss(x: torch.Tensor, y: torch.Tensor, reduction: str = 'mean',
@@ -80,15 +80,15 @@
     y_lum = y_lum[:, :, 0:rows, 0:cols]
 
     # Channel decomposition for both images by `dct_size`x`dct_size` 2D DCT
     dct_x = _dct_decomp(x_lum, dct_size)
     dct_y = _dct_decomp(y_lum, dct_size)
 
     # Create a Gaussian window that will be used to weight subbands scores
-    coords = torch.arange(1, dct_size + 1).to(x)
+    coords = torch.arange(1, dct_size + 1, dtype=x.dtype, device=x.device)
     weight = (coords - 0.5) ** 2
     weight = (- (weight.unsqueeze(0) + weight.unsqueeze(1)) / (2 * sigma_weight ** 2)).exp()
 
     # Compute similarity between each subband in img1 and img2
     subband_sim_matrix = torch.zeros((x.size(0), dct_size, dct_size), device=x.device)
     threshold = 1e-2
     for m in range(dct_size):
@@ -131,16 +131,16 @@
         This implementation is based on the original MATLAB code (see header).
     """
     # `c` takes value of DC or AC coefficient depending on stage
     dc_coeff, ac_coeff = (1000, 300)
     c = dc_coeff if first_term else ac_coeff
 
     # Compute local variance
-    kernel = gaussian_filter(kernel_size=kernel_size, sigma=sigma)
-    kernel = kernel.view(1, 1, kernel_size, kernel_size).to(x)
+    kernel = gaussian_filter(kernel_size=kernel_size, sigma=sigma, dtype=x.dtype, device=x.device)
+    kernel = kernel.view(1, 1, kernel_size, kernel_size)
     mu_x = F.conv2d(x, kernel, padding=kernel_size // 2)
     mu_y = F.conv2d(y, kernel, padding=kernel_size // 2)
 
     sigma_xx = F.conv2d(x * x, kernel, padding=kernel_size // 2) - mu_x ** 2
     sigma_yy = F.conv2d(y * y, kernel, padding=kernel_size // 2) - mu_y ** 2
 
     sigma_xx[sigma_xx < 0] = 0
@@ -158,25 +158,27 @@
         right_term = ((sigma_xy + c) / (torch.sqrt(sigma_xx * sigma_yy) + c))
         sorted_right = torch.sort(right_term.flatten(start_dim=1)).values
         similarity *= torch.mean(sorted_right[:, :percentile_index], dim=1)
 
     return similarity
 
 
-def _dct_matrix(size: int) -> torch.Tensor:
+def _dct_matrix(size: int, device: Optional[str] = None, dtype: Optional[type] = None) -> torch.Tensor:
     r""" Computes the matrix coefficients for DCT transform using the following formula:
     https://fr.mathworks.com/help/images/discrete-cosine-transform.html
 
     Args:
-       size : size of DCT matrix to create.  (`size`, `size`)
+        size : size of DCT matrix to create.  (`size`, `size`)
+        device: target device for generation
+        dtype: target data type for generation
     """
-    p = torch.arange(1, size).reshape((size - 1, 1))
-    q = torch.arange(1, 2 * size, 2)
+    p = torch.arange(1, size, device=device, dtype=dtype).reshape((size - 1, 1))
+    q = torch.arange(1, 2 * size, 2, device=device, dtype=dtype)
     return torch.cat((
-        math.sqrt(1 / size) * torch.ones((1, size)),
+        math.sqrt(1 / size) * torch.ones((1, size), device=device, dtype=dtype),
         math.sqrt(2 / size) * torch.cos(math.pi / (2 * size) * p * q)), 0)
 
 
 def _dct_decomp(x: torch.Tensor, dct_size: int = 8) -> torch.Tensor:
     r""" Computes 2D Discrete Cosine Transform on 8x8 blocks of an image
 
     Args:
@@ -192,15 +194,15 @@
 
     # make NxN blocks out of image
     blocks = F.unfold(x, kernel_size=(dct_size, dct_size), stride=(dct_size, dct_size))  # shape (1, NxN, block_num)
     blocks = blocks.transpose(1, 2)
     blocks = blocks.view(bs, 1, -1, dct_size, dct_size)  # shape (bs, 1, block_num, N, N)
 
     # apply DCT transform
-    coeffs = _dct_matrix(dct_size).to(x)
+    coeffs = _dct_matrix(dct_size, device=x.device, dtype=x.dtype)
 
     blocks = coeffs @ blocks @ coeffs.t()  # @ does operation on last 2 channels only
 
     # Reconstruct image
     blocks = blocks.reshape(bs, -1, dct_size ** 2)
     blocks = blocks.transpose(1, 2)
     blocks = F.fold(blocks, output_size=x.size()[-2:], kernel_size=(dct_size, dct_size), stride=(dct_size, dct_size))
```

### Comparing `piq-0.7.0/piq/feature_extractors/fid_inception.py` & `piq-0.7.1/piq/feature_extractors/fid_inception.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
         Returns:
             List of torch.autograd.Variable, corresponding to the selected output block, sorted ascending by index.
         """
         outp = []
         input_range = (0, 1) if self.normalize_input else (-1, 1)
         assert (x.min() >= input_range[0]) and (x.max() <= input_range[1]), \
-            f"Input tensor should be normalized in ({input_range[0]}, {input_range[0]}) range."
+            f"Input tensor should be normalized in ({input_range[0]}, {input_range[1]}) range."
 
         if self.resize_input:
             x = F.interpolate(x,
                               size=(299, 299),
                               mode='bilinear',
                               align_corners=False)
```

### Comparing `piq-0.7.0/piq/fid.py` & `piq-0.7.1/piq/fid.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.0/piq/fsim.py` & `piq-0.7.1/piq/fsim.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Code is based on MATLAB version for computations in pixel domain
 https://www4.comp.polyu.edu.hk/~cslzhang/IQA/FSIM/Files/FeatureSIM.m
 References:
     https://www4.comp.polyu.edu.hk/~cslzhang/IQA/TIP_IQA_FSIM.pdf
 """
 import math
 import functools
-from typing import Union, Tuple
+from typing import Union
 
 import torch
 from torch.nn.modules.loss import _Loss
 
 from piq.utils import _validate_input, _reduce, _parse_version
 from piq.functional import ifftshift, get_meshgrid, similarity_map, gradient_map, scharr_filter, rgb2yiq
 
@@ -80,28 +80,24 @@
         x_q = x_yiq[:, 2:]
         y_q = y_yiq[:, 2:]
 
     else:
         x_lum = x
         y_lum = y
 
+    # Compute filters
+    filters = _construct_filters(x_lum, scales, orientations, min_length, mult, sigma_f, delta_theta)
+
     # Compute phase congruency maps
-    pc_x = _phase_congruency(
-        x_lum, scales=scales, orientations=orientations,
-        min_length=min_length, mult=mult, sigma_f=sigma_f,
-        delta_theta=delta_theta, k=k
-    )
-    pc_y = _phase_congruency(
-        y_lum, scales=scales, orientations=orientations,
-        min_length=min_length, mult=mult, sigma_f=sigma_f,
-        delta_theta=delta_theta, k=k
-    )
+    pc_x = _phase_congruency(x_lum, filters=filters, scales=scales, orientations=orientations, k=k)
+    pc_y = _phase_congruency(y_lum, filters=filters, scales=scales, orientations=orientations, k=k)
 
     # Gradient maps
-    kernels = torch.stack([scharr_filter(), scharr_filter().transpose(-1, -2)])
+    sch_filter = scharr_filter(device=x_lum.device, dtype=x_lum.dtype)
+    kernels = torch.stack([sch_filter, sch_filter.transpose(-1, -2)])
     grad_map_x = gradient_map(x_lum, kernels)
     grad_map_y = gradient_map(y_lum, kernels)
 
     # Constants from the paper
     T1, T2, T3, T4, lmbda = 0.85, 160, 200, 200, 0.03
 
     # Compute FSIM
@@ -119,49 +115,57 @@
         # score = score * torch.real((S_I * S_Q).to(torch.complex64) ** lmbda)
 
     result = score.sum(dim=[1, 2, 3]) / pc_max.sum(dim=[1, 2, 3])
 
     return _reduce(result, reduction)
 
 
-def _construct_filters(x: torch.Tensor, scales: int = 4, orientations: int = 4,
-                       min_length: int = 6, mult: int = 2, sigma_f: float = 0.55,
-                       delta_theta: float = 1.2, k: float = 2.0):
+def _construct_filters(x: torch.Tensor, scales: int = 4, orientations: int = 4, min_length: int = 6,
+                       mult: int = 2, sigma_f: float = 0.55, delta_theta: float = 1.2):
     """Creates a stack of filters used for computation of phase congruensy maps
 
     Args:
         x: Tensor. Shape :math:`(N, 1, H, W)`.
         scales: Number of wavelets
         orientations: Number of filter orientations
         min_length: Wavelength of smallest scale filter
         mult: Scaling factor between successive filters
         sigma_f: Ratio of the standard deviation of the Gaussian
             describing the log Gabor filter's transfer function
             in the frequency domain to the filter center frequency.
         delta_theta: Ratio of angular interval between filter orientations
             and the standard deviation of the angular Gaussian function
             used to construct filters in the freq. plane.
-        k: No of standard deviations of the noise energy beyond the mean
-            at which we set the noise threshold point, below which phase
-            congruency values get penalized.
-        """
+    Returns:
+          Tensor with filters. Shape :math:`(1, scales * orientations, H, W)`
+    """
     N, _, H, W = x.shape
 
     # Calculate the standard deviation of the angular Gaussian function
     # used to construct filters in the freq. plane.
     theta_sigma = math.pi / (orientations * delta_theta)
 
     # Pre-compute some stuff to speed up filter construction
-    grid_x, grid_y = get_meshgrid((H, W))
+    grid_x, grid_y = get_meshgrid((H, W), device=x.device, dtype=x.dtype)
 
-    # Move grid to GPU early on, so that all math heavy stuff computes faster.
-    grid_x, grid_y = grid_x.to(x), grid_y.to(x)
     radius = torch.sqrt(grid_x ** 2 + grid_y ** 2)
     theta = torch.atan2(-grid_y, grid_x)
 
+    # First construct a low-pass filter that is as large as possible, yet falls
+    # away to zero at the boundaries.  All log Gabor filters are multiplied by
+    # this to ensure no extra frequencies at the 'corners' of the FFT are
+    # incorporated as this seems to upset the normalisation process when
+    # Computed explicitly without _lowpassfilter
+    # Explicit low pass filter computation
+    n = 15  # default parameter
+    cutoff = .45  # default parameter
+    assert 0 < cutoff <= 0.5, "Cutoff frequency must be between 0 and 0.5"
+    assert n > 1 and int(n) == n, "n must be an integer >= 1"
+    lp = ifftshift(1. / (1.0 + (radius / cutoff) ** (2 * n)))
+
     # Quadrant shift radius and theta so that filters are constructed with 0 frequency at the corners.
     # Get rid of the 0 radius value at the 0 frequency point (now at top-left corner)
     # so that taking the log of the radius will not cause trouble.
     radius = ifftshift(radius)
     theta = ifftshift(theta)
     radius[0, 0] = 1
 
@@ -169,30 +173,26 @@
     costheta = torch.cos(theta)
 
     # Filters are constructed in terms of two components.
     # 1) The radial component, which controls the frequency band that the filter responds to
     # 2) The angular component, which controls the orientation that the filter responds to.
     # The two components are multiplied together to construct the overall filter.
 
-    # First construct a low-pass filter that is as large as possible, yet falls
-    # away to zero at the boundaries.  All log Gabor filters are multiplied by
-    # this to ensure no extra frequencies at the 'corners' of the FFT are
-    # incorporated as this seems to upset the normalisation process when
-    lp = _lowpassfilter(size=(H, W), cutoff=.45, n=15).to(x)
-
     # Construct the radial filter components...
     log_gabor = []
     for s in range(scales):
         wavelength = min_length * mult ** s
         omega_0 = 1.0 / wavelength
         gabor_filter = torch.exp((- torch.log(radius / omega_0) ** 2) / (2 * math.log(sigma_f) ** 2))
         gabor_filter = gabor_filter * lp
         gabor_filter[0, 0] = 0
         log_gabor.append(gabor_filter)
 
+    log_gabor = torch.stack(log_gabor)
+
     # Then construct the angular filter components...
     spread = []
     for o in range(orientations):
         angl = o * math.pi / orientations
 
         # For each point in the filter matrix calculate the angular distance from
         # the specified filter orientation.  To overcome the angular wrap-around
@@ -200,52 +200,42 @@
         # and then the atan2 function is used to determine angular distance.
         ds = sintheta * math.cos(angl) - costheta * math.sin(angl)  # Difference in sine.
         dc = costheta * math.cos(angl) + sintheta * math.sin(angl)  # Difference in cosine.
         dtheta = torch.abs(torch.atan2(ds, dc))
         spread.append(torch.exp((- dtheta ** 2) / (2 * theta_sigma ** 2)))
 
     spread = torch.stack(spread)
-    log_gabor = torch.stack(log_gabor)
 
     # Multiply, add batch dimension and transfer to correct device.
     filters = (spread.repeat_interleave(scales, dim=0) * log_gabor.repeat(orientations, 1, 1)).unsqueeze(0)
     return filters
 
 
-def _phase_congruency(x: torch.Tensor, scales: int = 4, orientations: int = 4,
-                      min_length: int = 6, mult: int = 2, sigma_f: float = 0.55,
-                      delta_theta: float = 1.2, k: float = 2.0) -> torch.Tensor:
+def _phase_congruency(x: torch.Tensor, filters: torch.Tensor, scales: int = 4, orientations: int = 4,
+                      k: float = 2.0) -> torch.Tensor:
     r"""Compute Phase Congruence for a batch of greyscale images
 
     Args:
         x: Tensor. Shape :math:`(N, 1, H, W)`.
+        filters: Kernels to extract features.
         scales: Number of wavelet scales
         orientations: Number of filter orientations
-        min_length: Wavelength of smallest scale filter
-        mult: Scaling factor between successive filters
-        sigma_f: Ratio of the standard deviation of the Gaussian
-            describing the log Gabor filter's transfer function
-            in the frequency domain to the filter center frequency.
-        delta_theta: Ratio of angular interval between filter orientations
-            and the standard deviation of the angular Gaussian function
-            used to construct filters in the freq. plane.
         k: No of standard deviations of the noise energy beyond the mean
             at which we set the noise threshold point, below which phase
             congruency values get penalized.
 
     Returns:
         Phase Congruency map with shape :math:`(N, H, W)`
 
     """
     EPS = torch.finfo(x.dtype).eps
 
     N, _, H, W = x.shape
 
     # Fourier transform
-    filters = _construct_filters(x, scales, orientations, min_length, mult, sigma_f, delta_theta, k)
     recommended_torch_version = _parse_version('1.8.0')
     torch_version = _parse_version(torch.__version__)
     if len(torch_version) != 0 and torch_version >= recommended_torch_version:
         imagefft = torch.fft.fft2(x)
         filters_ifft = torch.fft.ifft2(filters)
         filters_ifft = filters_ifft.real * math.sqrt(H * W)
         even_odd = torch.view_as_real(torch.fft.ifft2(imagefft * filters)).view(N, orientations, scales, H, W, 2)
@@ -304,15 +294,15 @@
 
     # Now estimate the total energy^2 due to noise
     # Estimate for sum(An^2) + sum(Ai.*Aj.*(cphi.*cphj + sphi.*sphj))
     filters_ifft = filters_ifft.view(1, orientations, scales, H, W)
 
     sum_an2 = torch.sum(filters_ifft ** 2, dim=-3, keepdim=True)
 
-    sum_ai_aj = torch.zeros(N, orientations, 1, H, W).to(x)
+    sum_ai_aj = torch.zeros(N, orientations, 1, H, W, dtype=x.dtype, device=x.device)
     for s in range(scales - 1):
         sum_ai_aj = sum_ai_aj + (filters_ifft[:, :, s: s + 1] * filters_ifft[:, :, s + 1:]).sum(dim=-3, keepdim=True)
 
     sum_an2 = torch.sum(sum_an2, dim=[-1, -2], keepdim=True)
     sum_ai_aj = torch.sum(sum_ai_aj, dim=[-1, -2], keepdim=True)
 
     noise_energy2 = 2 * noise_power * sum_an2 + 4 * noise_power * sum_ai_aj
@@ -334,49 +324,20 @@
 
     # Empirical rescaling of the estimated noise effect to suit the PC_2 phase congruency measure
     T = T / 1.7
 
     # Apply noise threshold
     energy = torch.max(energy - T, torch.zeros_like(T))
 
-    eps = torch.finfo(energy.dtype).eps
-    energy_all = energy.sum(dim=[1, 2]) + eps
-    an_all = an.sum(dim=[1, 2]) + eps
+    energy_all = energy.sum(dim=[1, 2]) + EPS
+    an_all = an.sum(dim=[1, 2]) + EPS
     result_pc = energy_all / an_all
     return result_pc.unsqueeze(1)
 
 
-def _lowpassfilter(size: Tuple[int, int], cutoff: float, n: int) -> torch.Tensor:
-    r"""
-    Constructs a low-pass Butterworth filter.
-
-    Args:
-        size: Tuple with height and width of filter to construct
-        cutoff: Cutoff frequency of the filter in (0, 0.5()
-        n: Filter order. Higher `n` means sharper transition.
-            Note that `n` is doubled so that it is always an even integer.
-
-    Returns:
-        f = 1 / (1 + w/cutoff) ^ 2n
-
-    Note:
-        The frequency origin of the returned filter is at the corners.
-
-    """
-    assert 0 < cutoff <= 0.5, "Cutoff frequency must be between 0 and 0.5"
-    assert n > 1 and int(n) == n, "n must be an integer >= 1"
-
-    grid_x, grid_y = get_meshgrid(size)
-
-    # A matrix with every pixel = radius relative to centre.
-    radius = torch.sqrt(grid_x ** 2 + grid_y ** 2)
-
-    return ifftshift(1. / (1.0 + (radius / cutoff) ** (2 * n)))
-
-
 class FSIMLoss(_Loss):
     r"""Creates a criterion that measures the FSIM or FSIMc for input :math:`x` and target :math:`y`.
 
     In order to be considered as a loss, value ``1 - clip(FSIM, min=0, max=1)`` is returned. If you need FSIM value,
     use function `fsim` instead.
     Supports greyscale and colour images with RGB channel order.
```

### Comparing `piq-0.7.0/piq/functional/__init__.py` & `piq-0.7.1/piq/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.0/piq/functional/base.py` & `piq-0.7.1/piq/functional/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 r"""General purpose functions"""
-from typing import Tuple, Union
+from typing import Tuple, Union, Optional
 import torch
 
 
 def ifftshift(x: torch.Tensor) -> torch.Tensor:
     r""" Similar to np.fft.ifftshift but applies to PyTorch Tensors"""
     shift = [-(ax // 2) for ax in x.size()]
     return torch.roll(x, shift, tuple(range(len(shift))))
 
 
-def get_meshgrid(size: Tuple[int, int]) -> torch.Tensor:
+def get_meshgrid(size: Tuple[int, int], device: Optional[str] = None, dtype: Optional[type] = None) -> torch.Tensor:
     r"""Return coordinate grid matrices centered at zero point.
     Args:
         size: Shape of meshgrid to create
+        device: device to use for creation
+        dtype: dtype to use for creation
+    Returns:
+        Meshgrid of size on device with dtype values.
     """
     if size[0] % 2:
         # Odd
-        x = torch.arange(-(size[0] - 1) / 2, size[0] / 2) / (size[0] - 1)
+        x = torch.arange(-(size[0] - 1) / 2, size[0] / 2, device=device, dtype=dtype) / (size[0] - 1)
     else:
         # Even
-        x = torch.arange(- size[0] / 2, size[0] / 2) / size[0]
+        x = torch.arange(- size[0] / 2, size[0] / 2, device=device, dtype=dtype) / size[0]
 
     if size[1] % 2:
         # Odd
-        y = torch.arange(-(size[1] - 1) / 2, size[1] / 2) / (size[1] - 1)
+        y = torch.arange(-(size[1] - 1) / 2, size[1] / 2, device=device, dtype=dtype) / (size[1] - 1)
     else:
         # Even
-        y = torch.arange(- size[1] / 2, size[1] / 2) / size[1]
+        y = torch.arange(- size[1] / 2, size[1] / 2, device=device, dtype=dtype) / size[1]
     return torch.meshgrid(x, y)
 
 
 def similarity_map(map_x: torch.Tensor, map_y: torch.Tensor, constant: float, alpha: float = 0.0) -> torch.Tensor:
     r""" Compute similarity_map between two tensors using Dice-like equation.
 
     Args:
@@ -49,15 +53,15 @@
     Args:
         x: Tensor with shape (N, C, H, W).
         kernels: Stack of tensors for gradient computation with shape (k_N, k_H, k_W)
     Returns:
         Gradients of x per-channel with shape (N, C, H, W)
     """
     padding = kernels.size(-1) // 2
-    grads = torch.nn.functional.conv2d(x, kernels.to(x), padding=padding)
+    grads = torch.nn.functional.conv2d(x, kernels, padding=padding)
 
     return torch.sqrt(torch.sum(grads ** 2, dim=-3, keepdim=True))
 
 
 def pow_for_complex(base: torch.Tensor, exp: Union[int, float]) -> torch.Tensor:
     r""" Takes the power of each element in a 4D tensor with negative values or 5D tensor with complex values.
     Complex numbers are represented by modulus and argument: r * \exp(i * \phi).
```

### Comparing `piq-0.7.0/piq/functional/colour_conversion.py` & `piq-0.7.1/piq/functional/colour_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,36 +10,36 @@
         x: Batch of images with shape (N, 3, H, W). RGB colour space.
 
     Returns:
         Batch of images with shape (N, 3, H, W). LMN colour space.
     """
     weights_rgb_to_lmn = torch.tensor([[0.06, 0.63, 0.27],
                                        [0.30, 0.04, -0.35],
-                                       [0.34, -0.6, 0.17]]).t().to(x)
+                                       [0.34, -0.6, 0.17]], dtype=x.dtype, device=x.device).t()
     x_lmn = torch.matmul(x.permute(0, 2, 3, 1), weights_rgb_to_lmn).permute(0, 3, 1, 2)
     return x_lmn
 
 
 def rgb2xyz(x: torch.Tensor) -> torch.Tensor:
     r"""Convert a batch of RGB images to a batch of XYZ images
 
     Args:
         x: Batch of images with shape (N, 3, H, W). RGB colour space.
 
     Returns:
         Batch of images with shape (N, 3, H, W). XYZ colour space.
     """
-    mask_below = (x <= 0.04045).to(x)
-    mask_above = (x > 0.04045).to(x)
+    mask_below = (x <= 0.04045).type(x.dtype)
+    mask_above = (x > 0.04045).type(x.dtype)
 
     tmp = x / 12.92 * mask_below + torch.pow((x + 0.055) / 1.055, 2.4) * mask_above
 
     weights_rgb_to_xyz = torch.tensor([[0.4124564, 0.3575761, 0.1804375],
                                        [0.2126729, 0.7151522, 0.0721750],
-                                       [0.0193339, 0.1191920, 0.9503041]]).to(x)
+                                       [0.0193339, 0.1191920, 0.9503041]], dtype=x.dtype, device=x.device)
 
     x_xyz = torch.matmul(tmp.permute(0, 2, 3, 1), weights_rgb_to_xyz.t()).permute(0, 3, 1, 2)
     return x_xyz
 
 
 def xyz2lab(x: torch.Tensor, illuminant: str = 'D50', observer: str = '2') -> torch.Tensor:
     r"""Convert a batch of XYZ images to a batch of LAB images
@@ -64,26 +64,27 @@
          "D65": {'2': (0.95047, 1., 1.08883),  # This was: `lab_ref_white`
                  '10': (0.94809667673716, 1, 1.0730513595166162)},
          "D75": {'2': (0.9497220898840717, 1, 1.226393520724154),
                  '10': (0.9441713925645873, 1, 1.2064272211720228)},
          "E": {'2': (1.0, 1.0, 1.0),
                '10': (1.0, 1.0, 1.0)}}
 
-    illuminants_to_use = torch.tensor(illuminants[illuminant][observer]).to(x).view(1, 3, 1, 1)
+    illuminants_to_use = torch.tensor(illuminants[illuminant][observer],
+                                      dtype=x.dtype, device=x.device).view(1, 3, 1, 1)
 
     tmp = x / illuminants_to_use
 
-    mask_below = tmp <= epsilon
-    mask_above = tmp > epsilon
+    mask_below = (tmp <= epsilon).type(x.dtype)
+    mask_above = (tmp > epsilon).type(x.dtype)
     tmp = torch.pow(tmp, 1. / 3.) * mask_above + (kappa * tmp + 16.) / 116. * mask_below
 
     weights_xyz_to_lab = torch.tensor([[0, 116., 0],
                                        [500., -500., 0],
-                                       [0, 200., -200.]]).to(x)
-    bias_xyz_to_lab = torch.tensor([-16., 0., 0.]).to(x).view(1, 3, 1, 1)
+                                       [0, 200., -200.]], dtype=x.dtype, device=x.device)
+    bias_xyz_to_lab = torch.tensor([-16., 0., 0.], dtype=x.dtype, device=x.device).view(1, 3, 1, 1)
 
     x_lab = torch.matmul(tmp.permute(0, 2, 3, 1), weights_xyz_to_lab.t()).permute(0, 3, 1, 2) + bias_xyz_to_lab
     return x_lab
 
 
 def rgb2lab(x: torch.Tensor, data_range: Union[int, float] = 255) -> torch.Tensor:
     r"""Convert a batch of RGB images to a batch of LAB images
@@ -106,15 +107,15 @@
 
     Returns:
         Batch of images with shape (N, 3, H, W). YIQ colour space.
     """
     yiq_weights = torch.tensor([
         [0.299, 0.587, 0.114],
         [0.5959, -0.2746, -0.3213],
-        [0.2115, -0.5227, 0.3112]]).t().to(x)
+        [0.2115, -0.5227, 0.3112]], dtype=x.dtype, device=x.device).t()
     x_yiq = torch.matmul(x.permute(0, 2, 3, 1), yiq_weights).permute(0, 3, 1, 2)
     return x_yiq
 
 
 def rgb2lhm(x: torch.Tensor) -> torch.Tensor:
     r"""Convert a batch of RGB images to a batch of LHM images
 
@@ -126,10 +127,10 @@
 
     Reference:
         https://arxiv.org/pdf/1608.07433.pdf
     """
     lhm_weights = torch.tensor([
         [0.2989, 0.587, 0.114],
         [0.3, 0.04, -0.35],
-        [0.34, -0.6, 0.17]]).t().to(x)
+        [0.34, -0.6, 0.17]], dtype=x.dtype, device=x.device).t()
     x_lhm = torch.matmul(x.permute(0, 2, 3, 1), lhm_weights).permute(0, 3, 1, 2)
     return x_lhm
```

### Comparing `piq-0.7.0/piq/functional/layers.py` & `piq-0.7.1/piq/functional/layers.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.0/piq/functional/resize.py` & `piq-0.7.1/piq/functional/resize.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.0/piq/gmsd.py` & `piq-0.7.1/piq/gmsd.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,16 @@
         gmsd : Gradient Magnitude Similarity Deviation between given tensors.
 
     References:
         https://arxiv.org/pdf/1308.3052.pdf
     """
 
     # Compute grad direction
-    kernels = torch.stack([prewitt_filter(), prewitt_filter().transpose(-1, -2)])
+    p_filter = prewitt_filter(dtype=x.dtype, device=x.device)
+    kernels = torch.stack([p_filter, p_filter.transpose(-1, -2)])
     x_grad = gradient_map(x, kernels)
     y_grad = gradient_map(y, kernels)
 
     # Compute GMS
     gms = similarity_map(x_grad, y_grad, constant=t, alpha=alpha)
     mean_gms = torch.mean(gms, dim=[1, 2, 3], keepdims=True)
 
@@ -177,18 +178,18 @@
 
     # Rescale
     x = x / float(data_range) * 255
     y = y / float(data_range) * 255
 
     # Values from the paper
     if scale_weights is None:
-        scale_weights = torch.tensor([0.096, 0.596, 0.289, 0.019], device=x.device)
+        scale_weights = torch.tensor([0.096, 0.596, 0.289, 0.019], device=x.device, dtype=x.dtype)
     else:
         # Normalize scale weights
-        scale_weights = (scale_weights / scale_weights.sum()).to(x)
+        scale_weights = (scale_weights / scale_weights.sum())
 
     # Check that input is big enough
     num_scales = scale_weights.size(0)
     min_size = 2 ** num_scales + 1
 
     if x.size(-1) < min_size or x.size(-2) < min_size:
         raise ValueError(f'Invalid size of the input images, expected at least {min_size}x{min_size}.')
```

### Comparing `piq-0.7.0/piq/gs.py` & `piq-0.7.1/piq/gs.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.0/piq/haarpsi.py` & `piq-0.7.1/piq/haarpsi.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,22 +78,23 @@
         x_yiq = F.avg_pool2d(x_yiq, kernel_size=2, stride=2, padding=0)
         y_yiq = F.avg_pool2d(y_yiq, kernel_size=2, stride=2, padding=0)
 
     # Haar wavelet decomposition
     coefficients_x, coefficients_y = [], []
     for scale in range(scales):
         kernel_size = 2 ** (scale + 1)
-        kernels = torch.stack([haar_filter(kernel_size), haar_filter(kernel_size).transpose(-1, -2)])
+        h_filter = haar_filter(kernel_size, dtype=x.dtype, device=x.device)
+        kernels = torch.stack([h_filter, h_filter.transpose(-1, -2)])
 
         # Asymmetrical padding due to even kernel size. Matches MATLAB conv2(A, B, 'same')
         upper_pad = kernel_size // 2 - 1
         bottom_pad = kernel_size // 2
         pad_to_use = [upper_pad, bottom_pad, upper_pad, bottom_pad]
-        coeff_x = torch.nn.functional.conv2d(F.pad(x_yiq[:, : 1], pad=pad_to_use, mode='constant'), kernels.to(x))
-        coeff_y = torch.nn.functional.conv2d(F.pad(y_yiq[:, : 1], pad=pad_to_use, mode='constant'), kernels.to(y))
+        coeff_x = torch.nn.functional.conv2d(F.pad(x_yiq[:, : 1], pad=pad_to_use, mode='constant'), kernels)
+        coeff_y = torch.nn.functional.conv2d(F.pad(y_yiq[:, : 1], pad=pad_to_use, mode='constant'), kernels)
 
         coefficients_x.append(coeff_x)
         coefficients_y.append(coeff_y)
 
     # Shape (N, {scales * 2}, H, W)
     coefficients_x = torch.cat(coefficients_x, dim=1)
     coefficients_y = torch.cat(coefficients_y, dim=1)
```

### Comparing `piq-0.7.0/piq/isc.py` & `piq-0.7.1/piq/isc.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             p_yx = subset[k, :]
             scores.append(F.kl_div(p_y.log(), p_yx, reduction='sum'))
 
         # Compute exponential of the mean of the KL-divergence for each split
         partial_scores.append(torch.tensor(scores).mean().exp())
 
     partial_scores = torch.tensor(partial_scores)
-    return torch.mean(partial_scores).to(features), torch.std(partial_scores).to(features)
+    return torch.mean(partial_scores), torch.std(partial_scores)
 
 
 class IS(BaseFeatureMetric):
     r"""Creates a criterion that measures difference of Inception Score between two datasets.
 
     IS is computed separately for predicted :math:`x` and target :math:`y` features and expects raw InceptionV3 model
     logits as inputs.
```

### Comparing `piq-0.7.0/piq/iw_ssim.py` & `piq-0.7.1/piq/iw_ssim.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,19 +82,19 @@
 
     min_size = (kernel_size - 1) * 2 ** (levels - 1) + 1
     if x.size(-1) < min_size or x.size(-2) < min_size:
         raise ValueError(f'Invalid size of the input images, expected at least {min_size}x{min_size}.')
 
     blur_pad = math.ceil((kernel_size - 1) / 2)  # Ceil
     iw_pad = blur_pad - math.floor((blk_size - 1) / 2)  # floor
-    gauss_kernel = gaussian_filter(kernel_size, kernel_sigma).repeat(x.size(1), 1, 1, 1).to(x)
+    gauss_kernel = gaussian_filter(kernel_size, kernel_sigma, device=x.device, dtype=x.dtype).repeat(x.size(1), 1, 1, 1)
 
     # Size of the kernel size to build Laplacian pyramid
     pyramid_kernel_size = 5
-    bin_filter = binomial_filter1d(kernel_size=pyramid_kernel_size).to(x) * 2 ** 0.5
+    bin_filter = binomial_filter1d(kernel_size=pyramid_kernel_size, device=x.device, dtype=x.dtype) * 2 ** 0.5
 
     lo_x, x_diff_old = _pyr_step(x, bin_filter)
     lo_y, y_diff_old = _pyr_step(y, bin_filter)
 
     x = lo_x
     y = lo_y
     wmcs = []
@@ -315,15 +315,15 @@
 
     Returns:
         Information Content Maps.
     """
 
     EPS = torch.finfo(x.dtype).eps
     n_channels = x.size(1)
-    kernel = average_filter2d(kernel_size=kernel_size).repeat(x.size(1), 1, 1, 1).to(x)
+    kernel = average_filter2d(kernel_size=kernel_size, device=x.device, dtype=x.dtype).repeat(x.size(1), 1, 1, 1)
     padding_up = kernel.size(-1) // 2
     padding_down = kernel.size(-1) - padding_up
 
     mu_x = F.conv2d(input=F.pad(x, pad=[padding_up, padding_down, padding_up, padding_down]), weight=kernel, padding=0,
                     groups=n_channels)
     mu_y = F.conv2d(input=F.pad(y, pad=[padding_up, padding_down, padding_up, padding_down]), weight=kernel, padding=0,
                     groups=n_channels)
@@ -428,15 +428,15 @@
     Args:
         x: An input tensor. Shape :math:`(N, C, H, W)`.
 
     Returns:
         Upscaled tensor.
     """
     t1 = F.interpolate(x, size=(int(4 * x.size(-2) - 3), int(4 * x.size(-1) - 3)), mode='bilinear', align_corners=False)
-    t2 = torch.zeros([x.size(0), 1, 4 * x.size(-2) - 1, 4 * x.size(-1) - 1]).to(x)
+    t2 = torch.zeros([x.size(0), 1, 4 * x.size(-2) - 1, 4 * x.size(-1) - 1], device=x.device, dtype=x.dtype)
     t2[:, :, 1: -1, 1:-1] = t1
     t2[:, :, 0, :] = 2 * t2[:, :, 1, :] - t2[:, :, 2, :]
     t2[:, :, -1, :] = 2 * t2[:, :, -2, :] - t2[:, :, -3, :]
     t2[:, :, :, 0] = 2 * t2[:, :, :, 1] - t2[:, :, :, 2]
     t2[:, :, :, -1] = 2 * t2[:, :, :, -2] - t2[:, :, :, -3]
     out = t2[:, :, ::2, ::2]
     return out
```

### Comparing `piq-0.7.0/piq/kid.py` & `piq-0.7.1/piq/kid.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.0/piq/mdsi.py` & `piq-0.7.1/piq/mdsi.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,16 @@
 
     x = avg_pool2d(x, kernel_size=kernel_size)
     y = avg_pool2d(y, kernel_size=kernel_size)
 
     x_lhm = rgb2lhm(x)
     y_lhm = rgb2lhm(y)
 
-    kernels = torch.stack([prewitt_filter(), prewitt_filter().transpose(1, 2)]).to(x)
+    p_filter = prewitt_filter(device=x_lhm.device, dtype=x_lhm.dtype)
+    kernels = torch.stack([p_filter, p_filter.transpose(1, 2)])
     gm_x = gradient_map(x_lhm[:, :1], kernels)
     gm_y = gradient_map(y_lhm[:, :1], kernels)
     gm_avg = gradient_map((x_lhm[:, :1] + y_lhm[:, :1]) / 2., kernels)
 
     gs_x_y = similarity_map(gm_x, gm_y, c1)
     gs_x_average = similarity_map(gm_x, gm_avg, c2)
     gs_y_average = similarity_map(gm_y, gm_avg, c2)
```

### Comparing `piq-0.7.0/piq/ms_ssim.py` & `piq-0.7.1/piq/ms_ssim.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,22 +61,22 @@
     _validate_input([x, y], dim_range=(4, 5), data_range=(0, data_range))
 
     x = x / float(data_range)
     y = y / float(data_range)
 
     if scale_weights is None:
         # Values from MS-SSIM the paper
-        scale_weights = torch.tensor([0.0448, 0.2856, 0.3001, 0.2363, 0.1333]).to(x)
+        scale_weights = torch.tensor([0.0448, 0.2856, 0.3001, 0.2363, 0.1333], dtype=x.dtype, device=x.device)
     else:
         # Normalize scale weights
-        scale_weights = (scale_weights / scale_weights.sum()).to(x)
+        scale_weights = (scale_weights / scale_weights.sum())
     if scale_weights.size(0) != scale_weights.numel():
         raise ValueError(f'Expected a vector of weights, got {scale_weights.dim()}D tensor')
 
-    kernel = gaussian_filter(kernel_size, kernel_sigma).repeat(x.size(1), 1, 1, 1).to(x)
+    kernel = gaussian_filter(kernel_size, kernel_sigma, device=x.device, dtype=x.dtype).repeat(x.size(1), 1, 1, 1)
 
     _compute_msssim = _multi_scale_ssim_complex if x.dim() == 5 else _multi_scale_ssim
     msssim_val = _compute_msssim(
         x=x,
         y=y,
         data_range=data_range,
         kernel=kernel,
```

### Comparing `piq-0.7.0/piq/msid.py` & `piq-0.7.1/piq/msid.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.0/piq/perceptual.py` & `piq-0.7.1/piq/perceptual.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.0/piq/pieapp.py` & `piq-0.7.1/piq/pieapp.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.0/piq/pr.py` & `piq-0.7.1/piq/pr.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.0/piq/psnr.py` & `piq-0.7.1/piq/psnr.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     EPS = 1e-8
 
     x = x / float(data_range)
     y = y / float(data_range)
 
     if (x.size(1) == 3) and convert_to_greyscale:
         # Convert RGB image to YIQ and take luminance: Y = 0.299 R + 0.587 G + 0.114 B
-        rgb_to_grey = torch.tensor([0.299, 0.587, 0.114]).view(1, -1, 1, 1).to(x)
+        rgb_to_grey = torch.tensor([0.299, 0.587, 0.114], device=x.device, dtype=x.dtype).view(1, -1, 1, 1)
         x = torch.sum(x * rgb_to_grey, dim=1, keepdim=True)
         y = torch.sum(y * rgb_to_grey, dim=1, keepdim=True)
 
     mse = torch.mean((x - y) ** 2, dim=[1, 2, 3])
     score: torch.Tensor = - 10 * torch.log10(mse + EPS)
 
     return _reduce(score, reduction)
```

### Comparing `piq-0.7.0/piq/srsim.py` & `piq-0.7.1/piq/srsim.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,15 +88,16 @@
     )
     svrs_y = _spectral_residual_visual_saliency(
         y_lum, scale=scale, kernel_size=kernel_size,
         sigma=sigma, gaussian_size=gaussian_size
     )
 
     # Gradient maps
-    kernels = torch.stack([scharr_filter(), scharr_filter().transpose(-1, -2)])
+    sch_filter = scharr_filter(device=x_lum.device, dtype=x_lum.dtype)
+    kernels = torch.stack([sch_filter, sch_filter.transpose(-1, -2)])
     grad_map_x = gradient_map(x_lum, kernels)
     grad_map_y = gradient_map(y_lum, kernels)
 
     # Constants from the paper
     C1, C2, alpha = 0.40, 225, 0.50
 
     # Compute SR-SIM
@@ -183,20 +184,22 @@
         saliency_map = torch.abs(torch.fft.ifft2(torch.view_as_complex(compx))) ** 2
 
     else:
         saliency_map = torch.sum(torch.ifft(compx, 2) ** 2, dim=-1)
 
     # After effect for SR-SIM
     # Apply gaussian blur
-    kernel = gaussian_filter(gaussian_size, sigma)
+    kernel = gaussian_filter(gaussian_size, sigma, device=saliency_map.device, dtype=saliency_map.dtype)
     if gaussian_size % 2 == 0:  # matlab pads upper and lower borders with 0s for even kernels
-        kernel = torch.cat((torch.zeros(1, 1, gaussian_size), kernel), 1)
-        kernel = torch.cat((torch.zeros(1, gaussian_size + 1, 1), kernel), 2)
+        kernel = torch.cat((torch.zeros(1, 1, gaussian_size,
+                            device=saliency_map.device, dtype=saliency_map.dtype), kernel), 1)
+        kernel = torch.cat((torch.zeros(1, gaussian_size + 1, 1,
+                            device=saliency_map.device, dtype=saliency_map.dtype), kernel), 2)
         gaussian_size += 1
-    kernel = kernel.view(1, 1, gaussian_size, gaussian_size).to(saliency_map)
+    kernel = kernel.view(1, 1, gaussian_size, gaussian_size)
     saliency_map = F.conv2d(saliency_map, kernel, padding=(gaussian_size - 1) // 2)
 
     # normalize between [0, 1]
     min_sal = torch.min(saliency_map[:])
     max_sal = torch.max(saliency_map[:])
     saliency_map = (saliency_map - min_sal) / (max_sal - min_sal + eps)
```

### Comparing `piq-0.7.0/piq/ssim.py` & `piq-0.7.1/piq/ssim.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     # Averagepool image if the size is large enough
     f = max(1, round(min(x.size()[-2:]) / 256))
     if (f > 1) and downsample:
         x = F.avg_pool2d(x, kernel_size=f)
         y = F.avg_pool2d(y, kernel_size=f)
 
-    kernel = gaussian_filter(kernel_size, kernel_sigma).repeat(x.size(1), 1, 1, 1).to(y)
+    kernel = gaussian_filter(kernel_size, kernel_sigma, device=x.device, dtype=x.dtype).repeat(x.size(1), 1, 1, 1)
     _compute_ssim_per_channel = _ssim_per_channel_complex if x.dim() == 5 else _ssim_per_channel
     ssim_map, cs_map = _compute_ssim_per_channel(x=x, y=y, kernel=kernel, data_range=data_range, k1=k1, k2=k2)
     ssim_val = ssim_map.mean(1)
     cs = cs_map.mean(1)
 
     ssim_val = _reduce(ssim_val, reduction)
     cs = _reduce(cs, reduction)
```

### Comparing `piq-0.7.0/piq/tv.py` & `piq-0.7.1/piq/tv.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.0/piq/utils/common.py` & `piq-0.7.1/piq/utils/common.py`

 * *Files identical despite different names*

### Comparing `piq-0.7.0/piq/vif.py` & `piq-0.7.1/piq/vif.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
     # Constant for numerical stability
     EPS = 1e-8
 
     # Progressively downsample images and compute VIF on different scales
     x_vif, y_vif = 0, 0
     for scale in range(4):
         kernel_size = 2 ** (4 - scale) + 1
-        kernel = gaussian_filter(kernel_size, sigma=kernel_size / 5)
-        kernel = kernel.view(1, 1, kernel_size, kernel_size).to(x)
+        kernel = gaussian_filter(kernel_size, sigma=kernel_size / 5, device=x.device, dtype=x.dtype)
+        kernel = kernel.view(1, 1, kernel_size, kernel_size)
 
         if scale > 0:
             # Convolve and downsample
             x = F.conv2d(x, kernel)[:, :, ::2, ::2]  # valid padding
             y = F.conv2d(y, kernel)[:, :, ::2, ::2]  # valid padding
 
         mu_x, mu_y = F.conv2d(x, kernel), F.conv2d(y, kernel)  # valid padding
```

### Comparing `piq-0.7.0/piq/vsi.py` & `piq-0.7.1/piq/vsi.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 https://sse.tongji.edu.cn/linzhang/IQA/VSI/VSI.htm
 
 References:
     https://ieeexplore.ieee.org/document/6873260
 """
 import warnings
 import functools
-from typing import Union, Tuple
+from typing import Union
 
 import torch
 from torch.nn.modules.loss import _Loss
 from torch.nn.functional import avg_pool2d, interpolate, pad
 
 from piq.functional import ifftshift, gradient_map, scharr_filter, rgb2lmn, rgb2lab, similarity_map, get_meshgrid
 from piq.utils import _validate_input, _reduce, _parse_version
@@ -92,15 +92,16 @@
     vs_x = avg_pool2d(vs_x, kernel_size=kernel_size)
     vs_y = avg_pool2d(vs_y, kernel_size=kernel_size)
 
     x_lmn = avg_pool2d(x_lmn, kernel_size=kernel_size)
     y_lmn = avg_pool2d(y_lmn, kernel_size=kernel_size)
 
     # Calculate gradient map
-    kernels = torch.stack([scharr_filter(), scharr_filter().transpose(1, 2)]).to(x_lmn)
+    sch_filter = scharr_filter(device=x_lmn.device, dtype=x_lmn.dtype)
+    kernels = torch.stack([sch_filter, sch_filter.transpose(1, 2)])
     gm_x = gradient_map(x_lmn[:, :1], kernels)
     gm_y = gradient_map(y_lmn[:, :1], kernels)
 
     # Calculate all similarity maps
     s_vs = similarity_map(vs_x, vs_y, c1)
     s_gm = similarity_map(gm_x, gm_y, c2)
     s_m = similarity_map(x_lmn[:, 1:2], y_lmn[:, 1:2], c3)
@@ -207,27 +208,29 @@
     x = x / float(data_range) * 255
     size = x.size()
     size_to_use = (256, 256)
     x = interpolate(input=x, size=size_to_use, mode='bilinear', align_corners=False)
 
     x_lab = rgb2lab(x, data_range=255)
 
-    lg = _log_gabor(size_to_use, omega_0, sigma_f).to(x).view(1, 1, *size_to_use)
+    xx, yy = get_meshgrid(size_to_use, device=x_lab.device, dtype=x_lab.dtype)
+    lg = _log_gabor(xx, yy, omega_0, sigma_f).view(1, 1, *size_to_use)
+
     recommended_torch_version = _parse_version('1.8.0')
     torch_version = _parse_version(torch.__version__)
     if len(torch_version) != 0 and torch_version >= recommended_torch_version:
         x_fft = torch.fft.fft2(x_lab)
         x_ifft_real = torch.fft.ifft2(x_fft * lg).real
     else:
         x_fft = torch.rfft(x_lab, 2, onesided=False)
         x_ifft_real = torch.ifft(x_fft * lg.unsqueeze(-1), 2)[..., 0]
 
     s_f = x_ifft_real.pow(2).sum(dim=1, keepdim=True).sqrt()
 
-    coordinates = torch.stack(get_meshgrid(size_to_use), dim=0).to(x)
+    coordinates = torch.stack([xx, yy], dim=0)
     coordinates = coordinates * size_to_use[0] + 1
     s_d = torch.exp(-torch.sum(coordinates ** 2, dim=0) / sigma_d ** 2).view(1, 1, *size_to_use)
 
     eps = torch.finfo(x_lab.dtype).eps
     min_x = x_lab.min(dim=-1, keepdim=True).values.min(dim=-2, keepdim=True).values
     max_x = x_lab.max(dim=-1, keepdim=True).values.max(dim=-2, keepdim=True).values
     normalized = (x_lab - min_x) / (max_x - min_x + eps)
@@ -238,27 +241,27 @@
     vs_m = s_f * s_d * s_c
     vs_m = interpolate(vs_m, size[-2:], mode='bilinear', align_corners=True)
     min_vs_m = vs_m.min(dim=-1, keepdim=True).values.min(dim=-2, keepdim=True).values
     max_vs_m = vs_m.max(dim=-1, keepdim=True).values.max(dim=-2, keepdim=True).values
     return (vs_m - min_vs_m) / (max_vs_m - min_vs_m + eps)
 
 
-def _log_gabor(size: Tuple[int, int], omega_0: float, sigma_f: float) -> torch.Tensor:
+def _log_gabor(xx: torch.Tensor, yy: torch.Tensor, omega_0: float, sigma_f: float, ) -> torch.Tensor:
     r"""Creates log Gabor filter
 
     Args:
-        size: size of the requires log Gabor filter
+        xx: x component of meshgrid
+        yy: y component of meshgrid
         omega_0: center frequency of the filter
         sigma_f: bandwidth of the filter
-
+        device: target device for kernel generation
+        dtype: target data type for kernel generation
     Returns:
         log Gabor filter
     """
-    xx, yy = get_meshgrid(size)
-
     radius = (xx ** 2 + yy ** 2).sqrt()
     mask = radius <= 0.5
 
     r = radius * mask
     r = ifftshift(r)
     r[0, 0] = 1
```

### Comparing `piq-0.7.0/piq.egg-info/PKG-INFO` & `piq-0.7.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: piq
-Version: 0.7.0
-Summary: Measures and metrics for image2image tasks. PyTorch.
-Home-page: https://github.com/photosynthesis-team/piq
-Author: Sergey Kastryulin
-Author-email: snk4tr@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 
 .. image:: https://raw.githubusercontent.com/photosynthesis-team/piq/master/docs/source/_static/piq_logo_main.png
     :target: https://github.com/photosynthesis-team/piq
 
 ..
 
   PyTorch Image Quality (PIQ) is not endorsed by Facebook, Inc.;
@@ -51,18 +36,18 @@
 The library contains a set of measures and metrics that is continually getting extended.
 For measures/metrics that can be used as loss functions, corresponding PyTorch modules are implemented.
 
 We provide:
 
 * Unified interface, which is easy to use and extend.
 * Written on pure PyTorch with bare minima of additional dependencies.
-* Extensive user input validation. You code will not crash in the middle of the training.
+* Extensive user input validation. Your code will not crash in the middle of the training.
 * Fast (GPU computations available) and reliable.
 * Most metrics can be backpropagated for model optimization.
-* Supports python 3.6-3.8.
+* Supports python 3.7-3.10.
 
 PIQ was initially named `PhotoSynthesis.Metrics <https://pypi.org/project/photosynthesis-metrics/0.4.0/>`_.
 
 .. intro-section-end
 
 .. installation-section-start
 
@@ -330,20 +315,31 @@
 
 Citation
 --------
 If you use PIQ in your project, please, cite it as follows.
 
 .. code-block:: tex
 
+   @misc{kastryulin2022piq,
+     title = {PyTorch Image Quality: Metrics for Image Quality Assessment},
+     url = {https://arxiv.org/abs/2208.14818},
+     author = {Kastryulin, Sergey and Zakirov, Jamil and Prokopenko, Denis and Dylov, Dmitry V.},
+     doi = {10.48550/ARXIV.2208.14818},
+     publisher = {arXiv},
+     year = {2022}
+   }
+
+.. code-block:: tex
+
    @misc{piq,
      title={{PyTorch Image Quality}: Metrics and Measure for Image Quality Assessment},
      url={https://github.com/photosynthesis-team/piq},
      note={Open-source software available at https://github.com/photosynthesis-team/piq},
      author={Sergey Kastryulin and Dzhamil Zakirov and Denis Prokopenko},
-     year={2019},
+     year={2019}
    }
 
 .. citation-section-end
 
 .. contacts-section-start
 
 Contacts
@@ -352,9 +348,7 @@
 **Sergey Kastryulin** - `@snk4tr <https://github.com/snk4tr>`_ - ``snk4tr@gmail.com``
 
 **Jamil Zakirov** - `@zakajd <https://github.com/zakajd>`_ - ``djamilzak@gmail.com``
 
 **Denis Prokopenko** - `@denproc <https://github.com/denproc>`_ - ``d.prokopenko@outlook.com``
 
 .. contacts-section-end
-
-
```

### Comparing `piq-0.7.0/setup.py` & `piq-0.7.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,14 @@
     author="Sergey Kastryulin",
     author_email="snk4tr@gmail.com",
     description="Measures and metrics for image2image tasks. PyTorch.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/photosynthesis-team/piq",
     install_requires=required,
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(exclude=["tests", "examples"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
 )
```

