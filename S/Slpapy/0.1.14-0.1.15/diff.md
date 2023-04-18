# Comparing `tmp/Slpapy-0.1.14.tar.gz` & `tmp/Slpapy-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.1.14.tar", last modified: Tue Apr 18 05:24:56 2023, max compression
+gzip compressed data, was "Slpapy-0.1.15.tar", last modified: Tue Apr 18 09:58:50 2023, max compression
```

## Comparing `Slpapy-0.1.14.tar` & `Slpapy-0.1.15.tar`

### file list

```diff
@@ -1,15 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 05:24:56.474187 Slpapy-0.1.14/
--rw-rw-rw-   0        0        0      160 2023-04-18 05:24:56.473187 Slpapy-0.1.14/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 05:24:56.463187 Slpapy-0.1.14/Slpapy/
--rw-rw-rw-   0        0        0     2042 2023-04-17 08:19:46.000000 Slpapy-0.1.14/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.1.14/Slpapy/MZ_ppm_match.py
--rw-rw-rw-   0        0        0      525 2023-04-14 06:21:10.000000 Slpapy-0.1.14/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     5155 2023-04-18 05:23:52.000000 Slpapy-0.1.14/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:24:56.472203 Slpapy-0.1.14/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      160 2023-04-18 05:24:56.000000 Slpapy-0.1.14/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-04-18 05:24:56.000000 Slpapy-0.1.14/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 05:24:56.000000 Slpapy-0.1.14/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-04-18 05:24:56.000000 Slpapy-0.1.14/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 05:24:56.000000 Slpapy-0.1.14/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 05:24:56.474187 Slpapy-0.1.14/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-04-18 05:24:01.000000 Slpapy-0.1.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:50.626849 Slpapy-0.1.15/
+-rw-rw-rw-   0        0        0      160 2023-04-18 09:58:50.625848 Slpapy-0.1.15/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:50.594848 Slpapy-0.1.15/Slpapy/
+-rw-rw-rw-   0        0        0     2042 2023-04-17 08:19:46.000000 Slpapy-0.1.15/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.1.15/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:50.624848 Slpapy-0.1.15/Slpapy/Spatial_map/
+-rw-rw-rw-   0        0        0      293 2023-04-18 09:32:26.000000 Slpapy-0.1.15/Slpapy/Spatial_map/Spatial_map.py
+-rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.1.15/Slpapy/Spatial_map/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.1.15/Slpapy/Spatial_map/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.1.15/Slpapy/Spatial_map/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.1.15/Slpapy/Spatial_map/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.1.15/Slpapy/Spatial_map/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.1.15/Slpapy/Spatial_map/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.1.15/Slpapy/Spatial_map/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.1.15/Slpapy/Spatial_map/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.1.15/Slpapy/Spatial_map/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.1.15/Slpapy/Spatial_map/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.1.15/Slpapy/Spatial_map/readwrite.py
+-rw-rw-rw-   0        0        0    43073 2023-04-18 09:56:24.000000 Slpapy-0.1.15/Slpapy/Spatial_map/scatterplots.py
+-rw-rw-rw-   0        0        0      259 2023-04-18 08:16:12.000000 Slpapy-0.1.15/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     4983 2023-04-18 08:26:03.000000 Slpapy-0.1.15/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-04-18 09:58:50.602849 Slpapy-0.1.15/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      160 2023-04-18 09:58:50.000000 Slpapy-0.1.15/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2023-04-18 09:58:50.000000 Slpapy-0.1.15/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 09:58:50.000000 Slpapy-0.1.15/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-04-18 09:58:50.000000 Slpapy-0.1.15/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 09:58:50.000000 Slpapy-0.1.15/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 09:58:50.626849 Slpapy-0.1.15/setup.cfg
+-rw-rw-rw-   0        0        0      487 2023-04-18 09:58:38.000000 Slpapy-0.1.15/setup.py
```

### Comparing `Slpapy-0.1.14/Slpapy/Data_reconstruction.py` & `Slpapy-0.1.15/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.14/Slpapy/MZ_ppm_match.py` & `Slpapy-0.1.15/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.14/Slpapy/processing_analyze.py` & `Slpapy-0.1.15/Slpapy/processing_analyze.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-import csv
-import os
 import anndata as ad
-import numpy as np
-import pandas as pd
 import scanpy as sc
-from typing import Optional
 from scipy.sparse import csr_matrix
 from sklearn import preprocessing
 from sklearn.cluster import KMeans
-
+import numpy as np
+from typing import Optional
+from Spatial_map import Spatial_map
 sc.settings.verbosity = 3  # 设置日志等级: errors (0), warnings (1), info (2), hints (3)
 sc.logging.print_header()
 sc.settings.set_figure_params(dpi=720, facecolor='white')
 
 
 
 
@@ -27,15 +24,15 @@
     t = adata.obs
     adata = ad.concat([adata, XYmatrix], axis=1)
     adata.obs = t
     adata.obsm['X_spacial'] = np.array(adata.obs.loc[:, 'X':'Y'])
     return adata
 
 
-def pp_analyze(adata):
+def pp_analyze(adata,onlyhighly):
     # 显示在所有细胞中在每个单细胞中产生最高计数分数的脂质
     # sc.pl.highest_expr_genes(adata, n_top=20, save='_highest_expr_protein.png')
     # 小提琴图：表达基因的数量，每个细胞包含的表达量，线粒体基因表达量的百分比。
     adata.var['mt'] = adata.var_names.str.startswith('MT-')  # 将线粒体基因标记为 mt
     sc.pp.calculate_qc_metrics(adata, qc_vars=['mt'], percent_top=None,
                                log1p=False, inplace=True)
     sc.pl.violin(adata, 'total_counts', jitter=0.4, multi_panel=True,
@@ -44,15 +41,16 @@
     sc.pp.normalize_total(adata, target_sum=1e4)
     sc.pp.log1p(adata)
     # 存储数据
     adata.raw = adata
     sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
     sc.pl.highly_variable_genes(adata, save='_highly_variable_lipid.png')
     adata.raw = adata
-    adata = adata[:, adata.var.highly_variable]
+    if onlyhighly==True:
+        adata = adata[:, adata.var.highly_variable]
     adata.obsm['X_spacial'] = np.array(adata.obs.loc[:, 'X':'Y'])
     # 回归每个细胞的总计数和表达的线粒体基因的百分比的影响。
     sc.pp.regress_out(adata, ['total_counts', 'pct_counts_mt'])
     #保存mz值
     mz=adata.var
     mz.to_csv('mz.csv')
     adata.write('./pp_done.h5ad')
@@ -70,30 +68,25 @@
     sc.tl.umap(adata, min_dist=0.01, alpha=5, spread=2)  #
     # Leiden 图聚类
     # 计算
     sc.tl.leiden(adata, resolution=0.3)
     return adata
 
 
-def Spatial_map(adata, cls):
-    cls = str(cls)
-    sc.pl.embedding(adata, basis='X_spacial', color=f'{cls}', frameon=False, save=f'_spacial_{cls}.png')
-    """
-    如需原始比例则在embedding 458行后加上
-    axs.axis('equal')
-    """
+
 
 
 def Basic_processing_flow(
         adata: ad.AnnData,
         *,
         use_spacial: bool = False,
         orgknn: bool = False,
+        onlyhighly: bool = False,
 ) -> Optional[ad.AnnData]:
-    adata = pp_analyze(adata)
+    adata = pp_analyze(adata,onlyhighly)
     if use_spacial == True:
         adata = XYadata(adata)
         adata = se_analyze(adata)
         sc.pl.pca_variance_ratio(adata, log=True, save='_spacial.png')
         sc.pl.umap(adata, color=['leiden'], save='_spacial.png')
         sc.tl.rank_genes_groups(adata, 'leiden', method='wilcoxon')
         sc.pl.rank_genes_groups(adata, n_genes=25, sharey=False, save='_spacial_Wilcoxon.png')
```

