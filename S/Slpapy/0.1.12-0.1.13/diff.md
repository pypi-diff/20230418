# Comparing `tmp/Slpapy-0.1.12.tar.gz` & `tmp/Slpapy-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.1.12.tar", last modified: Sun Apr 16 10:52:03 2023, max compression
+gzip compressed data, was "Slpapy-0.1.13.tar", last modified: Tue Apr 18 01:22:37 2023, max compression
```

## Comparing `Slpapy-0.1.12.tar` & `Slpapy-0.1.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 10:52:03.903423 Slpapy-0.1.12/
--rw-rw-rw-   0        0        0      160 2023-04-16 10:52:03.902424 Slpapy-0.1.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 10:52:03.890437 Slpapy-0.1.12/Slpapy/
--rw-rw-rw-   0        0        0     1972 2023-04-14 08:19:22.000000 Slpapy-0.1.12/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.1.12/Slpapy/MZ_ppm_match.py
--rw-rw-rw-   0        0        0      525 2023-04-14 06:21:10.000000 Slpapy-0.1.12/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     5129 2023-04-16 10:50:55.000000 Slpapy-0.1.12/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-04-16 10:52:03.900424 Slpapy-0.1.12/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      160 2023-04-16 10:52:03.000000 Slpapy-0.1.12/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-04-16 10:52:03.000000 Slpapy-0.1.12/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 10:52:03.000000 Slpapy-0.1.12/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-04-16 10:52:03.000000 Slpapy-0.1.12/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-16 10:52:03.000000 Slpapy-0.1.12/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 10:52:03.903423 Slpapy-0.1.12/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-04-15 13:30:30.000000 Slpapy-0.1.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 01:22:37.079470 Slpapy-0.1.13/
+-rw-rw-rw-   0        0        0      160 2023-04-18 01:22:37.078470 Slpapy-0.1.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 01:22:37.067470 Slpapy-0.1.13/Slpapy/
+-rw-rw-rw-   0        0        0     2042 2023-04-17 08:19:46.000000 Slpapy-0.1.13/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.1.13/Slpapy/MZ_ppm_match.py
+-rw-rw-rw-   0        0        0      525 2023-04-14 06:21:10.000000 Slpapy-0.1.13/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     5133 2023-04-17 10:27:08.000000 Slpapy-0.1.13/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-04-18 01:22:37.076470 Slpapy-0.1.13/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      160 2023-04-18 01:22:36.000000 Slpapy-0.1.13/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-04-18 01:22:36.000000 Slpapy-0.1.13/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 01:22:36.000000 Slpapy-0.1.13/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-04-18 01:22:36.000000 Slpapy-0.1.13/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 01:22:36.000000 Slpapy-0.1.13/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 01:22:37.079470 Slpapy-0.1.13/setup.cfg
+-rw-rw-rw-   0        0        0      487 2023-04-18 01:21:49.000000 Slpapy-0.1.13/setup.py
```

### Comparing `Slpapy-0.1.12/Slpapy/Data_reconstruction.py` & `Slpapy-0.1.13/Slpapy/Data_reconstruction.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     os.remove(f'{XY}' + "-1.csv")
     # 建一个基本的 AnnData 对象
     counts = csr_matrix(df.T, dtype=np.float32)
     adata = ad.AnnData(counts)
     # 为x和y轴提供索引
     adata.obs_names = df.columns
     adata.var['m/z'] = df.index
+    adata.var_names = ['lips' + str(x) for x in range(adata.n_vars)]
     print(adata.obs_names[:])
     print(adata.var_names[:])
     # 标注坐标位置
     adata.obs["X"] = (df1.x.values-df1.x.values.min())//5
     adata.obs["Y"] = (df1.y.values-df1.y.values.min())//5
     adata.write(f'{XY}' + ".h5ad")
     return adata
```

### Comparing `Slpapy-0.1.12/Slpapy/MZ_ppm_match.py` & `Slpapy-0.1.13/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.12/Slpapy/__init__.py` & `Slpapy-0.1.13/Slpapy/__init__.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.12/Slpapy/processing_analyze.py` & `Slpapy-0.1.13/Slpapy/processing_analyze.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     sc.pp.normalize_total(adata, target_sum=1e4)
     sc.pp.log1p(adata)
     # 存储数据
     adata.raw = adata
     sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
     sc.pl.highly_variable_genes(adata, save='_highly_variable_lipid.png')
     adata = adata[:, adata.var.highly_variable]
+    adata.obsm['X_spacial'] = np.array(adata.obs.loc[:, 'X':'Y'])
     # 回归每个细胞的总计数和表达的线粒体基因的百分比的影响。
     #sc.pp.regress_out(adata, ['total_counts', 'pct_counts_mt'])
     #保存mz值
     mz=adata.var
     mz.to_csv('mz.csv')
     adata.write('./pp_done.h5ad')
     return adata
@@ -84,15 +85,14 @@
 def Basic_processing_flow(
         adata: ad.AnnData,
         *,
         use_spacial: bool = False,
         orgknn: bool = False,
 ) -> Optional[ad.AnnData]:
     adata = pp_analyze(adata)
-    adata.obsm['X_spacial'] = np.array(adata.obs.loc[:, 'X':'Y'])
     if use_spacial == True:
         adata = XYadata(adata)
         adata = se_analyze(adata)
         sc.pl.pca_variance_ratio(adata, log=True, save='_spacial.png')
         sc.pl.umap(adata, color=['leiden'], save='_spacial.png')
         sc.tl.rank_genes_groups(adata, 'leiden', method='wilcoxon')
         sc.pl.rank_genes_groups(adata, n_genes=25, sharey=False, save='_spacial_Wilcoxon.png')
@@ -121,7 +121,9 @@
         Spatial_map(adata, 'KNNlableXY')
     adata.write('./analyze_done.h5ad')
     return adata
 
 
 
 
+
+
```

