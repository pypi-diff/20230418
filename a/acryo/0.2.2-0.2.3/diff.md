# Comparing `tmp/acryo-0.2.2.tar.gz` & `tmp/acryo-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acryo-0.2.2.tar", last modified: Mon Apr 10 14:05:45 2023, max compression
+gzip compressed data, was "acryo-0.2.3.tar", last modified: Tue Apr 18 14:37:25 2023, max compression
```

## Comparing `acryo-0.2.2.tar` & `acryo-0.2.3.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.122452 acryo-0.2.2/
--rw-rw-rw-   0        0        0     1547 2022-04-12 12:12:07.000000 acryo-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     2301 2023-04-10 14:05:45.121942 acryo-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2011 2023-03-15 04:48:31.000000 acryo-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 14:05:44.975348 acryo-0.2.2/acryo/
--rw-rw-rw-   0        0        0      380 2023-04-09 13:27:24.000000 acryo-0.2.2/acryo/__init__.py
--rw-rw-rw-   0        0        0    10606 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/_correlation.py
--rw-rw-rw-   0        0        0      661 2023-02-19 09:29:23.000000 acryo-0.2.2/acryo/_fft.py
--rw-rw-rw-   0        0        0     2929 2023-02-20 00:46:56.000000 acryo-0.2.2/acryo/_reader.py
--rw-rw-rw-   0        0        0     2784 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/_rotation.py
--rw-rw-rw-   0        0        0      244 2023-02-23 14:34:20.000000 acryo-0.2.2/acryo/_types.py
--rw-rw-rw-   0        0        0    12048 2023-04-09 13:27:24.000000 acryo-0.2.2/acryo/_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.023437 acryo-0.2.2/acryo/alignment/
--rw-rw-rw-   0        0        0      384 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/alignment/__init__.py
--rw-rw-rw-   0        0        0    25875 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/alignment/_base.py
--rw-rw-rw-   0        0        0     1637 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/alignment/_concrete.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.034215 acryo-0.2.2/acryo/classification/
--rw-rw-rw-   0        0        0       62 2022-04-12 15:56:50.000000 acryo-0.2.2/acryo/classification/__init__.py
--rw-rw-rw-   0        0        0    18578 2023-02-08 03:31:15.000000 acryo-0.2.2/acryo/classification/_dask_pca.py
--rw-rw-rw-   0        0        0     5185 2023-02-21 02:27:31.000000 acryo-0.2.2/acryo/classification/pca.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.059301 acryo-0.2.2/acryo/loader/
--rw-rw-rw-   0        0        0      187 2023-02-19 15:38:13.000000 acryo-0.2.2/acryo/loader/__init__.py
--rw-rw-rw-   0        0        0    35134 2023-02-27 14:09:35.000000 acryo-0.2.2/acryo/loader/_base.py
--rw-rw-rw-   0        0        0     7099 2023-02-26 13:13:09.000000 acryo-0.2.2/acryo/loader/_batch.py
--rw-rw-rw-   0        0        0     1696 2023-02-21 08:34:02.000000 acryo-0.2.2/acryo/loader/_cache.py
--rw-rw-rw-   0        0        0    17909 2023-02-27 14:09:35.000000 acryo-0.2.2/acryo/loader/_group.py
--rw-rw-rw-   0        0        0     9034 2023-02-25 12:12:36.000000 acryo-0.2.2/acryo/loader/_loader.py
--rw-rw-rw-   0        0        0     2222 2023-02-24 06:22:10.000000 acryo-0.2.2/acryo/loader/_misc.py
--rw-rw-rw-   0        0        0     9986 2023-03-15 04:51:58.000000 acryo-0.2.2/acryo/loader/_mock.py
--rw-rw-rw-   0        0        0    34451 2023-04-09 13:27:24.000000 acryo-0.2.2/acryo/molecules.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.068941 acryo-0.2.2/acryo/pick/
--rw-rw-rw-   0        0        0      129 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/pick/__init__.py
--rw-rw-rw-   0        0        0     4680 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/pick/_base.py
--rw-rw-rw-   0        0        0     4799 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/pick/_concrete.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.087669 acryo-0.2.2/acryo/pipe/
--rw-rw-rw-   0        0        0      647 2023-02-23 14:49:44.000000 acryo-0.2.2/acryo/pipe/__init__.py
--rw-rw-rw-   0        0        0    12167 2023-02-23 11:14:01.000000 acryo-0.2.2/acryo/pipe/_classes.py
--rw-rw-rw-   0        0        0     3843 2023-02-25 03:55:45.000000 acryo-0.2.2/acryo/pipe/_curry.py
--rw-rw-rw-   0        0        0     5436 2023-02-23 15:13:40.000000 acryo-0.2.2/acryo/pipe/_imread.py
--rw-rw-rw-   0        0        0     3459 2023-02-23 11:14:00.000000 acryo-0.2.2/acryo/pipe/_masking.py
--rw-rw-rw-   0        0        0     1215 2023-02-25 03:55:55.000000 acryo-0.2.2/acryo/pipe/_transform.py
--rw-rw-rw-   0        0        0    13577 2023-02-18 15:53:02.000000 acryo-0.2.2/acryo/simulator.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.097191 acryo-0.2.2/acryo/testing/
--rw-rw-rw-   0        0        0      130 2022-04-15 01:53:16.000000 acryo-0.2.2/acryo/testing/__init__.py
--rw-rw-rw-   0        0        0     1145 2022-05-02 14:08:55.000000 acryo-0.2.2/acryo/testing/_templates.py
--rw-rw-rw-   0        0        0     4432 2023-03-02 06:44:45.000000 acryo-0.2.2/acryo/testing/core.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.014914 acryo-0.2.2/acryo.egg-info/
--rw-rw-rw-   0        0        0     2301 2023-04-10 14:05:44.000000 acryo-0.2.2/acryo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1142 2023-04-10 14:05:44.000000 acryo-0.2.2/acryo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 14:05:44.000000 acryo-0.2.2/acryo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-04-10 14:05:44.000000 acryo-0.2.2/acryo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-10 14:05:44.000000 acryo-0.2.2/acryo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 14:05:45.123467 acryo-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      821 2023-04-10 14:01:42.000000 acryo-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:05:45.118937 acryo-0.2.2/tests/
--rw-rw-rw-   0        0        0     3548 2023-04-09 13:27:24.000000 acryo-0.2.2/tests/test_alignment.py
--rw-rw-rw-   0        0        0     2602 2023-02-21 08:34:02.000000 acryo-0.2.2/tests/test_batch.py
--rw-rw-rw-   0        0        0     1360 2023-02-21 08:34:02.000000 acryo-0.2.2/tests/test_cache.py
--rw-rw-rw-   0        0        0     1736 2023-02-23 14:27:37.000000 acryo-0.2.2/tests/test_group.py
--rw-rw-rw-   0        0        0     6716 2023-02-24 04:50:51.000000 acryo-0.2.2/tests/test_molecules.py
--rw-rw-rw-   0        0        0      691 2023-02-21 11:08:36.000000 acryo-0.2.2/tests/test_pipe.py
--rw-rw-rw-   0        0        0     1545 2023-01-29 13:16:40.000000 acryo-0.2.2/tests/test_simulator.py
--rw-rw-rw-   0        0        0      542 2023-02-14 03:49:57.000000 acryo-0.2.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.379999 acryo-0.2.3/
+-rw-rw-rw-   0        0        0     1547 2022-04-12 12:12:07.000000 acryo-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     2301 2023-04-18 14:37:25.378989 acryo-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2011 2023-03-15 04:48:31.000000 acryo-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.230779 acryo-0.2.3/acryo/
+-rw-rw-rw-   0        0        0      380 2023-04-18 14:33:31.000000 acryo-0.2.3/acryo/__init__.py
+-rw-rw-rw-   0        0        0    11845 2023-04-18 09:04:57.000000 acryo-0.2.3/acryo/_correlation.py
+-rw-rw-rw-   0        0        0      661 2023-02-19 09:29:23.000000 acryo-0.2.3/acryo/_fft.py
+-rw-rw-rw-   0        0        0     2929 2023-02-20 00:46:56.000000 acryo-0.2.3/acryo/_reader.py
+-rw-rw-rw-   0        0        0     2784 2023-03-02 06:44:45.000000 acryo-0.2.3/acryo/_rotation.py
+-rw-rw-rw-   0        0        0      244 2023-02-23 14:34:20.000000 acryo-0.2.3/acryo/_types.py
+-rw-rw-rw-   0        0        0    12048 2023-04-09 13:27:24.000000 acryo-0.2.3/acryo/_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.280202 acryo-0.2.3/acryo/alignment/
+-rw-rw-rw-   0        0        0      384 2023-03-02 06:44:45.000000 acryo-0.2.3/acryo/alignment/__init__.py
+-rw-rw-rw-   0        0        0    30369 2023-04-18 09:04:57.000000 acryo-0.2.3/acryo/alignment/_base.py
+-rw-rw-rw-   0        0        0     1469 2023-04-18 09:04:57.000000 acryo-0.2.3/acryo/alignment/_bound.py
+-rw-rw-rw-   0        0        0     2701 2023-04-18 09:04:57.000000 acryo-0.2.3/acryo/alignment/_concrete.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.290294 acryo-0.2.3/acryo/classification/
+-rw-rw-rw-   0        0        0       62 2022-04-12 15:56:50.000000 acryo-0.2.3/acryo/classification/__init__.py
+-rw-rw-rw-   0        0        0    18578 2023-02-08 03:31:15.000000 acryo-0.2.3/acryo/classification/_dask_pca.py
+-rw-rw-rw-   0        0        0     5185 2023-02-21 02:27:31.000000 acryo-0.2.3/acryo/classification/pca.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.314296 acryo-0.2.3/acryo/loader/
+-rw-rw-rw-   0        0        0      187 2023-02-19 15:38:13.000000 acryo-0.2.3/acryo/loader/__init__.py
+-rw-rw-rw-   0        0        0    36831 2023-04-18 09:04:57.000000 acryo-0.2.3/acryo/loader/_base.py
+-rw-rw-rw-   0        0        0     7099 2023-02-26 13:13:09.000000 acryo-0.2.3/acryo/loader/_batch.py
+-rw-rw-rw-   0        0        0     1696 2023-02-21 08:34:02.000000 acryo-0.2.3/acryo/loader/_cache.py
+-rw-rw-rw-   0        0        0    17909 2023-02-27 14:09:35.000000 acryo-0.2.3/acryo/loader/_group.py
+-rw-rw-rw-   0        0        0     9034 2023-02-25 12:12:36.000000 acryo-0.2.3/acryo/loader/_loader.py
+-rw-rw-rw-   0        0        0     2222 2023-02-24 06:22:10.000000 acryo-0.2.3/acryo/loader/_misc.py
+-rw-rw-rw-   0        0        0     9986 2023-03-15 04:51:58.000000 acryo-0.2.3/acryo/loader/_mock.py
+-rw-rw-rw-   0        0        0    34451 2023-04-09 13:27:24.000000 acryo-0.2.3/acryo/molecules.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.324302 acryo-0.2.3/acryo/pick/
+-rw-rw-rw-   0        0        0      129 2023-03-02 06:44:45.000000 acryo-0.2.3/acryo/pick/__init__.py
+-rw-rw-rw-   0        0        0     4680 2023-03-02 06:44:45.000000 acryo-0.2.3/acryo/pick/_base.py
+-rw-rw-rw-   0        0        0     4799 2023-03-02 06:44:45.000000 acryo-0.2.3/acryo/pick/_concrete.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.342293 acryo-0.2.3/acryo/pipe/
+-rw-rw-rw-   0        0        0      647 2023-02-23 14:49:44.000000 acryo-0.2.3/acryo/pipe/__init__.py
+-rw-rw-rw-   0        0        0    12167 2023-02-23 11:14:01.000000 acryo-0.2.3/acryo/pipe/_classes.py
+-rw-rw-rw-   0        0        0     3843 2023-02-25 03:55:45.000000 acryo-0.2.3/acryo/pipe/_curry.py
+-rw-rw-rw-   0        0        0     5436 2023-02-23 15:13:40.000000 acryo-0.2.3/acryo/pipe/_imread.py
+-rw-rw-rw-   0        0        0     3459 2023-02-23 11:14:00.000000 acryo-0.2.3/acryo/pipe/_masking.py
+-rw-rw-rw-   0        0        0     1215 2023-02-25 03:55:55.000000 acryo-0.2.3/acryo/pipe/_transform.py
+-rw-rw-rw-   0        0        0    13577 2023-02-18 15:53:02.000000 acryo-0.2.3/acryo/simulator.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.351293 acryo-0.2.3/acryo/testing/
+-rw-rw-rw-   0        0        0      130 2022-04-15 01:53:16.000000 acryo-0.2.3/acryo/testing/__init__.py
+-rw-rw-rw-   0        0        0     1145 2022-05-02 14:08:55.000000 acryo-0.2.3/acryo/testing/_templates.py
+-rw-rw-rw-   0        0        0     4432 2023-03-02 06:44:45.000000 acryo-0.2.3/acryo/testing/core.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.270211 acryo-0.2.3/acryo.egg-info/
+-rw-rw-rw-   0        0        0     2301 2023-04-18 14:37:24.000000 acryo-0.2.3/acryo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1168 2023-04-18 14:37:25.000000 acryo-0.2.3/acryo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 14:37:24.000000 acryo-0.2.3/acryo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-04-18 14:37:24.000000 acryo-0.2.3/acryo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-18 14:37:24.000000 acryo-0.2.3/acryo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 14:37:25.380998 acryo-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      820 2023-04-18 09:04:57.000000 acryo-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 14:37:25.375489 acryo-0.2.3/tests/
+-rw-rw-rw-   0        0        0     5448 2023-04-18 09:04:57.000000 acryo-0.2.3/tests/test_alignment.py
+-rw-rw-rw-   0        0        0     2602 2023-02-21 08:34:02.000000 acryo-0.2.3/tests/test_batch.py
+-rw-rw-rw-   0        0        0     1360 2023-02-21 08:34:02.000000 acryo-0.2.3/tests/test_cache.py
+-rw-rw-rw-   0        0        0     1736 2023-02-23 14:27:37.000000 acryo-0.2.3/tests/test_group.py
+-rw-rw-rw-   0        0        0     6716 2023-02-24 04:50:51.000000 acryo-0.2.3/tests/test_molecules.py
+-rw-rw-rw-   0        0        0      691 2023-02-21 11:08:36.000000 acryo-0.2.3/tests/test_pipe.py
+-rw-rw-rw-   0        0        0     1545 2023-01-29 13:16:40.000000 acryo-0.2.3/tests/test_simulator.py
+-rw-rw-rw-   0        0        0      542 2023-02-14 03:49:57.000000 acryo-0.2.3/tests/test_utils.py
```

### Comparing `acryo-0.2.2/LICENSE` & `acryo-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/PKG-INFO` & `acryo-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acryo
-Version: 0.2.2
+Version: 0.2.3
 Summary: An extensible cryo-EM/ET toolkit for Python.
 Author: Hanjin Liu
 Author-email: liuhanjin-sc@g.ecc.u-tokyo.ac.jp
 License: BSD 3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `acryo-0.2.2/README.md` & `acryo-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/_correlation.py` & `acryo-0.2.3/acryo/_correlation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,53 @@
 from __future__ import annotations
 from functools import lru_cache
-from typing import Sequence
+from typing import Sequence, TypeVar
 import numpy as np
 from numpy.typing import NDArray
 
 from scipy.signal import fftconvolve
 from scipy import ndimage as ndi
 
 from acryo._fft import ifftn
 from acryo._types import pixel
 
 # cross correlation
 # Modified from skimage/registration/_phase_cross_correlation.py
 
 
+def pcc_landscape(
+    f0: NDArray[np.complex64],
+    f1: NDArray[np.complex64],
+    max_shifts: tuple[float, ...] | None = None,
+):
+    product = f0 * f1.conj()
+    power = _abs2(ifftn(product))
+    power = np.fft.fftshift(power)
+    if max_shifts is not None:
+        centers = tuple(s // 2 for s in power.shape)
+        slices = tuple(
+            slice(max(c - int(shiftl), 0), min(c + int(shiftr) + 1, s), None)
+            for c, shiftl, shiftr, s in zip(
+                centers, max_shifts, max_shifts, power.shape
+            )
+        )
+        power = power[slices]
+    return power
+
+
 def subpixel_pcc(
     f0: NDArray[np.complex64],
     f1: NDArray[np.complex64],
     upsample_factor: int,
     max_shifts: tuple[float, ...] | NDArray[np.number] | None = None,
 ) -> tuple[NDArray[np.float32], float]:
     if isinstance(max_shifts, (int, float)):
         max_shifts = (max_shifts,) * f0.ndim
     product = f0 * f1.conj()
-    power = abs2(ifftn(product))
+    power = _abs2(ifftn(product))
     if max_shifts is not None:
         max_shifts = np.asarray(max_shifts)
         power = crop_by_max_shifts(power, max_shifts, max_shifts)
 
     maxima = np.unravel_index(np.argmax(power), power.shape)
     midpoints = np.array([np.fix(axis_size / 2) for axis_size in power.shape])
 
@@ -38,15 +58,15 @@
     if upsample_factor > 1:
         upsampled_region_size = np.ceil(upsample_factor * 1.5)
         # Center of output array at dftshift + 1
         dftshift = np.fix(upsampled_region_size / 2.0)
         # Matrix multiply DFT around the current shift estimate
         sample_region_offset = dftshift - shifts * upsample_factor
         # Locate maximum and map back to original pixel grid
-        power = abs2(
+        power = _abs2(
             _upsampled_dft(
                 product.conj(),
                 upsampled_region_size,
                 upsample_factor,
                 sample_region_offset,
             )
         )
@@ -86,19 +106,22 @@
         )
         kernel = np.exp(-2j * np.pi * kernel)
 
         data = np.tensordot(kernel, data, axes=(1, -1))  # type: ignore
     return data
 
 
-def abs2(a: NDArray[np.number]) -> NDArray[np.number]:
+_DType = TypeVar("_DType", bound=np.number)
+
+
+def _abs2(a: NDArray[np.complex64]) -> NDArray[np.float32]:
     return a.real**2 + a.imag**2
 
 
-def crop_by_max_shifts(power: np.ndarray, left, right):
+def crop_by_max_shifts(power: NDArray[_DType], left, right) -> NDArray[_DType]:
     shifted_power = np.fft.fftshift(power)
     centers = tuple(s // 2 for s in power.shape)
     slices = tuple(
         slice(max(c - int(shiftl), 0), min(c + int(shiftr) + 1, s), None)
         for c, shiftl, shiftr, s in zip(centers, left, right, power.shape)
     )
     return np.fft.ifftshift(shifted_power[slices])
@@ -169,14 +192,30 @@
     mask = var > 0
     response[mask] = (corr - win_sum1 * template_mean)[mask] / _safe_sqrt(
         var, fill=np.inf
     )[mask]
     return response
 
 
+def zncc_landscape_with_crop(
+    img0: NDArray[np.float32],
+    img1: NDArray[np.float32],
+    max_shifts: tuple[float, ...] | None = None,
+):
+    response = ncc_landscape(img0 - img0.mean(), img1 - img1.mean(), max_shifts)
+    if max_shifts is None:
+        pad_width_eff = (3,) * img1.ndim
+    else:
+        pad_width_eff = tuple(
+            (s - int(m) * 2 - 1) // 2 for m, s in zip(max_shifts, response.shape)
+        )
+    sl_res = tuple(slice(w, -w, None) for w in pad_width_eff)
+    return response[sl_res]
+
+
 def subpixel_zncc(
     img0: NDArray[np.float32],
     img1: NDArray[np.float32],
     upsample_factor: int,
     max_shifts: pixel | tuple[pixel, ...] | None = None,
 ) -> tuple[np.ndarray, float]:
     img0 -= img0.mean()
```

### Comparing `acryo-0.2.2/acryo/_fft.py` & `acryo-0.2.3/acryo/_fft.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/_reader.py` & `acryo-0.2.3/acryo/_reader.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/_rotation.py` & `acryo-0.2.3/acryo/_rotation.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/_utils.py` & `acryo-0.2.3/acryo/_utils.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/alignment/_base.py` & `acryo-0.2.3/acryo/alignment/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # pyright: reportPrivateImportUsage=false
 
 from __future__ import annotations
 from abc import ABC, abstractmethod
+from functools import lru_cache
 from typing import (
     Callable,
     Iterable,
     NamedTuple,
     Sequence,
     TYPE_CHECKING,
     TypeVar,
     Union,
 )
 from typing_extensions import Self
 import inspect
+import warnings
 
 import numpy as np
 from numpy.typing import NDArray
 from scipy import ndimage as ndi
 from scipy.spatial.transform import Rotation
 from dask import array as da, delayed
 
@@ -25,14 +27,15 @@
 from acryo._utils import (
     compose_matrices,
     missing_wedge_mask,
     lowpass_filter_ft,
     delayed_affine,
 )
 from acryo._fft import ifftn
+from ._bound import ParametrizedModel
 
 if TYPE_CHECKING:
     from dask.delayed import Delayed
 
 
 TemplateType = Union[NDArray[np.float32], Sequence[NDArray[np.float32]]]
 MaskType = Union[
@@ -129,43 +132,44 @@
                     "Shape mismatch in between template image "
                     f"{self._template.shape[-self._ndim :]} and mask image {mask.shape})."
                 )
             if mask.dtype not in (np.float32, np.bool_):
                 mask = mask.astype(np.float32)
             self._mask = mask
 
-        self._align_func = self._get_alignment_function()
         self._template_input, self._mask_input = self._get_template_and_mask_input()
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(shape={self._template.shape})"
 
     @property
     def template(self) -> NDArray[np.float32]:
+        """The template image."""
         return self._template
 
     @property
     def mask(self) -> NDArray[np.float32]:
+        """The mask image."""
         return self._mask
 
     @property
     def input_shape(self) -> tuple[int, ...]:
         """Return the array shape of input images and template."""
         return self._template.shape[-self._ndim :]
 
     @classmethod
     def with_params(
         cls,
         **params,
-    ) -> Callable[[TemplateType, NDArray[np.float32] | None], Self]:
+    ):
         """Create a BaseAlignmentModel instance with parameters."""
-        return _with_params(cls, **params)
+        return ParametrizedModel(cls, **params)
 
     @abstractmethod
-    def optimize(
+    def _optimize(
         self,
         subvolume: NDArray[np.complex64],
         template: NDArray[np.complex64],
         max_shifts: tuple[float, ...],
         quaternion: NDArray[np.float32],
         pos: NDArray[np.float32],
     ) -> tuple[NDArray[np.float32], NDArray[np.float32], float]:
@@ -199,14 +203,27 @@
               better results.
         """
 
     @abstractmethod
     def pre_transform(self, image: NDArray[np.float32]) -> NDArray[np.complex64]:
         """Pre-transformation applied to input images (including template)."""
 
+    def _landscape(
+        self,
+        subvolume: NDArray[np.complex64],
+        template: NDArray[np.complex64],
+        max_shifts: tuple[float, ...],
+        quaternion: NDArray[np.float32],
+        pos: NDArray[np.float32],
+    ) -> NDArray[np.float32]:
+        """Return the landscape of the subvolume."""
+        raise NotImplementedError(
+            f"_landscape method is not implemented for {type(self).__name__}."
+        )
+
     def _get_template_and_mask_input(
         self,
     ) -> tuple[NDArray[np.complex64], NDArray[np.float32]]:
         """
         Returns proper template and mask images for alignment.
 
         Template dimensionality will be dispatched according to the input
@@ -217,15 +234,15 @@
         -------
         array
             Template image(s) and mask image(s). Its axes varies depending on the input.
 
             - single template image ... 3D
             - many template images ... 4D
         """
-        if self.is_multi_templates:
+        if self._n_templates > 1:
             template_input = np.stack(
                 [self.pre_transform(tmp * self._mask) for tmp in self._template],
                 axis=0,
             )
         else:
             template_input = self.pre_transform(self._template * self._mask)
         return template_input, self._mask
@@ -256,15 +273,20 @@
             _quat = self._DUMMY_QUAT
         else:
             _quat = quaternion
         if pos is None:
             _pos = self._DUMMY_POS
         else:
             _pos = pos
-        return self._align_func(
+
+        if self._is_multiple():
+            _align_fn = self._optimize_multiple
+        else:
+            _align_fn = self._optimize_single
+        return _align_fn(
             img,
             self._template_input,
             self._mask_input,
             max_shifts,
             _quat,
             _pos,
         )
@@ -294,24 +316,127 @@
         """
         result = self.align(img, max_shifts=max_shifts, quaternion=None, pos=None)
         mtx = result.affine_matrix(img.shape)
         _cval = _normalize_cval(cval, img)
         img_trans: NDArray[np.float32] = ndi.affine_transform(img, mtx, cval=_cval)  # type: ignore
         return img_trans, result
 
+    def landscape(
+        self,
+        img: NDArray[np.float32],
+        max_shifts: tuple[float, float, float],
+        quaternion: NDArray[np.float32] | None = None,
+        pos: NDArray[np.float32] | None = None,
+        upsample: int = 1,
+    ) -> NDArray[np.float32]:
+        """
+        Calculate correlation landscape of the input image.
+
+        Parameters
+        ----------
+        img : np.ndarray
+            Subvolume for the landscape calculation.
+        max_shifts : tuple[float, float, float]
+            Maximum shifts along z, y, x axis in pixel.
+
+        Returns
+        -------
+        np.ndarray
+            N (if single template) or N+1 (if multi-template) dimensional array of
+            correlation landscape.
+        """
+        if quaternion is None:
+            _quat = self._DUMMY_QUAT
+        else:
+            _quat = quaternion
+        if pos is None:
+            _pos = self._DUMMY_POS
+        else:
+            _pos = pos
+        if self._is_multiple():
+            fn = self._landscape_multiple
+        else:
+            fn = self._landscape_single
+
+        # calculate the landscape
+        lds = fn(
+            img,
+            self._template_input,
+            self._mask_input,
+            max_shifts,
+            _quat,
+            _pos,
+        )
+        
+        if upsample > 1:
+            if not self._is_multiple():
+                coords = _create_mesh_for_landscape(lds.shape, max_shifts, upsample)
+                lds_upsampled = ndi.map_coordinates(
+                    lds, coords, order=3, mode="constant", cval=0., prefilter=True
+                )
+            else:
+                coords = _create_mesh_for_landscape(lds.shape[1:], max_shifts, upsample)
+                all_lds = [
+                    ndi.map_coordinates(
+                        l, coords, order=3, mode="constant", cval=0., prefilter=True
+                    )
+                    for l in lds
+                ]
+                lds_upsampled = np.stack(all_lds, axis=0)
+            return lds_upsampled
+        return lds
+
+    def _landscape_single(
+        self,
+        subvolume: NDArray[np.float32],
+        template: NDArray[np.complex64],
+        mask: NDArray[np.float32],
+        max_shifts: tuple[float, ...],
+        quaternion: NDArray[np.float32],
+        pos: NDArray[np.float32],
+    ):
+        return self._landscape(
+            self.pre_transform(subvolume * mask),
+            template,
+            max_shifts=max_shifts,
+            quaternion=quaternion,
+            pos=pos,
+        )
+
+    def _landscape_multiple(
+        self,
+        subvolume: NDArray[np.float32],
+        template_list: Iterable[NDArray[np.complex64]],
+        mask_list: Iterable[NDArray[np.float32]],
+        max_shifts: tuple[float, float, float],
+        quaternion: NDArray[np.float32],
+        pos: NDArray[np.float32],
+    ):
+        out: list[NDArray[np.float32]] = []
+        for template, mask in zip(template_list, mask_list):
+            lnd = self._landscape(
+                self.pre_transform(subvolume * mask),
+                template,
+                max_shifts=max_shifts,
+                quaternion=quaternion,
+                pos=pos,
+            )
+            out.append(lnd)
+        return np.stack(out, axis=0)
+
     def _optimize_single(
         self,
         subvolume: NDArray[np.float32],
         template: NDArray[np.complex64],
         mask: NDArray[np.float32],
         max_shifts: tuple[float, float, float],
         quaternion: NDArray[np.float32],
         pos: NDArray[np.float32],
     ) -> AlignmentResult:
-        out = self.optimize(
+        out = self._optimize(
             self.pre_transform(subvolume * mask),
             template,
             max_shifts=max_shifts,
             quaternion=quaternion,
             pos=pos,
         )
         return AlignmentResult(0, *out)
@@ -325,41 +450,50 @@
         quaternion: NDArray[np.float32],
         pos: NDArray[np.float32],
     ) -> AlignmentResult:
         all_shifts: list[np.ndarray] = []
         all_quat: list[np.ndarray] = []
         all_score: list[float] = []
         for template, mask in zip(template_list, mask_list):
-            shift, quat, score = self.optimize(
+            shift, quat, score = self._optimize(
                 self.pre_transform(subvolume * mask),
                 template,
                 max_shifts=max_shifts,
                 quaternion=quaternion,
                 pos=pos,
             )
             all_shifts.append(shift)
             all_quat.append(quat)
             all_score.append(score)
 
         iopt = int(np.argmax(all_score))
         return AlignmentResult(iopt, all_shifts[iopt], all_quat[iopt], all_score[iopt])
 
-    def _get_alignment_function(self):
-        if self.is_multi_templates:
-            return self._optimize_multiple
-        else:
-            return self._optimize_single
+    def _is_multiple(self) -> bool:
+        return self.niter > 1
 
     @property
     def is_multi_templates(self) -> bool:
         """
         Whether alignment parameters requires multi-templates.
         "Multi-template" includes alignment with subvolume rotation.
         """
-        return self._n_templates > 1
+        return self._is_multiple()
+
+    @property
+    def niter(self) -> int:
+        """Number of templates."""
+        return self._n_templates
+
+# deprecated
+def optimize(self: BaseAlignmentModel, *args, **kwargs):
+    warnings.warn(
+        "`optimize` is deprecated. It is now a private method.", DeprecationWarning
+    )
+    return self._optimize(*args, **kwargs)
 
 
 class RotationImplemented(BaseAlignmentModel):
     """
     An alignment model implemented with default rotation optimizer.
 
     If ``optimize`` does not support rotation optimization, this class implements
@@ -378,17 +512,22 @@
         super().__init__(template=template, mask=mask)
 
     @classmethod
     def with_params(
         cls,
         *,
         rotations: Ranges | None = None,
-    ) -> Callable[[TemplateType, NDArray[np.float32] | None], Self]:
+    ) -> ParametrizedModel[Self]:
         """Create an alignment model instance with parameters."""
-        return _with_params(cls, rotations=rotations)
+        return ParametrizedModel(cls, rotations=rotations)
+
+    @property
+    def has_rotation(self) -> bool:
+        """If the alignment model has rotation optimization."""
+        return self._n_rotations > 1
 
     def align(
         self,
         img: NDArray[np.float32],
         max_shifts: tuple[subpixel, subpixel, subpixel],
         quaternion: NDArray[np.float32] | None,
         pos: NDArray[np.float32] | None,
@@ -434,15 +573,15 @@
             Constant value for padding.
 
         Returns
         -------
         np.ndarray, AlignmentResult
             Transformed input image and the alignment result.
         """
-        delayed_optimize = delayed(self.optimize)
+        delayed_optimize = delayed(self._optimize)
         tasks: list[Delayed] = []
         for quat, tmp, mask in zip(
             self.quaternions, self._template_input, self._mask_input
         ):
             task = delayed_optimize(
                 self.pre_transform(img * mask),
                 tmp,
@@ -518,15 +657,15 @@
         """
         if self._n_rotations > 1:
             rotators = [Rotation.from_quat(r).inv() for r in self.quaternions]
             matrices = compose_matrices(
                 np.array(self._template.shape[-3:]) / 2 - 0.5, rotators
             )
             cval = float(np.percentile(self._template, 1))
-            if self.is_multi_templates:
+            if self._n_templates > 1:
                 all_templates: list[da.Array] = []
                 all_masks: list[da.Array] = []
                 inputs_templates: list[NDArray[np.float32]] = [
                     ndi.spline_filter(
                         tmp * self._mask,
                         order=3,
                         mode="constant",
@@ -586,15 +725,15 @@
                     for mat in matrices
                 ]
                 template_input, mask_input = da.compute(
                     da.stack(all_templates, axis=0), da.stack(all_masks, axis=0)
                 )
         else:
             delayed_transform = delayed(self.pre_transform)
-            if self.is_multi_templates:
+            if self._n_templates > 1:
                 template_input = da.stack(
                     [
                         da.from_delayed(
                             delayed_transform(tmp * self._mask),
                             shape=tmp.shape,
                             dtype=np.complex64,
                         )
@@ -609,20 +748,21 @@
                 template_input = delayed_transform(
                     self._template * self._mask
                 ).compute()
                 mask_input = self._mask
 
         return template_input, mask_input
 
-    def _get_alignment_function(self):
-        if self.is_multi_templates or self._n_rotations > 1:
-            return self._optimize_multiple
-        else:
-            return self._optimize_single
+    def _is_multiple(self) -> bool:
+        return self._n_templates * self._n_rotations > 1
 
+    @property
+    def niter(self) -> int:
+        """Number of iteration per sub-volume."""
+        return self._n_templates * self._n_rotations
 
 class TomographyInput(RotationImplemented):
     """
     An alignment model that implements missing-wedge masking and low-pass filter.
 
     This alignment model is useful for subtomogram averaging of real experimental
     data with limited tilt ranges. Template image will be masked with synthetic
@@ -648,17 +788,17 @@
     @classmethod
     def with_params(
         cls,
         *,
         rotations: Ranges | None = None,
         cutoff: float | None = None,
         tilt_range: tuple[degree, degree] | None = None,
-    ) -> Callable[[TemplateType, NDArray[np.float32] | None], Self]:
+    ) -> ParametrizedModel[Self]:
         """Create an alignment model instance with parameters."""
-        return _with_params(
+        return ParametrizedModel(
             cls,
             rotations=rotations,
             cutoff=cutoff,
             tilt_range=tilt_range,
         )
 
     def pre_transform(self, image: NDArray[np.float32]) -> NDArray[np.complex64]:
@@ -682,15 +822,15 @@
             object.
 
         Returns
         -------
         3D array
             Difference map.
         """
-        if self.is_multi_templates:
+        if self._n_templates > 1:
             raise NotImplementedError(
                 "Masked difference is not implemented for multi-template."
             )
         ft = self._template_input  # NOTE: ft.ndim == 3
         ft[:] = self.mask_missing_wedge(ft, quaternion)
         template_masked = np.real(ifftn(ft))
         img_input = np.real(ifftn(self.pre_transform(image * self._mask)))
@@ -733,17 +873,21 @@
     if cval is None:
         _cval = float(np.percentile(img, 1))
     else:
         _cval = cval
     return _cval
 
 
-_T = TypeVar("_T", bound=BaseAlignmentModel)
-
-
-def _with_params(
-    cls: type[_T],
-    **params,
-) -> Callable[[TemplateType, NDArray[np.float32] | None], _T]:
-    """Create a BaseAlignmentModel instance with parameters."""
-    bound = inspect.signature(cls).bind_partial(**params)
-    return lambda template, mask: cls(template, mask, *bound.args, **bound.kwargs)
+@lru_cache(maxsize=2)
+def _create_mesh_for_landscape(
+    shape: tuple[int, int, int], 
+    max_shifts: tuple[float, float, float], 
+    upsample: int,
+) -> NDArray[np.float32]:
+    upsampled_max_shifts = (np.asarray(max_shifts) * upsample).astype(np.int32)
+    center = np.array(shape) / 2 - 0.5
+    mesh = np.meshgrid(
+        *[np.arange(-width, width + 1) / upsample + c
+        for c, width in zip(center, upsampled_max_shifts)], 
+        indexing="ij",
+    )
+    return np.stack(mesh, axis=0)
```

### Comparing `acryo-0.2.2/acryo/classification/_dask_pca.py` & `acryo-0.2.3/acryo/classification/_dask_pca.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/classification/pca.py` & `acryo-0.2.3/acryo/classification/pca.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/loader/_base.py` & `acryo-0.2.3/acryo/loader/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,14 +424,16 @@
             Additional keyword arguments passed to the input alignment model.
 
         Returns
         -------
         subtomogram loader object
             A loader instance of the same type with updated molecules.
         """
+        if np.isscalar(max_shifts):
+            max_shifts = (max_shifts,) * 3
         _max_shifts_px = np.asarray(max_shifts) / self.scale
 
         model = alignment_model(
             template=self.normalize_template(template),
             mask=self.normalize_mask(mask),
             **align_kwargs,
         )
@@ -605,14 +607,58 @@
         feature_list = _misc.get_feature_list(scores, local_shifts, rotator.as_rotvec())
         mole_aligned.features = self.molecules.features.with_columns(
             feature_list + [pl.Series(label_name, labels)]
         )
 
         return self.replace(molecules=mole_aligned, output_shape=shape)
 
+    def construct_landscape(
+        self,
+        template: TemplateInputType,
+        *,
+        mask: MaskInputType = None,
+        max_shifts: nm | tuple[nm, nm, nm] = 1.0,
+        alignment_model: type[BaseAlignmentModel] | AlignmentFactory = ZNCCAlignment,
+        upsample: int = 1,
+        **align_kwargs,
+    ) -> da.Array:
+        """
+        Construct a dask array of correlation landscape.
+
+        This method internally calls the ``landscape`` method of the input alignment
+        model.
+        """
+        if np.isscalar(max_shifts):
+            max_shifts = (max_shifts,) * 3
+        _max_shifts_px = tuple(np.asarray(max_shifts) / self.scale)
+
+        model = alignment_model(
+            template=self.normalize_template(template),
+            mask=self.normalize_mask(mask),
+            **align_kwargs,
+        )
+
+        if model.is_multi_templates:
+            task_shape = (model.niter,) + tuple(2 * np.ceil(_max_shifts_px).astype(np.int32) + 1)
+        else:
+            task_shape = tuple(2 * np.ceil(_max_shifts_px).astype(np.int32) + 1)
+        task_arrays: list[da.Array] = [
+            da.from_delayed(task, shape=task_shape, dtype=np.float32)
+            for task in self.iter_mapping_tasks(
+                model.landscape,
+                max_shifts=_max_shifts_px,
+                upsample=upsample,
+                var_kwarg=dict(
+                    quaternion=self.molecules.quaternion(),
+                    pos=self.molecules.pos / self.scale,
+                )
+            )
+        ]
+        return da.stack(task_arrays, axis=0)
+
     def apply(
         self,
         func: AggFunction | Iterable[AggFunction],
         schema: list[str] | None = None,
     ) -> pl.DataFrame:
         """
         Apply functions to subtomograms.
```

### Comparing `acryo-0.2.2/acryo/loader/_batch.py` & `acryo-0.2.3/acryo/loader/_batch.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/loader/_cache.py` & `acryo-0.2.3/acryo/loader/_cache.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/loader/_group.py` & `acryo-0.2.3/acryo/loader/_group.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/loader/_loader.py` & `acryo-0.2.3/acryo/loader/_loader.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/loader/_misc.py` & `acryo-0.2.3/acryo/loader/_misc.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/loader/_mock.py` & `acryo-0.2.3/acryo/loader/_mock.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/molecules.py` & `acryo-0.2.3/acryo/molecules.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/pick/_base.py` & `acryo-0.2.3/acryo/pick/_base.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/pick/_concrete.py` & `acryo-0.2.3/acryo/pick/_concrete.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/pipe/__init__.py` & `acryo-0.2.3/acryo/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/pipe/_classes.py` & `acryo-0.2.3/acryo/pipe/_classes.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/pipe/_curry.py` & `acryo-0.2.3/acryo/pipe/_curry.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/pipe/_imread.py` & `acryo-0.2.3/acryo/pipe/_imread.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/pipe/_masking.py` & `acryo-0.2.3/acryo/pipe/_masking.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/pipe/_transform.py` & `acryo-0.2.3/acryo/pipe/_transform.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/simulator.py` & `acryo-0.2.3/acryo/simulator.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/testing/_templates.py` & `acryo-0.2.3/acryo/testing/_templates.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo/testing/core.py` & `acryo-0.2.3/acryo/testing/core.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/acryo.egg-info/PKG-INFO` & `acryo-0.2.3/acryo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acryo
-Version: 0.2.2
+Version: 0.2.3
 Summary: An extensible cryo-EM/ET toolkit for Python.
 Author: Hanjin Liu
 Author-email: liuhanjin-sc@g.ecc.u-tokyo.ac.jp
 License: BSD 3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `acryo-0.2.2/acryo.egg-info/SOURCES.txt` & `acryo-0.2.3/acryo.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 acryo.egg-info/PKG-INFO
 acryo.egg-info/SOURCES.txt
 acryo.egg-info/dependency_links.txt
 acryo.egg-info/requires.txt
 acryo.egg-info/top_level.txt
 acryo/alignment/__init__.py
 acryo/alignment/_base.py
+acryo/alignment/_bound.py
 acryo/alignment/_concrete.py
 acryo/classification/__init__.py
 acryo/classification/_dask_pca.py
 acryo/classification/pca.py
 acryo/loader/__init__.py
 acryo/loader/_base.py
 acryo/loader/_batch.py
```

### Comparing `acryo-0.2.2/setup.py` & `acryo-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,13 +18,13 @@
     author="Hanjin Liu",
     author_email="liuhanjin-sc@g.ecc.u-tokyo.ac.jp",
     license="BSD 3-Clause",
     packages=find_packages(exclude=["tests", "tests.*"]),
     install_requires=[
         "numpy>=1.21",
         "scipy>=1.7.3",
-        "polars>=0.16.18",
+        "polars>=0.17.3",
         "dask>=2021.6.0",
         "typing_extensions>=4.1.1",
     ],
     python_requires=">=3.8",
 )
```

### Comparing `acryo-0.2.2/tests/test_alignment.py` & `acryo-0.2.3/tests/test_alignment.py`

 * *Files 21% similar despite different names*

```diff
@@ -48,26 +48,64 @@
     )
     loader.fsc()
     loader.fsc(mask=(temp > np.mean(temp)).astype(np.float32))
 
 
 @pytest.mark.parametrize("shift", [[1, 2, 2], [-4, 3, 2]])
 @pytest.mark.parametrize("rot", [[15, 0, 15], [-15, 15, 15], [0, 0, -15]])
-def test_fit(shift, rot):
+@pytest.mark.parametrize("alignment_model", [ZNCCAlignment, PCCAlignment])
+def test_fit(shift, rot, alignment_model: "type[BaseAlignmentModel]"):
     rotations = ((15, 15), (15, 15), (15, 15))
-    model = ZNCCAlignment(temp, rotations=rotations)
+    model = alignment_model(temp, rotations=rotations)
     temp_transformed = temp * 4 + np.mean(temp)  # linear transformation to input image
     img = ndi.shift(rotate(temp_transformed, rot, cval=np.min), shift=shift)
-    imgout, result = model.fit(img, (5, 5, 5))  # type: ignore
+    imgout, result = model.fit(img, (5, 5, 5))
     assert_allclose(result.quat, euler_to_quat(rot))
     assert_allclose(result.shift, shift)
     coef = np.corrcoef(imgout.ravel(), temp.ravel())
     assert coef[0, 1] > 0.95  # check results are well aligned
 
 
+@pytest.mark.parametrize("shift", [[1, 2, 2], [-4, 3, 2]])
+@pytest.mark.parametrize("alignment_model", [ZNCCAlignment, PCCAlignment])
+@pytest.mark.parametrize("upsample", [1, 2])
+def test_landscape(shift, alignment_model: "type[BaseAlignmentModel]", upsample):
+    model = alignment_model(temp)
+    temp_transformed = temp * 4 + np.mean(temp)  # linear transformation to input image
+    img = ndi.shift(temp_transformed, shift=shift)
+    lnd = model.landscape(img, (5, 5, 5), upsample=upsample)
+    maxima = np.unravel_index(np.argmax(lnd), lnd.shape)
+    assert_allclose((np.array(maxima) - 5 * upsample) / upsample, shift)
+
+def test_with_params():
+    model = ZNCCAlignment.with_params(rotations=((15, 15), (15, 15), (15, 15)), cutoff=0.4)
+    assert model.quaternions.shape == (27, 4)
+    assert type(model(temp)) is ZNCCAlignment
+
+@pytest.mark.parametrize("upsample", [1, 2])
+def test_landscape_in_loader(upsample):
+    loader = SubtomogramLoader(
+        tomo, mole, order=0, scale=scale, output_shape=temp.shape
+    )
+    mask = temp > np.mean(temp)
+    arr: np.ndarray = loader.construct_landscape(temp, mask=mask, upsample=upsample, max_shifts=1.0).compute()
+    assert arr.shape == (len(mole), 6 * upsample + 1, 6 * upsample + 1, 6 * upsample + 1)
+
+@pytest.mark.parametrize("upsample", [1, 2])
+def test_landscape_in_loader_with_rotation(upsample):
+    loader = SubtomogramLoader(
+        tomo, mole, order=0, scale=scale, output_shape=temp.shape
+    )
+    mask = temp > np.mean(temp)
+    arr: np.ndarray = loader.construct_landscape(
+        temp, mask=mask, upsample=upsample, max_shifts=1.0, rotations=((15, 15), (15, 15), (15, 15))
+    ).compute()
+    assert arr.shape == (len(mole), 27, 6 * upsample + 1, 6 * upsample + 1, 6 * upsample + 1)
+
+
 def test_pca_classify():
     loader = SubtomogramLoader(
         tomo, mole, order=0, scale=scale, output_shape=temp.shape
     )
     mask = temp > np.mean(temp)
     loader.classify(mask.astype(np.float32), tilt_range=(-60, 60))
```

### Comparing `acryo-0.2.2/tests/test_batch.py` & `acryo-0.2.3/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/tests/test_cache.py` & `acryo-0.2.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/tests/test_group.py` & `acryo-0.2.3/tests/test_group.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/tests/test_molecules.py` & `acryo-0.2.3/tests/test_molecules.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/tests/test_pipe.py` & `acryo-0.2.3/tests/test_pipe.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/tests/test_simulator.py` & `acryo-0.2.3/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `acryo-0.2.2/tests/test_utils.py` & `acryo-0.2.3/tests/test_utils.py`

 * *Files identical despite different names*

