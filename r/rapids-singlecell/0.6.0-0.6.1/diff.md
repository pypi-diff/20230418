# Comparing `tmp/rapids_singlecell-0.6.0.tar.gz` & `tmp/rapids_singlecell-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapids_singlecell-0.6.0.tar", last modified: Tue Apr 18 13:27:32 2023, max compression
+gzip compressed data, was "rapids_singlecell-0.6.1.tar", last modified: Tue Apr 18 15:37:06 2023, max compression
```

## Comparing `rapids_singlecell-0.6.0.tar` & `rapids_singlecell-0.6.1.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0     1069 2023-03-03 11:20:17.299953 rapids_singlecell-0.6.0/LICENSE
--rw-r--r--   0        0        0     5989 2023-04-18 11:17:34.044876 rapids_singlecell-0.6.0/README.md
--rw-r--r--   0        0        0      875 2023-04-18 09:58:06.059693 rapids_singlecell-0.6.0/pyproject.toml
--rwxr-xr-x   0        0        0      132 2023-03-29 22:28:18.323022 rapids_singlecell-0.6.0/rapids_singlecell/__init__.py
--rw-r--r--   0        0        0    13190 2023-03-29 22:51:45.957485 rapids_singlecell-0.6.0/rapids_singlecell/cunnData/__init__.py
--rw-r--r--   0        0        0      348 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/__init__.py
--rw-r--r--   0        0        0    33809 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_hvg.py
--rw-r--r--   0        0        0     5655 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_normalize.py
--rw-r--r--   0        0        0     4042 2023-04-18 12:39:27.596837 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_pca.py
--rw-r--r--   0        0        0     2801 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_plotting.py
--rw-r--r--   0        0        0     4761 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_regress_out.py
--rw-r--r--   0        0        0     1418 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_scale.py
--rw-r--r--   0        0        0    20228 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_simple.py
--rw-r--r--   0        0        0      574 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_utils.py
--rw-r--r--   0        0        0       29 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/dcg.py
--rw-r--r--   0        0        0       68 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/decoupler_gpu/__init__.py
--rw-r--r--   0        0        0     4570 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/decoupler_gpu/_method_mlm.py
--rw-r--r--   0        0        0     6256 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/decoupler_gpu/_method_wsum.py
--rw-r--r--   0        0        0       27 2023-03-29 22:29:08.519202 rapids_singlecell-0.6.0/rapids_singlecell/gr.py
--rw-r--r--   0        0        0       91 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/pl.py
--rw-r--r--   0        0        0       31 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/pp.py
--rw-r--r--   0        0        0      339 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/__init__.py
--rw-r--r--   0        0        0     5734 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_clustering.py
--rw-r--r--   0        0        0     3515 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_diffmap.py
--rw-r--r--   0        0        0     4075 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_draw_graph.py
--rw-r--r--   0        0        0     5143 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_embedding_density.py
--rw-r--r--   0        0        0    12184 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
--rw-r--r--   0        0        0     1743 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
--rw-r--r--   0        0        0     4177 2023-03-30 09:21:25.830448 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_pca.py
--rw-r--r--   0        0        0     2467 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_pymde.py
--rw-r--r--   0        0        0     8052 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
--rw-r--r--   0        0        0     3238 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_tsne.py
--rw-r--r--   0        0        0     5955 2023-03-29 23:19:18.101264 rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/.ipynb_checkpoints/_gearysc-checkpoint.py
--rw-r--r--   0        0        0       40 2023-03-29 22:29:32.419282 rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/__init__.py
--rw-r--r--   0        0        0     5765 2023-04-18 12:02:04.942440 rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/_autocorr.py
--rw-r--r--   0        0        0     5955 2023-03-29 23:19:18.101264 rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/_gearysc.py
--rw-r--r--   0        0        0     5774 2023-03-30 09:02:49.753339 rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/_moransi.py
--rw-r--r--   0        0        0     3319 2023-03-30 09:31:07.162869 rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/_utils.py
--rw-r--r--   0        0        0       26 2023-03-03 11:20:17.459952 rapids_singlecell-0.6.0/rapids_singlecell/tl.py
--rw-r--r--   0        0        0     6761 1970-01-01 00:00:00.000000 rapids_singlecell-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-18 15:29:50.416825 rapids_singlecell-0.6.1/LICENSE
+-rw-r--r--   0        0        0     5989 2023-04-18 15:29:50.416825 rapids_singlecell-0.6.1/README.md
+-rw-r--r--   0        0        0      903 2023-04-18 15:36:55.344433 rapids_singlecell-0.6.1/pyproject.toml
+-rwxr-xr-x   0        0        0      132 2023-04-18 15:33:39.042766 rapids_singlecell-0.6.1/rapids_singlecell/__init__.py
+-rw-r--r--   0        0        0    13190 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData/__init__.py
+-rw-r--r--   0        0        0      348 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/__init__.py
+-rw-r--r--   0        0        0    33809 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_hvg.py
+-rw-r--r--   0        0        0     5655 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_normalize.py
+-rw-r--r--   0        0        0     4042 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_pca.py
+-rw-r--r--   0        0        0     2801 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_plotting.py
+-rw-r--r--   0        0        0     4761 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_regress_out.py
+-rw-r--r--   0        0        0     1418 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_scale.py
+-rw-r--r--   0        0        0    20228 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_simple.py
+-rw-r--r--   0        0        0      574 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_utils.py
+-rw-r--r--   0        0        0       29 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/dcg.py
+-rw-r--r--   0        0        0       68 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/decoupler_gpu/__init__.py
+-rw-r--r--   0        0        0     4570 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/decoupler_gpu/_method_mlm.py
+-rw-r--r--   0        0        0     6256 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/decoupler_gpu/_method_wsum.py
+-rw-r--r--   0        0        0       27 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/gr.py
+-rw-r--r--   0        0        0       91 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/pl.py
+-rw-r--r--   0        0        0       31 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/pp.py
+-rw-r--r--   0        0        0      339 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/__init__.py
+-rw-r--r--   0        0        0     5734 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_clustering.py
+-rw-r--r--   0        0        0     3515 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_diffmap.py
+-rw-r--r--   0        0        0     4075 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_draw_graph.py
+-rw-r--r--   0        0        0     5143 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_embedding_density.py
+-rw-r--r--   0        0        0    12184 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
+-rw-r--r--   0        0        0     1743 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
+-rw-r--r--   0        0        0     4177 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_pca.py
+-rw-r--r--   0        0        0     2467 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_pymde.py
+-rw-r--r--   0        0        0     8052 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
+-rw-r--r--   0        0        0     3238 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_tsne.py
+-rw-r--r--   0        0        0       40 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/__init__.py
+-rw-r--r--   0        0        0     5785 2023-04-18 15:32:56.994409 rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/_autocorr.py
+-rw-r--r--   0        0        0     5955 2023-04-18 15:29:50.584827 rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/_gearysc.py
+-rw-r--r--   0        0        0     5774 2023-04-18 15:29:50.584827 rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/_moransi.py
+-rw-r--r--   0        0        0     3278 2023-04-18 15:29:50.584827 rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/_utils.py
+-rw-r--r--   0        0        0       26 2023-04-18 15:29:50.584827 rapids_singlecell-0.6.1/rapids_singlecell/tl.py
+-rw-r--r--   0        0        0     6796 1970-01-01 00:00:00.000000 rapids_singlecell-0.6.1/PKG-INFO
```

### Comparing `rapids_singlecell-0.6.0/LICENSE` & `rapids_singlecell-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/README.md` & `rapids_singlecell-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/pyproject.toml` & `rapids_singlecell-0.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,16 @@
     "decoupler>=1.3.2",
     "scipy>=1.4",
     "pandas>=1.0",
     "natsort",
     "scikit-misc>=0.1.3",
     "matplotlib>=3.4",
     "seaborn",
-    "tqdm"
+    "tqdm",
+    "statsmodels>=0.12.0",
 ]
 
 [project.optional-dependencies]
 rapids = ["cudf-cu11", "cuml-cu11", "cugraph-cu11"] 
 
 [project.urls]
 Documentation = "https://rapids-singlecell.readthedocs.io"
```

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/cunnData/__init__.py` & `rapids_singlecell-0.6.1/rapids_singlecell/cunnData/__init__.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_hvg.py` & `rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_hvg.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_normalize.py` & `rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_normalize.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_pca.py` & `rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_pca.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_plotting.py` & `rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_plotting.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_regress_out.py` & `rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_regress_out.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_scale.py` & `rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_scale.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_simple.py` & `rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_simple.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/cunnData_funcs/_utils.py` & `rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_utils.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/decoupler_gpu/_method_mlm.py` & `rapids_singlecell-0.6.1/rapids_singlecell/decoupler_gpu/_method_mlm.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/decoupler_gpu/_method_wsum.py` & `rapids_singlecell-0.6.1/rapids_singlecell/decoupler_gpu/_method_wsum.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_clustering.py` & `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_clustering.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_diffmap.py` & `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_diffmap.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_draw_graph.py` & `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_draw_graph.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_embedding_density.py` & `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_embedding_density.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py` & `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_harmony_integrate.py` & `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_harmony_integrate.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_pca.py` & `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_pca.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_pymde.py` & `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_pymde.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py` & `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/scanpy_gpu/_tsne.py` & `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_tsne.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/.ipynb_checkpoints/_gearysc-checkpoint.py` & `rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/_gearysc.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/_autocorr.py` & `rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/_autocorr.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 import pandas as pd
 import numpy as np
 from typing import (
     TYPE_CHECKING,
     Literal,  # < 3.8
     Sequence,
     Union,
+    Optional,
 )
 from scipy import sparse
 import cupy as cp
 from ._moransi import _morans_I_cupy
 from ._gearysc import _gearys_C_cupy
 from ._utils import _p_value_calc
 from statsmodels.stats.multitest import multipletests
 
 def spatial_autocorr(
     adata: AnnData,
     connectivity_key: str = "spatial_connectivities",
     genes: Union[str, Sequence[str],None] = None,
     mode: Literal["moran", "geary"] = "moran",
     transformation: bool = True,
-    n_perms: int | None = None,
+    n_perms: Union[int,None]= None,
     two_tailed: bool = False,
     corr_method: Union[str,None] = "fdr_bh",
     layer: Union[str,None] = None,
     use_raw: bool = False,
     use_sparse:bool = False,
     copy: bool = False,
-
-) -> pd.DataFrame | None:
+) -> Optional[pd.DataFrame]:
     """
     Calculate spatial autocorrelation for genes in an AnnData object.
 
     This function computes spatial autocorrelation scores (Moran's I or Geary's C) for each gene in an AnnData object. 
     The function also calculates p-values and corrected p-values for multiple testing.
 
     Note:
```

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/_gearysc.py` & `rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/_moransi.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,137 +1,129 @@
 import cupy as cp
 import math
 
-
-kernel_gearys_C_num_dense = '''
-extern "C" __global__ void gearys_C_num_dense(const float* data, 
-const int* adj_matrix_row_ptr, const int* adj_matrix_col_ind, const float* adj_matrix_data, 
-float* num, int n_samples, int n_features) {
+kernel_morans_I_num_dense = '''
+extern "C" __global__
+void morans_I_num_dense(const float* data_centered, const int* adj_matrix_row_ptr, const int* adj_matrix_col_ind, 
+const float* adj_matrix_data, float* num, int n_samples, int n_features) {
     int f = blockIdx.x * blockDim.x + threadIdx.x;
     int i = blockIdx.y * blockDim.y + threadIdx.y;
 
     if (i >= n_samples || f >= n_features) {
         return;
     }
 
     int k_start = adj_matrix_row_ptr[i];
     int k_end = adj_matrix_row_ptr[i + 1];
 
     for (int k = k_start; k < k_end; ++k) {
         int j = adj_matrix_col_ind[k];
-        float edge_weight = adj_matrix_data[k];
-        float diff_sq = (data[i * n_features + f] - data[j * n_features + f]) * (data[i * n_features + f] - data[j * n_features + f]);
-        atomicAdd(&num[f], edge_weight * diff_sq);
+        float edge_weight = (adj_matrix_data[k]);
+        float product = data_centered[i * n_features + f] * data_centered[j * n_features + f];
+        atomicAdd(&num[f], edge_weight * product);
     }
 }
 '''
 
-
-def _gearys_C_cupy_dense(data, adj_matrix_cupy, n_permutations=100):
+def _morans_I_cupy_dense(data, adj_matrix_cupy, n_permutations=100):
     n_samples, n_features = data.shape
-    # Calculate the numerator for Geary's C
+    data_centered_cupy = data - data.mean(axis=0)
+
+    # Calculate the numerator and denominator for Moran's I
     num = cp.zeros(n_features, dtype=cp.float32)
-    num_kernel = cp.RawKernel(kernel_gearys_C_num_dense, 'gearys_C_num_dense')
-    
     block_size = 8
     fg = int(math.ceil(n_features / block_size))
     sg = int(math.ceil(n_samples / block_size))
-    grid_size = (fg, sg,1)
+    grid_size = (fg, sg, 1)
+
+    num_kernel = cp.RawKernel(kernel_morans_I_num_dense, 'morans_I_num_dense')
     num_kernel(grid_size, 
-               (block_size, block_size,1), 
-               (data, adj_matrix_cupy.indptr, adj_matrix_cupy.indices, 
+               (block_size, block_size, 1), 
+               (data_centered_cupy, adj_matrix_cupy.indptr, adj_matrix_cupy.indices, 
                 adj_matrix_cupy.data, num, n_samples, n_features))
-    # Calculate the denominator for Geary's C
-    gene_mean = data.mean(axis=0).ravel()
-    preden = cp.sum((data - gene_mean) ** 2, axis=0)
-    den = 2 * adj_matrix_cupy.sum() * preden
-    
-    # Calculate Geary's C
-    gearys_C = (n_samples - 1) * num / den
-    
+    den = cp.sum(data_centered_cupy ** 2, axis=0)
+    morans_I = num / den
     # Calculate p-values using permutation tests
     if n_permutations:
-        gearys_C_permutations = cp.zeros((n_permutations, n_features), dtype=cp.float32)
+        morans_I_permutations = cp.zeros((n_permutations, n_features), dtype=cp.float32)
         for p in range(n_permutations):
             idx_shuffle = cp.random.permutation(adj_matrix_cupy.shape[0])
             adj_matrix_permuted = adj_matrix_cupy[idx_shuffle,:]
-            num_permuted = cp.zeros(n_features, dtype=data.dtype)
+            num_permuted = cp.zeros(n_features, dtype=cp.float32)
             num_kernel(grid_size, 
-                       (block_size, block_size,1), 
-                       (data, adj_matrix_permuted.indptr, adj_matrix_permuted.indices, 
-                        adj_matrix_permuted.data, num_permuted, n_samples, n_features))
-            #den_permuted = 2 * adj_matrix_permuted.sum() * preden
-            gearys_C_permutations[p,:] = (n_samples - 1) * num_permuted / den
+                       (block_size, block_size, 1), 
+                       (data_centered_cupy, adj_matrix_permuted.indptr, adj_matrix_permuted.indices, 
+                       adj_matrix_permuted.data, num_permuted, n_samples, n_features))
+            morans_I_permutations[p,:] = num_permuted / den
             cp.cuda.Stream.null.synchronize()
     else:
-        gearys_C_permutations = None
-    return gearys_C, gearys_C_permutations
+        morans_I_permutations=None
+    return morans_I, morans_I_permutations
 
-def _gearys_C_cupy_sparse(data, adj_matrix_cupy, n_permutations=100):
+def _morans_I_cupy_sparse(data, adj_matrix_cupy, n_permutations=100):
     n_samples, n_features = data.shape
-        
-    # Calculate the denominator for Geary's C
-    gene_mean = data.mean(axis=0).ravel()
-    preden = cp.sum((data - gene_mean) ** 2, axis=0)
-    den = 2 * adj_matrix_cupy.sum() * preden    
+    data_mean = data.mean(axis=0).ravel()
+
+    # Calculate den
+    den = cp.sum((data- data_mean) ** 2, axis=0)
     
-    # Calculate the numerator for Geary's C
+    # Calculate the numerator and denominator for Moran's I
     data = data.tocsc()
     num = cp.zeros(n_features, dtype=data.dtype)
     block_size = 8
+    
     sg = int(math.ceil(n_samples / block_size))
-    num_kernel = cp.RawKernel(kernel_gearys_C_num_dense, 'gearys_C_num_dense')
+    
+    num_kernel = cp.RawKernel(kernel_morans_I_num_dense, 'morans_I_num_dense')
     batchsize = 1000
     n_batches = math.ceil(n_features / batchsize)
     for batch in range(n_batches):
         start_idx = batch * batchsize
         stop_idx = min(batch * batchsize + batchsize, n_features)
-        data_block = data[:,start_idx:stop_idx].toarray()
-        num_block = cp.zeros(data_block.shape[1], dtype=data.dtype)
-        fg = int(math.ceil(data_block.shape[1] / block_size))
+        data_centered_cupy = data[:,start_idx:stop_idx].toarray()
+        data_centered_cupy = data_centered_cupy-data_mean[start_idx:stop_idx]
+        num_block = cp.zeros(data_centered_cupy.shape[1], dtype=data.dtype)
+        fg = int(math.ceil(data_centered_cupy.shape[1] / block_size))
         grid_size = (fg, sg, 1)
 
         num_kernel(grid_size, 
                    (block_size, block_size, 1), 
-                   (data_block, adj_matrix_cupy.indptr, adj_matrix_cupy.indices, 
-                    adj_matrix_cupy.data, num_block, n_samples, data_block.shape[1]))
+                   (data_centered_cupy, adj_matrix_cupy.indptr, adj_matrix_cupy.indices, 
+                    adj_matrix_cupy.data, num_block, n_samples, data_centered_cupy.shape[1]))
         num[start_idx:stop_idx] = num_block
         cp.cuda.Stream.null.synchronize()
-       
-    # Calculate Geary's C
-    gearys_C = (n_samples - 1) * num / den
     
+    morans_I = num / den
     # Calculate p-values using permutation tests
     if n_permutations:
-        gearys_C_permutations = cp.zeros((n_permutations, n_features), dtype=cp.float32)
+        morans_I_permutations = cp.zeros((n_permutations, n_features), dtype=cp.float32)
         for p in range(n_permutations):
             idx_shuffle = cp.random.permutation(adj_matrix_cupy.shape[0])
             adj_matrix_permuted = adj_matrix_cupy[idx_shuffle,:]
             num_permuted = cp.zeros(n_features, dtype=data.dtype)
             for batch in range(n_batches):
                 start_idx = batch * batchsize
                 stop_idx = min(batch * batchsize + batchsize, n_features)
-                data_block = data[:,start_idx:stop_idx].toarray()
-                num_block = cp.zeros(data_block.shape[1], dtype=data.dtype)
-                fg = int(math.ceil(data_block.shape[1] / block_size))
+                data_centered_cupy = data[:,start_idx:stop_idx].toarray()
+                data_centered_cupy = data_centered_cupy-data_mean[start_idx:stop_idx]
+                num_block = cp.zeros(data_centered_cupy.shape[1], dtype=data.dtype)
+                fg = int(math.ceil(data_centered_cupy.shape[1] / block_size))
                 grid_size = (fg, sg, 1)
-
                 num_kernel(grid_size, 
                            (block_size, block_size, 1), 
-                           (data_block, adj_matrix_permuted.indptr, adj_matrix_permuted.indices, 
-                            adj_matrix_permuted.data, num_block, n_samples, data_block.shape[1]))
-                num_permuted[start_idx:stop_idx] = num_block            
-
-            #den_permuted = 2 * adj_matrix_permuted.sum() * preden
-            gearys_C_permutations[p,:] = (n_samples - 1) * num_permuted / den
-            cp.cuda.Stream.null.synchronize()
+                           (data_centered_cupy, adj_matrix_permuted.indptr, adj_matrix_permuted.indices, 
+                            adj_matrix_permuted.data, num_block, n_samples, data_centered_cupy.shape[1]))
+                num_permuted[start_idx:stop_idx] = num_block
+                cp.cuda.Stream.null.synchronize()
+            morans_I_permutations[p,:] = num_permuted / den
     else:
-        gearys_C_permutations = None
-    return gearys_C, gearys_C_permutations
+        morans_I_permutations=None
+    return morans_I, morans_I_permutations
+
 
-def _gearys_C_cupy(data, adj_matrix_cupy, n_permutations=100):
+def _morans_I_cupy(data, adj_matrix_cupy, n_permutations=100):
     if cp.sparse.isspmatrix_csr(data):
-        return _gearys_C_cupy_sparse(data, adj_matrix_cupy, n_permutations)
+        return _morans_I_cupy_sparse(data, adj_matrix_cupy, n_permutations)
     elif isinstance(data, cp.ndarray):
-        return _gearys_C_cupy_dense(data, adj_matrix_cupy, n_permutations)
+        return _morans_I_cupy_dense(data, adj_matrix_cupy, n_permutations)
     else:
         raise ValueError("Datatype not supported")
```

### Comparing `rapids_singlecell-0.6.0/rapids_singlecell/squidpy_gpu/_utils.py` & `rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import numpy as np
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
+    Union,
 )
 from scipy import stats
 from scipy.sparse import spmatrix
 
 ### Taken from squidpy: https://github.com/scverse/squidpy/blob/main/squidpy/gr/_ppatterns.py
 def _p_value_calc(
     score: np.ndarray,
-    sims: np.ndarray | None,
-    weights: spmatrix | np.ndarray,
+    sims: Union[np.ndarray, None],
+    weights: Union[spmatrix, np.ndarray],
     params: Dict[str, Any],
-) -> Dict[str, Any]:
+):
     """
     Handle p-value calculation for spatial autocorrelation function.
     Parameters
     ----------
     score
         (n_features,).
     sims
@@ -60,15 +61,15 @@
     results["pval_z_sim"] = p_z_sim
     results["pval_sim"] = p_sim
     results["var_sim"] = var_sim
 
     return results
 
 
-def _analytic_pval(score: np.ndarray, g: spmatrix | np.ndarray, params: Dict[str, Any]) -> tuple[np.ndarray, float]:
+def _analytic_pval(score: np.ndarray, g: Union[spmatrix, np.ndarray], params: Dict[str, Any]):
     """
     Analytic p-value computation.
     See `Moran's I <https://pysal.org/esda/_modules/esda/moran.html#Moran>`_ and
     `Geary's C <https://pysal.org/esda/_modules/esda/geary.html#Geary>`_ implementation.
     """
     s0, s1, s2 = _g_moments(g)
     n = g.shape[0]
@@ -87,15 +88,15 @@
 
     if params["two_tailed"]:
         p_norm *= 2.0
 
     return p_norm, Vscore_norm
 
 
-def _g_moments(w: spmatrix | np.ndarray) -> tuple[float, float, float]:
+def _g_moments(w: Union[spmatrix, np.ndarray]):
     """
     Compute moments of adjacency matrix for analytic p-value calculation.
     See `pysal <https://pysal.org/libpysal/_modules/libpysal/weights/weights.html#W>`_ implementation.
     """
     # s0
     s0 = w.sum()
```

### Comparing `rapids_singlecell-0.6.0/PKG-INFO` & `rapids_singlecell-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: rapids_singlecell
-Version: 0.6.0
+Version: 0.6.1
 Summary: running single cell analysis on Nvidia GPUs
 Author: Severin Dicks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: anndata>=0.7.4
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: decoupler>=1.3.2
 Requires-Dist: scipy>=1.4
 Requires-Dist: pandas>=1.0
 Requires-Dist: natsort
 Requires-Dist: scikit-misc>=0.1.3
 Requires-Dist: matplotlib>=3.4
 Requires-Dist: seaborn
 Requires-Dist: tqdm
+Requires-Dist: statsmodels>=0.12.0
 Requires-Dist: cudf-cu11 ; extra == "rapids"
 Requires-Dist: cuml-cu11 ; extra == "rapids"
 Requires-Dist: cugraph-cu11 ; extra == "rapids"
 Project-URL: Documentation, https://rapids-singlecell.readthedocs.io
 Project-URL: Source, https://github.com/Intron7/rapids_singlecell
 Provides-Extra: rapids
```

