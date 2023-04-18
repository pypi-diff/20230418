# Comparing `tmp/rapids_singlecell-0.5.1.tar.gz` & `tmp/rapids_singlecell-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapids_singlecell-0.5.1.tar", last modified: Mon Feb 27 13:30:15 2023, max compression
+gzip compressed data, was "rapids_singlecell-0.6.0.tar", last modified: Tue Apr 18 13:27:32 2023, max compression
```

## Comparing `rapids_singlecell-0.5.1.tar` & `rapids_singlecell-0.6.0.tar`

### file list

```diff
@@ -1,37 +1,40 @@
--rw-r--r--   0        0        0     1069 2023-02-10 10:06:37.176988 rapids_singlecell-0.5.1/LICENSE
--rw-r--r--   0        0        0     5453 2023-02-10 10:06:37.183679 rapids_singlecell-0.5.1/README.md
--rw-r--r--   0        0        0      816 2023-02-10 10:06:38.225961 rapids_singlecell-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4096 2023-02-24 08:53:16.198917 rapids_singlecell-0.5.1/rapids_singlecell/.___init__.py
--rwxr-xr-x   0        0        0      115 2023-02-24 08:28:13.000000 rapids_singlecell-0.5.1/rapids_singlecell/__init__.py
--rw-r--r--   0        0        0     4096 2023-02-27 13:25:21.152948 rapids_singlecell-0.5.1/rapids_singlecell/cunnData/.___init__.py
--rw-r--r--   0        0        0    13227 2023-02-24 08:57:44.000000 rapids_singlecell-0.5.1/rapids_singlecell/cunnData/__init__.py
--rw-r--r--   0        0        0     4096 2023-02-27 12:53:47.742453 rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/.___init__.py
--rw-r--r--   0        0        0     4096 2023-02-27 13:12:08.438788 rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/.__simple.py
--rw-r--r--   0        0        0      348 2023-02-24 14:19:36.000000 rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/__init__.py
--rw-r--r--   0        0        0    33809 2023-02-10 10:06:38.265587 rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_hvg.py
--rw-r--r--   0        0        0     5655 2023-02-10 10:06:38.271925 rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_normalize.py
--rw-r--r--   0        0        0     4070 2023-02-10 10:06:38.278745 rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_pca.py
--rw-r--r--   0        0        0     2801 2023-02-10 10:06:38.285247 rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_plotting.py
--rw-r--r--   0        0        0     4761 2023-02-10 10:06:38.291814 rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_regress_out.py
--rw-r--r--   0        0        0     1418 2023-02-10 10:06:38.298505 rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_scale.py
--rw-r--r--   0        0        0    20228 2023-02-27 13:01:14.000000 rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_simple.py
--rw-r--r--   0        0        0      574 2023-02-10 10:06:38.312315 rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_utils.py
--rw-r--r--   0        0        0       29 2023-02-10 10:06:38.318495 rapids_singlecell-0.5.1/rapids_singlecell/dcg.py
--rw-r--r--   0        0        0       68 2023-02-10 10:06:38.328967 rapids_singlecell-0.5.1/rapids_singlecell/decoupler_gpu/__init__.py
--rw-r--r--   0        0        0     4570 2023-02-10 10:06:38.335855 rapids_singlecell-0.5.1/rapids_singlecell/decoupler_gpu/_method_mlm.py
--rw-r--r--   0        0        0     6256 2023-02-10 10:06:38.342940 rapids_singlecell-0.5.1/rapids_singlecell/decoupler_gpu/_method_wsum.py
--rw-r--r--   0        0        0       91 2023-02-10 10:06:38.348532 rapids_singlecell-0.5.1/rapids_singlecell/pl.py
--rw-r--r--   0        0        0       31 2023-02-10 10:06:38.354975 rapids_singlecell-0.5.1/rapids_singlecell/pp.py
--rw-r--r--   0        0        0      339 2023-02-10 10:06:38.365403 rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/__init__.py
--rw-r--r--   0        0        0     5734 2023-02-10 10:06:38.372669 rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_clustering.py
--rw-r--r--   0        0        0     3515 2023-02-10 10:06:38.379028 rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_diffmap.py
--rw-r--r--   0        0        0     4075 2023-02-10 10:06:38.385681 rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_draw_graph.py
--rw-r--r--   0        0        0     5143 2023-02-10 10:06:38.392219 rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_embedding_density.py
--rw-r--r--   0        0        0    12184 2023-02-10 10:06:38.398756 rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
--rw-r--r--   0        0        0     1743 2023-02-10 10:06:38.405413 rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
--rw-r--r--   0        0        0     4177 2023-02-10 10:06:38.412013 rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_pca.py
--rw-r--r--   0        0        0     2467 2023-02-10 10:06:38.418627 rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_pymde.py
--rw-r--r--   0        0        0     8052 2023-02-10 10:06:38.424830 rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
--rw-r--r--   0        0        0     3238 2023-02-10 10:06:38.432567 rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_tsne.py
--rw-r--r--   0        0        0       26 2023-02-10 10:06:38.440359 rapids_singlecell-0.5.1/rapids_singlecell/tl.py
--rw-r--r--   0        0        0     6156 1970-01-01 00:00:00.000000 rapids_singlecell-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-03 11:20:17.299953 rapids_singlecell-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5989 2023-04-18 11:17:34.044876 rapids_singlecell-0.6.0/README.md
+-rw-r--r--   0        0        0      875 2023-04-18 09:58:06.059693 rapids_singlecell-0.6.0/pyproject.toml
+-rwxr-xr-x   0        0        0      132 2023-03-29 22:28:18.323022 rapids_singlecell-0.6.0/rapids_singlecell/__init__.py
+-rw-r--r--   0        0        0    13190 2023-03-29 22:51:45.957485 rapids_singlecell-0.6.0/rapids_singlecell/cunnData/__init__.py
+-rw-r--r--   0        0        0      348 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/__init__.py
+-rw-r--r--   0        0        0    33809 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_hvg.py
+-rw-r--r--   0        0        0     5655 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_normalize.py
+-rw-r--r--   0        0        0     4042 2023-04-18 12:39:27.596837 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_pca.py
+-rw-r--r--   0        0        0     2801 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_plotting.py
+-rw-r--r--   0        0        0     4761 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_regress_out.py
+-rw-r--r--   0        0        0     1418 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_scale.py
+-rw-r--r--   0        0        0    20228 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_simple.py
+-rw-r--r--   0        0        0      574 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_utils.py
+-rw-r--r--   0        0        0       29 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/dcg.py
+-rw-r--r--   0        0        0       68 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/decoupler_gpu/__init__.py
+-rw-r--r--   0        0        0     4570 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/decoupler_gpu/_method_mlm.py
+-rw-r--r--   0        0        0     6256 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/decoupler_gpu/_method_wsum.py
+-rw-r--r--   0        0        0       27 2023-03-29 22:29:08.519202 rapids_singlecell-0.6.0/rapids_singlecell/gr.py
+-rw-r--r--   0        0        0       91 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/pl.py
+-rw-r--r--   0        0        0       31 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/pp.py
+-rw-r--r--   0        0        0      339 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/__init__.py
+-rw-r--r--   0        0        0     5734 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_clustering.py
+-rw-r--r--   0        0        0     3515 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_diffmap.py
+-rw-r--r--   0        0        0     4075 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_draw_graph.py
+-rw-r--r--   0        0        0     5143 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_embedding_density.py
+-rw-r--r--   0        0        0    12184 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
+-rw-r--r--   0        0        0     1743 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
+-rw-r--r--   0        0        0     4177 2023-03-30 09:21:25.830448 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_pca.py
+-rw-r--r--   0        0        0     2467 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_pymde.py
+-rw-r--r--   0        0        0     8052 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
+-rw-r--r--   0        0        0     3238 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_tsne.py
+-rw-r--r--   0        0        0     5955 2023-03-29 23:19:18.101264 rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/.ipynb_checkpoints/_gearysc-checkpoint.py
+-rw-r--r--   0        0        0       40 2023-03-29 22:29:32.419282 rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/__init__.py
+-rw-r--r--   0        0        0     5765 2023-04-18 12:02:04.942440 rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/_autocorr.py
+-rw-r--r--   0        0        0     5955 2023-03-29 23:19:18.101264 rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/_gearysc.py
+-rw-r--r--   0        0        0     5774 2023-03-30 09:02:49.753339 rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/_moransi.py
+-rw-r--r--   0        0        0     3319 2023-03-30 09:31:07.162869 rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/_utils.py
+-rw-r--r--   0        0        0       26 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/tl.py
+-rw-r--r--   0        0        0     6761 1970-01-01 00:00:00.000000 rapids_singlecell-0.6.0/PKG-INFO
```

### Comparing `rapids_singlecell-0.5.1/LICENSE` & `rapids_singlecell-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/README.md` & `rapids_singlecell-0.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,36 @@
+[![Stars](https://img.shields.io/github/stars/Intron7/rapids_singlecell?logo=GitHub&color=blue)](https://github.com/Intron7/rapids_singlecell/stargazers)
+[![PyPI](https://img.shields.io/pypi/v/rapids-singlecell?logo=PyPI)](https://pypi.org/project/rapids-singlecell)
+[![PyPIDownloads](https://pepy.tech/badge/rapids-singlecell)](https://pepy.tech/project/rapids-singlecell)
+[![Documentation Status](https://readthedocs.org/projects/rapids-singlecell/badge/?version=latest)](https://rapids-singlecell.readthedocs.io/en/latest/?badge=latest)
+
 # rapids-singlecell
 
 ## Background
 This repository offers some tools to make analyses of single cell datasets faster by running them on the GPU. 
 The functions are analogous versions of functions that can be found within [scanpy](https://github.com/scverse/scanpy) from the Theis lab or functions from [rapids-single-cell-examples](https://github.com/clara-parabricks/rapids-single-cell-examples) created by the Nvidia RAPIDS team. Most functions are kept close to the original code to ensure compatibility. My aim with this repository was to use the speedup that GPU computing offers and combine it with the ease of use from scanpy.
 
 ## Installation
 ### Conda
 The easiest way to install *rapids-singlecell* is to use one of the *yaml* file provided in the [conda](https://github.com/Intron7/rapids_singlecell/tree/main/conda) folder. These *yaml* files install everything needed to run the example notbooks and get you started.
 ```
 conda env create -f conda/rsc_rapids_22.12.yml
 # or
-mamba env create -f conda/rsc_rapids_23.02a.yml
+mamba env create -f conda/rsc_rapids_23.02.yml
 ```
 ### PyPI
 As of version 0.4.0 *rapids-singlecell* is now on PyPI.
 ```
 pip install rapids-singlecell
 ```
 The default installer doesn't cover RAPIDS nor cupy. Information on how to install RAPIDS & cupy can be found [here](https://rapids.ai/start.html).
 
 If you want to use RAPIDS new PyPI packages, the whole library with all dependencies can be install with:
 ````
-pip install 'rapids-singlecell[rapids]' --extra-index-url=https://pypi.ngc.nvidia.com
+pip install 'rapids-singlecell[rapids]' --extra-index-url=https://pypi.nvidia.com
 ````
 Please note that the RAPIDS PyPI packages are still considered experimental. It is important to ensure that the CUDA environment is set up correctly so that RAPIDS and Cupy can locate the necessary libraries.
 
 To view a full guide how to set up a fully functioned single cell GPU accelerated conda environment visit [GPU_SingleCell_Setup](https://github.com/Intron7/GPU_SingleCell_Setup)
 
 ## Documentation
```

### Comparing `rapids_singlecell-0.5.1/pyproject.toml` & `rapids_singlecell-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -29,8 +29,9 @@
     "tqdm"
 ]
 
 [project.optional-dependencies]
 rapids = ["cudf-cu11", "cuml-cu11", "cugraph-cu11"] 
 
 [project.urls]
+Documentation = "https://rapids-singlecell.readthedocs.io"
 Source = "https://github.com/Intron7/rapids_singlecell"
```

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/cunnData/__init__.py` & `rapids_singlecell-0.6.0/rapids_singlecell/cunnData/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import cupyx as cpx
 from anndata import AnnData
 from anndata._core.index import _normalize_indices
 import anndata
 
 import numpy as np
 import pandas as pd
-import scipy
 from scipy import sparse
 from collections import OrderedDict
 from typing import Any, Union, Optional, Mapping, MutableMapping
 from pandas.api.types import infer_dtype
 
 from natsort import natsorted
 
@@ -89,30 +88,30 @@
         var: Optional[pd.DataFrame] = None,
         uns: Optional[Mapping[str, Any]] = None,
         layers: Optional[Mapping[str, Any]] = None,
         obsm: Optional[Mapping[str, Any]] = None,
         varm: Optional[Mapping[str, Any]] = None):
             if adata:
                 if not issparse_cpu(adata.X):
-                    inter = scipy.sparse.csr_matrix(adata.X)
+                    inter = sparse.csr_matrix(adata.X)
                     self._X = cp.sparse.csr_matrix(inter, dtype=cp.float32)
                     del inter
                 else:
                     self._X = cp.sparse.csr_matrix(adata.X, dtype=cp.float32)
                 self._obs = adata.obs.copy()
                 self._var = adata.var.copy()
                 self._uns = adata.uns.copy()
                 self._layers = Layer_Mapping(self.shape)
                 self._obsm = obsm_Mapping(self.shape[0])
                 self._varm = varm_Mapping(self.shape[1])
                 self.raw = None
                 if adata.layers:
                     for key, matrix in adata.layers.items():
                         if not issparse_cpu(matrix):
-                            inter = scipy.sparse.csr_matrix(matrix)
+                            inter = sparse.csr_matrix(matrix)
                             inter = cp.sparse.csr_matrix(inter, dtype=cp.float32)
                             
                         else:
                             inter = cp.sparse.csr_matrix(matrix, dtype=cp.float32)
                         self._layers[key] = inter.copy()
                         del inter
                 if adata.obsm:
@@ -124,15 +123,15 @@
                 
             else:
                 if issparse_gpu(X):
                     self._X = X      
                 elif isinstance(X,cp.ndarray):
                     self._X  = X            
                 elif not issparse_cpu(X):
-                    inter = scipy.sparse.csr_matrix(X)
+                    inter = sparse.csr_matrix(X)
                     self._X = cp.sparse.csr_matrix(inter, dtype=cp.float32)
                     del inter
                 else:
                     self._X = cp.sparse.csr_matrix(X, dtype=cp.float32)
 
                 self._obs = obs
                 self._var = var
@@ -148,15 +147,15 @@
                 if layers:
                     for key, matrix in layers.items():
                         if issparse_gpu(matrix):
                             inter = matrix
                         elif isinstance(matrix,cp.ndarray):
                             inter = matrix               
                         elif not issparse_cpu(X):
-                            inter = scipy.sparse.csr_matrix(matrix)
+                            inter = sparse.csr_matrix(matrix)
                             inter = cp.sparse.csr_matrix(inter, dtype=cp.float32)
                         else:
                             inter = cp.sparse.csr_matrix(matrix, dtype=cp.float32)
                         self.layers[key] = inter.copy()
                         del inter
                 if obsm:
                     for key, matrix in obsm.items():
```

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_hvg.py` & `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_hvg.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_normalize.py` & `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_normalize.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_pca.py` & `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from ..cunnData import cunnData
 
 from cuml.decomposition import PCA, TruncatedSVD
-from anndata import AnnData
 from typing import Optional
 
 from cupy.sparse import issparse
 import math
 import numpy as np
 
 def pca(cudata: cunnData,
```

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_plotting.py` & `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_plotting.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_regress_out.py` & `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_regress_out.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_scale.py` & `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_scale.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_simple.py` & `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_simple.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/cunnData_funcs/_utils.py` & `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_utils.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/decoupler_gpu/_method_mlm.py` & `rapids_singlecell-0.6.0/rapids_singlecell/decoupler_gpu/_method_mlm.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/decoupler_gpu/_method_wsum.py` & `rapids_singlecell-0.6.0/rapids_singlecell/decoupler_gpu/_method_wsum.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_clustering.py` & `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_clustering.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_diffmap.py` & `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_diffmap.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_draw_graph.py` & `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_draw_graph.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_embedding_density.py` & `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_embedding_density.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py` & `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_harmony_integrate.py` & `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_harmony_integrate.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_pca.py` & `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_pca.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_pymde.py` & `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_pymde.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py` & `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/rapids_singlecell/scanpy_gpu/_tsne.py` & `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_tsne.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.5.1/PKG-INFO` & `rapids_singlecell-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapids_singlecell
-Version: 0.5.1
+Version: 0.6.0
 Summary: running single cell analysis on Nvidia GPUs
 Author: Severin Dicks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: anndata>=0.7.4
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: decoupler>=1.3.2
@@ -14,41 +14,47 @@
 Requires-Dist: scikit-misc>=0.1.3
 Requires-Dist: matplotlib>=3.4
 Requires-Dist: seaborn
 Requires-Dist: tqdm
 Requires-Dist: cudf-cu11 ; extra == "rapids"
 Requires-Dist: cuml-cu11 ; extra == "rapids"
 Requires-Dist: cugraph-cu11 ; extra == "rapids"
+Project-URL: Documentation, https://rapids-singlecell.readthedocs.io
 Project-URL: Source, https://github.com/Intron7/rapids_singlecell
 Provides-Extra: rapids
 
+[![Stars](https://img.shields.io/github/stars/Intron7/rapids_singlecell?logo=GitHub&color=blue)](https://github.com/Intron7/rapids_singlecell/stargazers)
+[![PyPI](https://img.shields.io/pypi/v/rapids-singlecell?logo=PyPI)](https://pypi.org/project/rapids-singlecell)
+[![PyPIDownloads](https://pepy.tech/badge/rapids-singlecell)](https://pepy.tech/project/rapids-singlecell)
+[![Documentation Status](https://readthedocs.org/projects/rapids-singlecell/badge/?version=latest)](https://rapids-singlecell.readthedocs.io/en/latest/?badge=latest)
+
 # rapids-singlecell
 
 ## Background
 This repository offers some tools to make analyses of single cell datasets faster by running them on the GPU. 
 The functions are analogous versions of functions that can be found within [scanpy](https://github.com/scverse/scanpy) from the Theis lab or functions from [rapids-single-cell-examples](https://github.com/clara-parabricks/rapids-single-cell-examples) created by the Nvidia RAPIDS team. Most functions are kept close to the original code to ensure compatibility. My aim with this repository was to use the speedup that GPU computing offers and combine it with the ease of use from scanpy.
 
 ## Installation
 ### Conda
 The easiest way to install *rapids-singlecell* is to use one of the *yaml* file provided in the [conda](https://github.com/Intron7/rapids_singlecell/tree/main/conda) folder. These *yaml* files install everything needed to run the example notbooks and get you started.
 ```
 conda env create -f conda/rsc_rapids_22.12.yml
 # or
-mamba env create -f conda/rsc_rapids_23.02a.yml
+mamba env create -f conda/rsc_rapids_23.02.yml
 ```
 ### PyPI
 As of version 0.4.0 *rapids-singlecell* is now on PyPI.
 ```
 pip install rapids-singlecell
 ```
 The default installer doesn't cover RAPIDS nor cupy. Information on how to install RAPIDS & cupy can be found [here](https://rapids.ai/start.html).
 
 If you want to use RAPIDS new PyPI packages, the whole library with all dependencies can be install with:
 ````
-pip install 'rapids-singlecell[rapids]' --extra-index-url=https://pypi.ngc.nvidia.com
+pip install 'rapids-singlecell[rapids]' --extra-index-url=https://pypi.nvidia.com
 ````
 Please note that the RAPIDS PyPI packages are still considered experimental. It is important to ensure that the CUDA environment is set up correctly so that RAPIDS and Cupy can locate the necessary libraries.
 
 To view a full guide how to set up a fully functioned single cell GPU accelerated conda environment visit [GPU_SingleCell_Setup](https://github.com/Intron7/GPU_SingleCell_Setup)
 
 ## Documentation
```

