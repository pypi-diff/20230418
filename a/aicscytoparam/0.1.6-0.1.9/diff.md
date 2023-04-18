# Comparing `tmp/aicscytoparam-0.1.6.tar.gz` & `tmp/aicscytoparam-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicscytoparam-0.1.6.tar", last modified: Wed Jun 22 03:29:42 2022, max compression
+gzip compressed data, was "aicscytoparam-0.1.9.tar", last modified: Tue Apr 18 17:42:39 2023, max compression
```

## Comparing `aicscytoparam-0.1.6.tar` & `aicscytoparam-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 03:29:42.359989 aicscytoparam-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6426 2022-06-22 03:29:42.359989 aicscytoparam-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4560 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 03:29:42.359989 aicscytoparam-0.1.6/aicscytoparam/
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/aicscytoparam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 03:29:42.359989 aicscytoparam-0.1.6/aicscytoparam/bin/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/aicscytoparam/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2895 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/aicscytoparam/bin/my_example.py
--rw-r--r--   0 runner    (1001) docker     (121)    19290 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/aicscytoparam/cytoparam.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 03:29:42.359989 aicscytoparam-0.1.6/aicscytoparam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6426 2022-06-22 03:29:42.000000 aicscytoparam-0.1.6/aicscytoparam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-06-22 03:29:42.000000 aicscytoparam-0.1.6/aicscytoparam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-22 03:29:42.000000 aicscytoparam-0.1.6/aicscytoparam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-06-22 03:29:42.000000 aicscytoparam-0.1.6/aicscytoparam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-22 03:29:42.000000 aicscytoparam-0.1.6/aicscytoparam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-06-22 03:29:42.000000 aicscytoparam-0.1.6/aicscytoparam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-22 03:29:42.000000 aicscytoparam-0.1.6/aicscytoparam.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 03:29:42.359989 aicscytoparam-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     5350 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7901 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/docs/im1.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     8518 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/docs/im2.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    11386 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/docs/im3.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)   126983 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/docs/logo.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-06-22 03:29:42.363989 aicscytoparam-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-06-22 03:29:39.000000 aicscytoparam-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:42:39.947347 aicscytoparam-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-04-18 17:42:39.947347 aicscytoparam-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:42:39.947347 aicscytoparam-0.1.9/aicscytoparam/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/aicscytoparam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:42:39.947347 aicscytoparam-0.1.9/aicscytoparam/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/aicscytoparam/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/aicscytoparam/bin/my_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/aicscytoparam/cytoparam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:42:39.947347 aicscytoparam-0.1.9/aicscytoparam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-04-18 17:42:39.000000 aicscytoparam-0.1.9/aicscytoparam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-18 17:42:39.000000 aicscytoparam-0.1.9/aicscytoparam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:42:39.000000 aicscytoparam-0.1.9/aicscytoparam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-18 17:42:39.000000 aicscytoparam-0.1.9/aicscytoparam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:42:39.000000 aicscytoparam-0.1.9/aicscytoparam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-18 17:42:39.000000 aicscytoparam-0.1.9/aicscytoparam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 17:42:39.000000 aicscytoparam-0.1.9/aicscytoparam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:42:39.947347 aicscytoparam-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/docs/im1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/docs/im2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/docs/im3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   126983 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/docs/logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-18 17:42:39.951347 aicscytoparam-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-18 17:42:33.000000 aicscytoparam-0.1.9/setup.py
```

### Comparing `aicscytoparam-0.1.6/CONTRIBUTING.md` & `aicscytoparam-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aicscytoparam-0.1.6/LICENSE` & `aicscytoparam-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aicscytoparam-0.1.6/LICENSE.txt` & `aicscytoparam-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aicscytoparam-0.1.6/PKG-INFO` & `aicscytoparam-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicscytoparam
-Version: 0.1.6
+Version: 0.1.9
 Summary: Cytoplasm parameterization using spherical harmonics
 Home-page: https://github.com/AllenCell/aics-cytoparam
 Author: Matheus Viana
 Author-email: matheus.viana@alleninstitute.org
 License: Allen Institute Software License
 Description: # 3D Cell Parameterization
         
@@ -146,15 +146,14 @@
         
 Keywords: aicscytoparam
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: setup
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: all
```

### Comparing `aicscytoparam-0.1.6/README.md` & `aicscytoparam-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `aicscytoparam-0.1.6/aicscytoparam/bin/my_example.py` & `aicscytoparam-0.1.9/aicscytoparam/bin/my_example.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     level=logging.INFO, format="[%(levelname)4s:%(lineno)4s %(asctime)s] %(message)s"
 )
 
 ###############################################################################
 
 
 class Args(argparse.Namespace):
-
     DEFAULT_FIRST = 10
     DEFAULT_SECOND = 20
 
     def __init__(self):
         # Arguments that could be passed in through the command line
         self.first = self.DEFAULT_FIRST
         self.second = self.DEFAULT_SECOND
```

### Comparing `aicscytoparam-0.1.6/aicscytoparam/cytoparam.py` & `aicscytoparam-0.1.9/aicscytoparam/cytoparam.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import Optional, List, Dict, Tuple
 from vtk.util.numpy_support import vtk_to_numpy, numpy_to_vtk
 
 
 def parameterize_image_coordinates(
     seg_mem: np.array, seg_nuc: np.array, lmax: int, nisos: List
 ):
-
     """
     Runs the parameterization for a cell represented by its spherical
     harmonics coefficients calculated by using ther package aics-shparam.
 
     Parameters
     --------------------
     seg_mem: np.array
@@ -80,15 +79,14 @@
     coeffs_mem: Dict,
     centroid_mem: List,
     coeffs_nuc: Dict,
     centroid_nuc: List,
     nisos: List,
     images_to_probe: Optional[List] = None,
 ):
-
     """
     Runs the parameterization for a cell represented by its spherical
     harmonics coefficients calculated by using ther package aics-shparam.
 
     Parameters
     --------------------
     coeffs_mem: dict
@@ -138,15 +136,14 @@
 def get_interpolators(
     coeffs_mem: Dict,
     centroid_mem: Dict,
     coeffs_nuc: Dict,
     centroid_nuc: Dict,
     nisos: List,
 ):
-
     """
     Creates 1D interpolators for SHE coefficients with fixed points
     at: 1) nuclear centroid, 2) nuclear shell and 3) cell membrane.
     Also creates an interpolator for corresponding centroids.
 
     Parameters
     --------------------
@@ -220,15 +217,14 @@
 def get_mapping_coordinates(
     coeffs_mem: Dict,
     centroid_mem: List,
     coeffs_nuc: Dict,
     centroid_nuc: List,
     nisos: List,
 ):
-
     """
     Interpolate spherical harmonics coefficients representing the nuclear centroid,
     the nuclear shell and the cell membrane. As the coefficients are interpolated,
     polygonal meshes representing corresponding 3D shapes are reconstructed and
     the coordinates of their points are returned.
 
     Parameters
@@ -266,15 +262,14 @@
         coeffs_nuc=coeffs_nuc,
         centroid_nuc=centroid_nuc,
         nisos=nisos,
     )
 
     x_coords, y_coords, z_coords = [], [], []
     for i, iso_value in enumerate(np.linspace(0.0, 1.0, 1 + np.sum(nisos))):
-
         # Get coeffs at given fixed point
         coeffs = coeffs_interpolator(iso_value).reshape(2, lmax + 1, lmax + 1)
         mesh, _ = shtools.get_reconstruction_from_coeffs(coeffs, lrec=2 * lmax)
 
         # Store coordinates
         coords = vtk_to_numpy(mesh.GetPoints().GetData())
 
@@ -293,15 +288,14 @@
     coeffs_mem: Dict,
     centroid_mem: List,
     coeffs_nuc: Dict,
     centroid_nuc: List,
     nisos: List,
     images_to_probe: Optional[List] = None,
 ):
-
     """
     Interpolate spherical harmonics coefficients representing the nuclear centroid,
     the nuclear shell and the cell membrane. As the coefficients are interpolated,
     polygonal meshes representing corresponding 3D shapes are reconstructed and used
     to probe input images and create intensity representations.
 
     Parameters
@@ -345,15 +339,14 @@
         coeffs_nuc=coeffs_nuc,
         centroid_nuc=centroid_nuc,
         nisos=nisos,
     )
 
     representations = []
     for i, iso_value in enumerate(np.linspace(0.0, 1.0, 1 + np.sum(nisos))):
-
         # Get coeffs at given fixed point
         coeffs = coeffs_interpolator(iso_value).reshape(2, lmax + 1, lmax + 1)
         mesh, grid = shtools.get_reconstruction_from_coeffs(coeffs, lrec=2 * lmax)
 
         # Translate mesh to interpolated location
         centroid = centroids_interpolator(iso_value).reshape(1, 3)
         coords = vtk_to_numpy(mesh.GetPoints().GetData())
@@ -387,15 +380,14 @@
     # Convert array into TIFF
     code = AICSImage(code, channel_names=ch_names)
 
     return code
 
 
 def get_intensity_representation(polydata: vtk.vtkPolyData, images_to_probe: List):
-
     """
     This function probes the location of 3D mesh points in a list
     of 3D images.
 
     Parameters
     --------------------
     polydata: vtkPolyData
@@ -412,29 +404,28 @@
     result: list of ndarrays
         [(a,b)] where a is the probed image name and b is a 1d array with
         the corresponding probed intensities.
     """
 
     representation = {}
     coords = vtk_to_numpy(polydata.GetPoints().GetData())
-    x, y, z = [coords[:, i].astype(np.int) for i in range(3)]
+    x, y, z = [coords[:, i].astype(int) for i in range(3)]
     for name, img in images_to_probe:
         # Bound the values of x, y and z coordinates to fit inside the
         # probe image
         x_clip = np.clip(x, 0, img.shape[2] - 1)
         y_clip = np.clip(y, 0, img.shape[1] - 1)
         z_clip = np.clip(z, 0, img.shape[0] - 1)
         representation[name] = img[z_clip, y_clip, x_clip]
     return representation
 
 
 def voxelize_mesh(
     imagedata: vtk.vtkImageData, shape: Tuple, mesh: vtk.vtkPolyData, origin: List
 ):
-
     """
     Voxelize a triangle mesh into an image.
 
     Parameters
     --------------------
     imagedata: vtkImageData
         Imagedata that will be uses as support for voxelization.
@@ -469,15 +460,14 @@
     scalars = imgstenc.GetOutput().GetPointData().GetScalars()
     img = vtk_to_numpy(scalars).reshape(shape)
 
     return img
 
 
 def voxelize_meshes(meshes: List):
-
     """
     List of meshes to be voxelized into an image. Usually
     the input corresponds to the cell membrane and nuclear
     shell meshes.
 
     Parameters
     --------------------
@@ -500,16 +490,16 @@
     # the larger than the 2nd one (nucleus).
     mesh = meshes[0]
 
     # Find mesh coordinates
     coords = vtk_to_numpy(mesh.GetPoints().GetData())
 
     # Find bounds of the mesh
-    rmin = (coords.min(axis=0) - 0.5).astype(np.int)
-    rmax = (coords.max(axis=0) + 0.5).astype(np.int)
+    rmin = (coords.min(axis=0) - 0.5).astype(int)
+    rmax = (coords.max(axis=0) + 0.5).astype(int)
 
     # Width, height and depth
     w = int(2 + (rmax[0] - rmin[0]))
     h = int(2 + (rmax[1] - rmin[1]))
     d = int(2 + (rmax[2] - rmin[2]))
 
     # Create image data
@@ -538,15 +528,14 @@
 
     return img, origin
 
 
 def morph_representation_on_shape(
     img: np.array, param_img_coords: np.array, representation: np.array
 ):
-
     """
     Decodes the parameterized intensity representation
     into an image. To do so, an input image with the final
     shape is required.
 
     Parameters
     --------------------
```

### Comparing `aicscytoparam-0.1.6/aicscytoparam.egg-info/PKG-INFO` & `aicscytoparam-0.1.9/aicscytoparam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicscytoparam
-Version: 0.1.6
+Version: 0.1.9
 Summary: Cytoplasm parameterization using spherical harmonics
 Home-page: https://github.com/AllenCell/aics-cytoparam
 Author: Matheus Viana
 Author-email: matheus.viana@alleninstitute.org
 License: Allen Institute Software License
 Description: # 3D Cell Parameterization
         
@@ -146,15 +146,14 @@
         
 Keywords: aicscytoparam
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: setup
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: all
```

### Comparing `aicscytoparam-0.1.6/aicscytoparam.egg-info/SOURCES.txt` & `aicscytoparam-0.1.9/aicscytoparam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aicscytoparam-0.1.6/docs/Makefile` & `aicscytoparam-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aicscytoparam-0.1.6/docs/conf.py` & `aicscytoparam-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aicscytoparam-0.1.6/docs/im1.jpg` & `aicscytoparam-0.1.9/docs/im1.jpg`

 * *Files identical despite different names*

### Comparing `aicscytoparam-0.1.6/docs/im2.jpg` & `aicscytoparam-0.1.9/docs/im2.jpg`

 * *Files identical despite different names*

### Comparing `aicscytoparam-0.1.6/docs/im3.jpg` & `aicscytoparam-0.1.9/docs/im3.jpg`

 * *Files identical despite different names*

### Comparing `aicscytoparam-0.1.6/docs/installation.rst` & `aicscytoparam-0.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aicscytoparam-0.1.6/docs/logo.jpg` & `aicscytoparam-0.1.9/docs/logo.jpg`

 * *Files identical despite different names*

### Comparing `aicscytoparam-0.1.6/docs/make.bat` & `aicscytoparam-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aicscytoparam-0.1.6/setup.py` & `aicscytoparam-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 setup_requirements = [
     "pytest-runner>=5.2",
 ]
 
 test_requirements = [
     "black>=19.10b0",
-    "codecov>=2.1.4",
+    # "codecov>=2.1.4",
     "flake8>=3.8.3",
     "flake8-debugger>=3.2.1",
     "pytest>=5.4.3",
     "pytest-cov>=2.9.0",
     "pytest-raises>=0.11",
 ]
 
@@ -61,15 +61,14 @@
     author="Matheus Viana",
     author_email="matheus.viana@alleninstitute.org",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: Free for non-commercial use",
         "Natural Language :: English",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
     description="Cytoplasm parameterization using spherical harmonics",
     entry_points={
         "console_scripts": [
             "my_example=aicscytoparam.bin.my_example:main"
         ],
@@ -78,18 +77,18 @@
     license="Allen Institute Software License",
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="aicscytoparam",
     name="aicscytoparam",
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*"]),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     setup_requires=setup_requirements,
     test_suite="aicscytoparam/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/AllenCell/aics-cytoparam",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="0.1.6",
+    version="0.1.9",
     zip_safe=False,
 )
```

