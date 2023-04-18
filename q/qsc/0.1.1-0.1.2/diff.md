# Comparing `tmp/qsc-0.1.1.tar.gz` & `tmp/qsc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qsc-0.1.1.tar", last modified: Wed Jun  8 14:39:30 2022, max compression
+gzip compressed data, was "dist/qsc-0.1.2.tar", last modified: Tue Apr 18 14:07:31 2023, max compression
```

## Comparing `qsc-0.1.1.tar` & `qsc-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 14:39:30.000000 qsc-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-06-08 14:39:30.000000 qsc-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-06-08 14:39:28.000000 qsc-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 14:39:30.000000 qsc-0.1.1/qsc/
--rw-r--r--   0 runner    (1001) docker     (121)    10523 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/Frenet_to_cylindrical.py
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5618 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/calculate_r1.py
--rw-r--r--   0 runner    (1001) docker     (121)    11444 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/calculate_r2.py
--rw-r--r--   0 runner    (1001) docker     (121)    16789 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/calculate_r3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/fourier_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)    76751 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/grad_B_tensor.py
--rw-r--r--   0 runner    (1001) docker     (121)     8947 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/init_axis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/mercier.py
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/newton.py
--rw-r--r--   0 runner    (1001) docker     (121)    33104 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)    16967 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/qsc.py
--rw-r--r--   0 runner    (1001) docker     (121)    37305 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/r_singularity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/spectral_diff_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 14:39:30.000000 qsc-0.1.1/qsc/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2819 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/tests/test_fourier_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)    11046 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/tests/test_grad_B_tensor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3179 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/tests/test_iota2.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/tests/test_newton.py
--rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)    19153 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/tests/test_qsc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4759 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/tests/test_spectral_diff_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     4424 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/tests/test_to_vmec.py
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     6024 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/to_vmec.py
--rw-r--r--   0 runner    (1001) docker     (121)     5633 2022-06-08 14:39:28.000000 qsc-0.1.1/qsc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 14:39:30.000000 qsc-0.1.1/qsc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-06-08 14:39:30.000000 qsc-0.1.1/qsc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-06-08 14:39:30.000000 qsc-0.1.1/qsc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-08 14:39:30.000000 qsc-0.1.1/qsc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-06-08 14:39:30.000000 qsc-0.1.1/qsc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-08 14:39:30.000000 qsc-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-06-08 14:39:28.000000 qsc-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:31.000000 qsc-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-18 14:07:31.000000 qsc-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-18 14:07:28.000000 qsc-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:31.000000 qsc-0.1.2/qsc/
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/Frenet_to_cylindrical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/calculate_r1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/calculate_r2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/calculate_r3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/fourier_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76751 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/grad_B_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/init_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/mercier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33104 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/qsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37305 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/r_singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/spectral_diff_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:31.000000 qsc-0.1.2/qsc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/tests/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/tests/test_fourier_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/tests/test_grad_B_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/tests/test_iota2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/tests/test_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/tests/test_qsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/tests/test_spectral_diff_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/tests/test_to_vmec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/to_vmec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-04-18 14:07:28.000000 qsc-0.1.2/qsc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:07:31.000000 qsc-0.1.2/qsc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-18 14:07:31.000000 qsc-0.1.2/qsc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-18 14:07:31.000000 qsc-0.1.2/qsc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:07:31.000000 qsc-0.1.2/qsc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-18 14:07:31.000000 qsc-0.1.2/qsc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:07:31.000000 qsc-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-18 14:07:28.000000 qsc-0.1.2/setup.py
```

### Comparing `qsc-0.1.1/PKG-INFO` & `qsc-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Quasisymmetric Stellarator Construction
 Home-page: https://github.com/landreman/pyQSC
 Author: Matt Landreman
 Author-email: matt.landreman@gmail.com
 License: UNKNOWN
 Description: # pyQSC
         Python implementation of the Quasisymmetric Stellarator Construction method
```

### Comparing `qsc-0.1.1/qsc/Frenet_to_cylindrical.py` & `qsc-0.1.2/qsc/Frenet_to_cylindrical.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,24 +100,32 @@
 
     total_R = np.sqrt(total_x * total_x + total_y * total_y)
     total_phi=np.arctan2(total_y, total_x)
 
     return total_R, total_z, total_phi
 
 def Frenet_to_cylindrical(self, r, ntheta=20):
-    """
-    Function to convert the near-axis coordinate system to
-    a cylindrical one for a surface at a particular radius,
-    outputing the following arrays: R(theta,varphi),
-    phi(theta,varphi) and Z(theta,varphi) with R,phi,Z cylindrical
-    coordinates and theta and varphi Boozer coordinates
-
+    r"""
+    For a given minor radius coordinate :math:`r`, compute the
+    shape of the flux surface in standard cylindrical coordinates
+    :math:`(R, \phi, Z)`.  This function returns :math:`R` and
+    :math:`Z` as 2D arrays corresponding to dimensions ``(theta,
+    phi)``, where ``theta`` is the Boozer poloidal angle and ``phi``
+    is the standard toroidal angle.  Also returned is ``phi0(theta,
+    phi)``, defined as follows: for given ``(theta, phi)``, move to
+    the magnetic axis while holding the Boozer poloidal and toroidal
+    angles fixed; the standard toroidal angle at that resulting point
+    on the axis is ``phi0``.
+    
     Args:
-        r:  near-axis radius r of the desired boundary surface
+        r: near-axis radius r of the desired boundary surface
         ntheta: resolution in the poloidal angle theta
+
+    Returns: 3 element tuple containing ``(R, Z, phi0)``. Each entry has shape ``(ntheta, nphi)``.
+
     """
     nphi_conversion = self.nphi
     theta = np.linspace(0,2*np.pi,ntheta,endpoint=False)
     phi_conversion = np.linspace(0,2*np.pi/self.nfp,nphi_conversion,endpoint=False)
     R_2D = np.zeros((ntheta,nphi_conversion))
     Z_2D = np.zeros((ntheta,nphi_conversion))
     phi0_2D = np.zeros((ntheta,nphi_conversion))
@@ -211,8 +219,8 @@
         self.Y_spline = self.convert_to_spline(Y_at_this_theta)
         self.Z_spline = self.convert_to_spline(Z_at_this_theta)
         final_R, final_Z, final_phi = Frenet_to_cylindrical_1_point(phi0, self)
         R.append(final_R)
         Z.append(final_Z)
         phi.append(final_phi)
 
-    return R, Z, phi
+    return R, Z, phi
```

### Comparing `qsc-0.1.1/qsc/calculate_r1.py` & `qsc-0.1.2/qsc/calculate_r1.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/calculate_r2.py` & `qsc-0.1.2/qsc/calculate_r2.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/calculate_r3.py` & `qsc-0.1.2/qsc/calculate_r3.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/fourier_interpolation.py` & `qsc-0.1.2/qsc/fourier_interpolation.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/grad_B_tensor.py` & `qsc-0.1.2/qsc/grad_B_tensor.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/init_axis.py` & `qsc-0.1.2/qsc/init_axis.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/mercier.py` & `qsc-0.1.2/qsc/mercier.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/newton.py` & `qsc-0.1.2/qsc/newton.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/plot.py` & `qsc-0.1.2/qsc/plot.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/r_singularity.py` & `qsc-0.1.2/qsc/r_singularity.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/spectral_diff_matrix.py` & `qsc-0.1.2/qsc/spectral_diff_matrix.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/tests/test_fourier_interpolation.py` & `qsc-0.1.2/qsc/tests/test_fourier_interpolation.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/tests/test_grad_B_tensor.py` & `qsc-0.1.2/qsc/tests/test_grad_B_tensor.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/tests/test_iota2.py` & `qsc-0.1.2/qsc/tests/test_iota2.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/tests/test_newton.py` & `qsc-0.1.2/qsc/tests/test_newton.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/tests/test_plot.py` & `qsc-0.1.2/qsc/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/tests/test_spectral_diff_matrix.py` & `qsc-0.1.2/qsc/tests/test_spectral_diff_matrix.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/tests/test_to_vmec.py` & `qsc-0.1.2/qsc/tests/test_to_vmec.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/tests/test_util.py` & `qsc-0.1.2/qsc/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/to_vmec.py` & `qsc-0.1.2/qsc/to_vmec.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc/util.py` & `qsc-0.1.2/qsc/util.py`

 * *Files identical despite different names*

### Comparing `qsc-0.1.1/qsc.egg-info/PKG-INFO` & `qsc-0.1.2/qsc.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Quasisymmetric Stellarator Construction
 Home-page: https://github.com/landreman/pyQSC
 Author: Matt Landreman
 Author-email: matt.landreman@gmail.com
 License: UNKNOWN
 Description: # pyQSC
         Python implementation of the Quasisymmetric Stellarator Construction method
```

### Comparing `qsc-0.1.1/setup.py` & `qsc-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qsc",
-    version="0.1.1",
+    version="0.1.2",
     author="Matt Landreman",
     author_email="matt.landreman@gmail.com",
     description="Quasisymmetric Stellarator Construction",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url="https://github.com/landreman/pyQSC",
```

