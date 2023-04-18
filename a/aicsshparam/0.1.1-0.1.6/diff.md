# Comparing `tmp/aicsshparam-0.1.1.tar.gz` & `tmp/aicsshparam-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicsshparam-0.1.1.tar", last modified: Fri Mar  5 05:31:07 2021, max compression
+gzip compressed data, was "aicsshparam-0.1.6.tar", last modified: Tue Apr 18 02:56:19 2023, max compression
```

## Comparing `aicsshparam-0.1.1.tar` & `aicsshparam-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 05:31:07.386568 aicsshparam-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1554 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1951 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      243 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5497 2021-03-05 05:31:07.386568 aicsshparam-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3807 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 05:31:07.386568 aicsshparam-0.1.1/aicsshparam/
--rw-r--r--   0 runner    (1001) docker     (121)      305 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/aicsshparam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 05:31:07.386568 aicsshparam-0.1.1/aicsshparam/bin/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/aicsshparam/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7221 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/aicsshparam/shparam.py
--rw-r--r--   0 runner    (1001) docker     (121)    18809 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/aicsshparam/shtools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 05:31:07.386568 aicsshparam-0.1.1/aicsshparam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5497 2021-03-05 05:31:07.000000 aicsshparam-0.1.1/aicsshparam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      530 2021-03-05 05:31:07.000000 aicsshparam-0.1.1/aicsshparam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-05 05:31:07.000000 aicsshparam-0.1.1/aicsshparam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-05 05:31:07.000000 aicsshparam-0.1.1/aicsshparam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      951 2021-03-05 05:31:07.000000 aicsshparam-0.1.1/aicsshparam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-03-05 05:31:07.000000 aicsshparam-0.1.1/aicsshparam.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-05 05:31:07.386568 aicsshparam-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      612 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     5324 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)   621959 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/docs/logo.gif
--rw-r--r--   0 runner    (1001) docker     (121)      773 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     7871 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/docs/pc12.png
--rw-r--r--   0 runner    (1001) docker     (121)    25314 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/docs/table1.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    13241 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/docs/table2.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-03-05 05:31:07.386568 aicsshparam-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2237 2021-03-05 05:31:01.000000 aicsshparam-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:56:19.413527 aicsshparam-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-04-18 02:56:19.413527 aicsshparam-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:56:19.409527 aicsshparam-0.1.6/aicsshparam/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/aicsshparam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:56:19.409527 aicsshparam-0.1.6/aicsshparam/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/aicsshparam/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/aicsshparam/shparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19075 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/aicsshparam/shtools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:56:19.409527 aicsshparam-0.1.6/aicsshparam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-04-18 02:56:19.000000 aicsshparam-0.1.6/aicsshparam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-18 02:56:19.000000 aicsshparam-0.1.6/aicsshparam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 02:56:19.000000 aicsshparam-0.1.6/aicsshparam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 02:56:19.000000 aicsshparam-0.1.6/aicsshparam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-18 02:56:19.000000 aicsshparam-0.1.6/aicsshparam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 02:56:19.000000 aicsshparam-0.1.6/aicsshparam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:56:19.413527 aicsshparam-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   621959 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/logo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/pc12.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25314 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/table1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/docs/table2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-18 02:56:19.413527 aicsshparam-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-18 02:56:14.000000 aicsshparam-0.1.6/setup.py
```

### Comparing `aicsshparam-0.1.1/CONTRIBUTING.md` & `aicsshparam-0.1.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.1/LICENSE` & `aicsshparam-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.1/PKG-INFO` & `aicsshparam-0.1.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,138 +1,116 @@
-Metadata-Version: 2.1
-Name: aicsshparam
-Version: 0.1.1
-Summary: Spherical harmonics parametrization for 3D starlike shapes
-Home-page: https://github.com/AllenCell/aics-shparam
-Author: Matheus Viana
-Author-email: matheus.viana@alleninstitute.org
-License: Allen Institute Software License
-Description: # AICS Spherical Hamonics Parametrization
-        
-        [![Build Status](https://github.com/AllenCell/aics-shparam/workflows/Build%20Main/badge.svg)](https://github.com/AllenCell/aics-shparam/actions)
-        [![Documentation](https://github.com/AllenCell/aics-shparam/workflows/Documentation/badge.svg)](https://AllenCell.github.io/aics-shparam/)
-        
-        ### Spherical harmonics parametrization for 3D starlike shapes. 
-        
-        ![Parameterization of cell and nuclear shape](docs/logo.gif)
-        
-        ## Installation:
-        
-        **Stable Release**: `pip install aicsshparam`
-        
-        **Build from source to make customization**: 
-        
-        ```console
-        git clone git@github.com:AllenCell/aics-shparam.git
-        cd aics-shparam
-        pip install -e .
-        ```
-        
-        ## How to use
-        
-        Here we outline an example of how one could use spherical harmonics coefficients as shape descriptors on a synthetic dataset composed by 3 different shapes: spheres, cubes and octahedrons.
-        
-        ```python
-        # Import required packages
-        import numpy as np
-        import pandas as pd
-        import matplotlib.pyplot as plt
-        from sklearn.decomposition import PCA
-        from aicsshparam import shtools, shparam
-        from skimage.morphology import ball, cube, octahedron
-        np.random.seed(42) # for reproducibility
-        ```
-        
-        ```python
-        # Function that returns binary images containing one of the three
-        # shapes: cubes, spheres octahedrons of random sizes. 
-        def get_random_3d_shape():
-            idx = np.random.choice([0, 1, 2], 1)[0]
-            element = [ball, cube, octahedron][idx]
-            label = ['ball', 'cube', 'octahedron'][idx]
-            img = element(10 + int(10 * np.random.rand()))
-            img = np.pad(img, ((1, 1), (1, 1), (1, 1)))
-            img = img.reshape(1, *img.shape)
-            # Rotate shapes to increase dataset variability.
-            img = shtools.rotate_image_2d(
-                image=img,
-                angle=360 * np.random.rand()
-            ).squeeze()
-            return label, img
-        
-        # Compute spherical harmonics coefficients of shape and store them
-        # in a pandas dataframe.
-        df_coeffs = pd.DataFrame([])
-        for i in range(30):
-            # Get a random shape
-            label, img = get_random_3d_shape()
-            # Parameterize with L=4, which corresponds to50 coefficients
-            # in total
-            (coeffs, _), _ = shparam.get_shcoeffs(image=img, lmax=4)
-            coeffs.update({'label': label})
-            df_coeffs = df_coeffs.append(coeffs, ignore_index=True)
-         
-        # Vizualize the resulting dataframe
-        with pd.option_context('display.max_rows', 5, 'display.max_columns', 5):
-            display(df_coeffs)
-        ```
-        
-        ![Coefficients dataframe](docs/table1.jpg)
-        
-        ```python
-        # Let's use PCA to reduce the dimensionality of the coefficients
-        # dataframe from 51 down to 2.
-        pca = PCA(n_components=2)
-        trans = pca.fit_transform(df_coeffs.drop(columns=['label']))
-        df_trans = pd.DataFrame(trans)
-        df_trans.columns = ['PC1', 'PC2']
-        df_trans['label'] = df_coeffs.label
-        
-        # Vizualize the resulting dataframe
-        with pd.option_context('display.max_rows', 5, 'display.max_columns', 5):
-            display(df_trans)
-        ```
-        
-        ![PCA dataframe](docs/table2.jpg)
-        
-        ```python
-        # Scatter plot to show how similar shapes are grouped together.
-        fig, ax = plt.subplots(1,1, figsize=(3,3))
-        for label, df_label in df_trans.groupby('label'):
-            ax.scatter(df_label.PC1, df_label.PC2, label=label, s=50)
-        plt.legend(loc='upper left', bbox_to_anchor=(1.05, 1))
-        plt.xlabel('PC1')
-        plt.ylabel('PC2')
-        plt.show()
-        ```
-        
-        ![PC1 vs. PC2](docs/pc12.png)
-        
-        
-        ## Reference
-        
-        For an example of how this package was used to analyse a dataset of over 200k single-cell images at the Allen Institute for Cell Science, please check out our paper in [bioaRxiv](https://www.biorxiv.org/content/10.1101/2020.12.08.415562v1).
-        
-        ## Development
-        See [CONTRIBUTING.md](CONTRIBUTING.md) for information related to developing the code.
-        
-        
-        ## Questions?
-        
-        If you have any questions, feel free to leave a comment in our Allen Cell forum: [https://forum.allencell.org/](https://forum.allencell.org/). 
-        
-        
-        ***Free software: Allen Institute Software License***
-Keywords: aicsshparam
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: Free for non-commercial use
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: setup
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: all
+# AICS Spherical Hamonics Parametrization
+
+[![Build Status](https://github.com/AllenCell/aics-shparam/workflows/Build%20Main/badge.svg)](https://github.com/AllenCell/aics-shparam/actions)
+[![Documentation](https://github.com/AllenCell/aics-shparam/workflows/Documentation/badge.svg)](https://AllenCell.github.io/aics-shparam/)
+
+### Spherical harmonics parametrization for 3D starlike shapes. 
+
+![Parameterization of cell and nuclear shape](docs/logo.gif)
+
+## Installation:
+
+**Stable Release**: `pip install aicsshparam`
+
+**Build from source to make customization**: 
+
+```console
+git clone git@github.com:AllenCell/aics-shparam.git
+cd aics-shparam
+pip install -e .
+```
+
+## How to use
+
+Here we outline an example of how one could use spherical harmonics coefficients as shape descriptors on a synthetic dataset composed by 3 different shapes: spheres, cubes and octahedrons.
+
+```python
+# Import required packages
+import numpy as np
+import pandas as pd
+import matplotlib.pyplot as plt
+from sklearn.decomposition import PCA
+from aicsshparam import shtools, shparam
+from skimage.morphology import ball, cube, octahedron
+np.random.seed(42) # for reproducibility
+```
+
+```python
+# Function that returns binary images containing one of the three
+# shapes: cubes, spheres octahedrons of random sizes. 
+def get_random_3d_shape():
+    idx = np.random.choice([0, 1, 2], 1)[0]
+    element = [ball, cube, octahedron][idx]
+    label = ['ball', 'cube', 'octahedron'][idx]
+    img = element(10 + int(10 * np.random.rand()))
+    img = np.pad(img, ((1, 1), (1, 1), (1, 1)))
+    img = img.reshape(1, *img.shape)
+    # Rotate shapes to increase dataset variability.
+    img = shtools.rotate_image_2d(
+        image=img,
+        angle=360 * np.random.rand()
+    ).squeeze()
+    return label, img
+
+# Compute spherical harmonics coefficients of shape and store them
+# in a pandas dataframe.
+df_coeffs = pd.DataFrame([])
+for i in range(30):
+    # Get a random shape
+    label, img = get_random_3d_shape()
+    # Parameterize with L=4, which corresponds to50 coefficients
+    # in total
+    (coeffs, _), _ = shparam.get_shcoeffs(image=img, lmax=4)
+    coeffs.update({'label': label})
+    df_coeffs = df_coeffs.append(coeffs, ignore_index=True)
+ 
+# Vizualize the resulting dataframe
+with pd.option_context('display.max_rows', 5, 'display.max_columns', 5):
+    display(df_coeffs)
+```
+
+![Coefficients dataframe](docs/table1.jpg)
+
+```python
+# Let's use PCA to reduce the dimensionality of the coefficients
+# dataframe from 51 down to 2.
+pca = PCA(n_components=2)
+trans = pca.fit_transform(df_coeffs.drop(columns=['label']))
+df_trans = pd.DataFrame(trans)
+df_trans.columns = ['PC1', 'PC2']
+df_trans['label'] = df_coeffs.label
+
+# Vizualize the resulting dataframe
+with pd.option_context('display.max_rows', 5, 'display.max_columns', 5):
+    display(df_trans)
+```
+
+![PCA dataframe](docs/table2.jpg)
+
+```python
+# Scatter plot to show how similar shapes are grouped together.
+fig, ax = plt.subplots(1,1, figsize=(3,3))
+for label, df_label in df_trans.groupby('label'):
+    ax.scatter(df_label.PC1, df_label.PC2, label=label, s=50)
+plt.legend(loc='upper left', bbox_to_anchor=(1.05, 1))
+plt.xlabel('PC1')
+plt.ylabel('PC2')
+plt.show()
+```
+
+![PC1 vs. PC2](docs/pc12.png)
+
+
+## Reference
+
+For an example of how this package was used to analyse a dataset of over 200k single-cell images at the Allen Institute for Cell Science, please check out our paper in [bioaRxiv](https://www.biorxiv.org/content/10.1101/2020.12.08.415562v1).
+
+## Development
+See [CONTRIBUTING.md](CONTRIBUTING.md) for information related to developing the code.
+
+
+## Questions?
+
+If you have any questions, feel free to leave a comment in our Allen Cell forum: [https://forum.allencell.org/](https://forum.allencell.org/). 
+
+
+***Free software: Allen Institute Software License***
```

### Comparing `aicsshparam-0.1.1/aicsshparam/shparam.py` & `aicsshparam-0.1.6/aicsshparam/shparam.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     image: np.array,
     lmax: int,
     sigma: float = 0,
     compute_lcc: bool = True,
     alignment_2d: bool = True,
     make_unique: bool = False,
 ):
-
     """Compute spherical harmonics coefficients that describe an object stored as
     an image.
 
         Calculates the spherical harmonics coefficients that parametrize the shape
         formed by the foreground set of voxels in the input image. The input image
         does not need to be binary and all foreground voxels (background=0) are used
         in the computation. Foreground voxels must form a single connected component.
@@ -138,15 +137,15 @@
 
     transform = centroid + ((angle,) if alignment_2d else ())
 
     # Translate and update mesh normals
     mesh = shtools.update_mesh_points(mesh, x, y, z)
 
     # Cartesian to spherical coordinates convertion
-    rad = np.sqrt(x ** 2 + y ** 2 + z ** 2)
+    rad = np.sqrt(x**2 + y**2 + z**2)
     lat = np.arccos(np.divide(z, rad, out=np.zeros_like(rad), where=(rad != 0)))
     lon = np.pi + np.arctan2(y, x)
 
     # Creating a meshgrid data from (lon,lat,r)
     points = np.concatenate(
         [np.array(lon).reshape(-1, 1), np.array(lat).reshape(-1, 1)], axis=1
     )
@@ -169,13 +168,13 @@
     grid_down = sktrans.resize(grid, output_shape=grid_rec.shape, preserve_range=True)
 
     # Create (l,m) keys for the coefficient dictionary
     lvalues = np.repeat(np.arange(lmax + 1).reshape(-1, 1), lmax + 1, axis=1)
 
     keys = []
     for suffix in ["C", "S"]:
-        for (l, m) in zip(lvalues.flatten(), lvalues.T.flatten()):
-            keys.append(f"shcoeffs_L{l}M{m}{suffix}")
+        for L, m in zip(lvalues.flatten(), lvalues.T.flatten()):
+            keys.append(f"shcoeffs_L{L}M{m}{suffix}")
 
     coeffs_dict = dict(zip(keys, coeffs.flatten()))
 
     return (coeffs_dict, grid_rec), (image_, mesh, grid_down, transform)
```

### Comparing `aicsshparam-0.1.1/aicsshparam/shtools.py` & `aicsshparam-0.1.6/aicsshparam/shtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 def get_mesh_from_image(
     image: np.array,
     sigma: float = 0,
     lcc: bool = True,
     translate_to_origin: bool = True,
 ):
-
     """Converts a numpy array into a vtkImageData and then into a 3d mesh
     using vtkContourFilter. The input is assumed to be binary and the
     isosurface value is set to 0.5.
 
     Optionally the input can be pre-processed by i) extracting the largest
     connected component and ii) applying a gaussian smooth to it. In case
     smooth is used, the image is binarize using thershold 1/e.
@@ -63,28 +62,26 @@
 
     img = image.copy()
 
     # VTK requires YXZ
     img = np.swapaxes(img, 0, 2)
 
     # Extracting the largest connected component
-    if lcc:
-
+    if lcc is True:
         img = skmorpho.label(img.astype(np.uint8))
 
         counts = np.bincount(img.flatten())
 
         lcc = 1 + np.argmax(counts[1:])
 
         img[img != lcc] = 0
         img[img == lcc] = 1
 
     # Smooth binarize the input image and binarize
-    if sigma:
-
+    if sigma > 0:
         img = skfilters.gaussian(img.astype(np.float32), sigma=(sigma, sigma, sigma))
 
         img[img < 1.0 / np.exp(1.0)] = 0
         img[img > 0] = 1
 
         if img.sum() == 0:
             raise ValueError(
@@ -122,23 +119,23 @@
 
     mesh = cf.GetOutput()
 
     # Calculate the mesh centroid
     coords = numpy_support.vtk_to_numpy(mesh.GetPoints().GetData())
     centroid = coords.mean(axis=0, keepdims=True)
 
-    # Translate to origin
-    coords -= centroid
-    mesh.GetPoints().SetData(numpy_support.numpy_to_vtk(coords))
+    if translate_to_origin is True:
+        # Translate to origin
+        coords -= centroid
+        mesh.GetPoints().SetData(numpy_support.numpy_to_vtk(coords))
 
     return mesh, img_output, tuple(centroid.squeeze())
 
 
 def rotate_image_2d(image: np.array, angle: float, interpolation_order: int = 0):
-
     """Rotate multichannel image in 2D by a given angle. The
     expected shape of image is (C,Z,Y,X). The rotation will
     be done clock-wise around the center of the image.
 
     Parameters
     ----------
     angle : float
@@ -180,30 +177,34 @@
 
     img_aligned = img_aligned.astype(image.dtype)
 
     return img_aligned
 
 
 def align_image_2d(
-    image: np.array, alignment_channel: int = None, make_unique: bool = False
+    image: np.array,
+    alignment_channel: int = None,
+    make_unique: bool = False,
+    compute_aligned_image: bool = True,
 ):
-
     """Align a multichannel 3D image based on the channel
     specified by alignment_channel. The expected shape of
     image is (C,Z,Y,X) or (Z,Y,X).
 
     Parameters
     ----------
     image : np.array
         Input array of shape (C,Z,Y,X) or (Z,Y,X).
     alignment_channel : int
         Number of channel to be used as reference for alignemnt. The
         alignment will be propagated to all other channels.
     make_unique : bool
         Set true to make sure the alignment rotation is unique.
+    compute_aligned_image : bool
+        Set false to only compute and return the alignment angle
     Returns
     -------
     img_aligned : np.array
         Aligned image
     angle : float
         Angle used for align the shape.
     """
@@ -229,16 +230,15 @@
 
     pca = skdecomp.PCA(n_components=2)
 
     pca = pca.fit(xy)
 
     eigenvecs = pca.components_
 
-    if make_unique:
-
+    if make_unique is True:
         # Calculate angle with arctan2
         angle = 180.0 * np.arctan2(eigenvecs[0][1], eigenvecs[0][0]) / np.pi
 
         # Rotate x coordinates
         x_rot = (x - x.mean()) * np.cos(np.pi * angle / 180) + (y - y.mean()) * np.sin(
             np.pi * angle / 180
         )
@@ -248,28 +248,29 @@
         if xsk < 0.0:
             angle += 180
 
         # Map all angles to anti-clockwise
         angle = angle % 360
 
     else:
-
         # Calculate smallest angle
         angle = 0.0
         if np.abs(eigenvecs[0][0]) > EPS:
             angle = 180.0 * np.arctan(eigenvecs[0][1] / eigenvecs[0][0]) / np.pi
 
-    # Apply skimage rotation clock-wise
-    img_aligned = rotate_image_2d(image=image, angle=angle)
+    if compute_aligned_image is True:
+        # Apply skimage rotation clock-wise
+        img_aligned = rotate_image_2d(image=image, angle=angle)
 
-    return img_aligned, angle
+        return img_aligned, angle
 
+    return angle
 
-def apply_image_alignment_2d(image: np.array, angle: float):
 
+def apply_image_alignment_2d(image: np.array, angle: float):
     """Apply an existing set of alignment parameters to a
     multichannel 3D image. The expected shape of
     image is (C,Z,Y,X) or (Z,Y,X).
 
     Parameters
     ----------
     image : np.array
@@ -292,15 +293,14 @@
 
     return img_aligned
 
 
 def update_mesh_points(
     mesh: vtk.vtkPolyData, x_new: np.array, y_new: np.array, z_new: np.array
 ):
-
     """Updates the xyz coordinates of points in the input mesh
     with new coordinates provided.
 
     Parameters
     ----------
     mesh : vtkPolyData
         Mesh in VTK format to be updated.
@@ -330,15 +330,14 @@
 
     return mesh_updated
 
 
 def get_even_reconstruction_from_grid(
     grid: np.array, npoints: int = 512, centroid: Tuple = (0, 0, 0)
 ):
-
     """Converts a parametric 2D grid of type (lon,lat,rad) into
     a 3d mesh. lon in [0,2pi], lat in [0,pi]. The method uses
     a spherical mesh with an even distribution of points. The
     even distribution is obtained via the Fibonacci grid rule.
 
     Parameters
     ----------
@@ -385,15 +384,15 @@
     # Assign to sphere
     fib_x = centroid[0] + fib_grid * np.sin(fib_theta) * np.cos(fib_phi)
     fib_y = centroid[1] + fib_grid * np.sin(fib_theta) * np.sin(fib_phi)
     fib_z = centroid[2] + fib_grid * np.cos(fib_theta)
 
     # Add points (x,y,z) to a polydata
     points = vtk.vtkPoints()
-    for (x, y, z) in zip(fib_x, fib_y, fib_z):
+    for x, y, z in zip(fib_x, fib_y, fib_z):
         points.InsertNextPoint(x, y, z)
 
     rec = vtk.vtkPolyData()
     rec.SetPoints(points)
 
     # Calculates the connections between points via Delaunay triangulation
     delaunay = vtk.vtkDelaunay3D()
@@ -424,15 +423,14 @@
 
     return mesh
 
 
 def get_even_reconstruction_from_coeffs(
     coeffs: np.array, lrec: int = 0, npoints: int = 512
 ):
-
     """Converts a set of spherical harmonic coefficients into
     a 3d mesh using the Fibonacci grid for generating a mesh
     with a more even distribution of points
 
     Parameters
     ----------
     coeffs : np.array
@@ -471,15 +469,14 @@
 
     mesh = get_even_reconstruction_from_grid(grid, npoints)
 
     return mesh, grid
 
 
 def get_reconstruction_from_grid(grid: np.array, centroid: Tuple = (0, 0, 0)):
-
     """Converts a parametric 2D grid of type (lon,lat,rad) into
     a 3d mesh. lon in [0,2pi], lat in [0,pi].
 
     Parameters
     ----------
     grid : np.array
         Input grid where the element grid[i,j] represents the
@@ -538,15 +535,14 @@
 
     mesh = normals.GetOutput()
 
     return mesh
 
 
 def get_reconstruction_from_coeffs(coeffs: np.array, lrec: int = 0):
-
     """Converts a set of spherical harmonic coefficients into
     a 3d mesh.
 
     Parameters
     ----------
     coeffs : np.array
         Input array of spherical harmonic coefficients. These
@@ -597,15 +593,14 @@
     # Get mesh
     mesh = get_reconstruction_from_grid(grid)
 
     return mesh, grid
 
 
 def get_reconstruction_error(grid_input: np.array, grid_rec: np.array):
-
     """Compute mean square error between two parametric grids. When applied
     to the input parametric grid and its corresponsing reconstructed
     version, it gives an idea of the quality of the parametrization with
     low values indicate good parametrization.
 
     Parameters
     ----------
@@ -622,15 +617,14 @@
 
     mse = np.power(grid_input - grid_rec, 2).mean()
 
     return mse
 
 
 def save_polydata(mesh: vtk.vtkPolyData, filename: str):
-
     """Saves a mesh as a vtkPolyData file.
 
     Parameters
     ----------
     mesh : vtkPolyData
         Input mesh
     filename : str
```

### Comparing `aicsshparam-0.1.1/aicsshparam.egg-info/SOURCES.txt` & `aicsshparam-0.1.6/aicsshparam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.1/aicsshparam.egg-info/requires.txt` & `aicsshparam-0.1.6/aicsshparam.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 numpy>=1.18.1
 scipy>=1.4.1
 scikit-image>=0.16.2
 scikit-learn>=0.22.1
 vtk>=9.0.1
-pyshtools>=4.5
+pyshtools==4.9.1
 
 [all]
 numpy>=1.18.1
 scipy>=1.4.1
 scikit-image>=0.16.2
 scikit-learn>=0.22.1
 vtk>=9.0.1
-pyshtools>=4.5
+pyshtools==4.9.1
 pytest-runner>=5.2
-black>=19.10b0
-codecov>=2.1.4
+black>=22.10.0
 flake8>=3.8.3
 flake8-debugger>=3.2.1
 pytest>=5.4.3
 pytest-cov>=2.9.0
 pytest-raises>=0.11
 bump2version>=1.0.1
 coverage>=5.1
@@ -29,16 +28,15 @@
 sphinx_rtd_theme>=0.5.1
 tox>=3.15.2
 twine>=3.1.1
 wheel>=0.34.2
 
 [dev]
 pytest-runner>=5.2
-black>=19.10b0
-codecov>=2.1.4
+black>=22.10.0
 flake8>=3.8.3
 flake8-debugger>=3.2.1
 pytest>=5.4.3
 pytest-cov>=2.9.0
 pytest-raises>=0.11
 bump2version>=1.0.1
 coverage>=5.1
@@ -51,14 +49,13 @@
 twine>=3.1.1
 wheel>=0.34.2
 
 [setup]
 pytest-runner>=5.2
 
 [test]
-black>=19.10b0
-codecov>=2.1.4
+black>=22.10.0
 flake8>=3.8.3
 flake8-debugger>=3.2.1
 pytest>=5.4.3
 pytest-cov>=2.9.0
 pytest-raises>=0.11
```

### Comparing `aicsshparam-0.1.1/docs/Makefile` & `aicsshparam-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.1/docs/conf.py` & `aicsshparam-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.1/docs/installation.rst` & `aicsshparam-0.1.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.1/docs/logo.gif` & `aicsshparam-0.1.6/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.1/docs/make.bat` & `aicsshparam-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.1/docs/pc12.png` & `aicsshparam-0.1.6/docs/pc12.png`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.1/docs/table1.jpg` & `aicsshparam-0.1.6/docs/table1.jpg`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.1/docs/table2.jpg` & `aicsshparam-0.1.6/docs/table2.jpg`

 * *Files identical despite different names*

### Comparing `aicsshparam-0.1.1/setup.py` & `aicsshparam-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     readme = readme_file.read()
 
 setup_requirements = [
     "pytest-runner>=5.2",
 ]
 
 test_requirements = [
-    "black>=19.10b0",
-    "codecov>=2.1.4",
+    "black>=22.10.0",
+#    "codecov>=2.1.4",
     "flake8>=3.8.3",
     "flake8-debugger>=3.2.1",
     "pytest>=5.4.3",
     "pytest-cov>=2.9.0",
     "pytest-raises>=0.11",
 ]
 
@@ -39,15 +39,15 @@
 
 requirements = [
     'numpy>=1.18.1',
     'scipy>=1.4.1',
     'scikit-image>=0.16.2',
     'scikit-learn>=0.22.1',
     'vtk>=9.0.1',
-    'pyshtools>=4.5'
+    'pyshtools==4.9.1'
 ]
 
 extra_requirements = {
     "setup": setup_requirements,
     "test": test_requirements,
     "dev": dev_requirements,
     "all": [
@@ -80,10 +80,10 @@
     setup_requires=setup_requirements,
     test_suite="aicsshparam/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/AllenCell/aics-shparam",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="0.1.1",
+    version="0.1.6",
     zip_safe=False,
 )
```

