# Comparing `tmp/Slpapy-0.1.13.tar.gz` & `tmp/Slpapy-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.1.13.tar", last modified: Tue Apr 18 01:22:37 2023, max compression
+gzip compressed data, was "Slpapy-0.1.14.tar", last modified: Tue Apr 18 05:24:56 2023, max compression
```

## Comparing `Slpapy-0.1.13.tar` & `Slpapy-0.1.14.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 01:22:37.079470 Slpapy-0.1.13/
--rw-rw-rw-   0        0        0      160 2023-04-18 01:22:37.078470 Slpapy-0.1.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 01:22:37.067470 Slpapy-0.1.13/Slpapy/
--rw-rw-rw-   0        0        0     2042 2023-04-17 08:19:46.000000 Slpapy-0.1.13/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.1.13/Slpapy/MZ_ppm_match.py
--rw-rw-rw-   0        0        0      525 2023-04-14 06:21:10.000000 Slpapy-0.1.13/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     5133 2023-04-17 10:27:08.000000 Slpapy-0.1.13/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-04-18 01:22:37.076470 Slpapy-0.1.13/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      160 2023-04-18 01:22:36.000000 Slpapy-0.1.13/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-04-18 01:22:36.000000 Slpapy-0.1.13/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 01:22:36.000000 Slpapy-0.1.13/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-04-18 01:22:36.000000 Slpapy-0.1.13/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 01:22:36.000000 Slpapy-0.1.13/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 01:22:37.079470 Slpapy-0.1.13/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-04-18 01:21:49.000000 Slpapy-0.1.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:24:56.474187 Slpapy-0.1.14/
+-rw-rw-rw-   0        0        0      160 2023-04-18 05:24:56.473187 Slpapy-0.1.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 05:24:56.463187 Slpapy-0.1.14/Slpapy/
+-rw-rw-rw-   0        0        0     2042 2023-04-17 08:19:46.000000 Slpapy-0.1.14/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.1.14/Slpapy/MZ_ppm_match.py
+-rw-rw-rw-   0        0        0      525 2023-04-14 06:21:10.000000 Slpapy-0.1.14/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     5155 2023-04-18 05:23:52.000000 Slpapy-0.1.14/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:24:56.472203 Slpapy-0.1.14/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      160 2023-04-18 05:24:56.000000 Slpapy-0.1.14/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-04-18 05:24:56.000000 Slpapy-0.1.14/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:24:56.000000 Slpapy-0.1.14/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-04-18 05:24:56.000000 Slpapy-0.1.14/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 05:24:56.000000 Slpapy-0.1.14/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 05:24:56.474187 Slpapy-0.1.14/setup.cfg
+-rw-rw-rw-   0        0        0      487 2023-04-18 05:24:01.000000 Slpapy-0.1.14/setup.py
```

### Comparing `Slpapy-0.1.13/Slpapy/Data_reconstruction.py` & `Slpapy-0.1.14/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.13/Slpapy/MZ_ppm_match.py` & `Slpapy-0.1.14/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.13/Slpapy/__init__.py` & `Slpapy-0.1.14/Slpapy/__init__.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.1.13/Slpapy/processing_analyze.py` & `Slpapy-0.1.14/Slpapy/processing_analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,19 @@
     # 归一化，使得不同细胞样本间可比
     sc.pp.normalize_total(adata, target_sum=1e4)
     sc.pp.log1p(adata)
     # 存储数据
     adata.raw = adata
     sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
     sc.pl.highly_variable_genes(adata, save='_highly_variable_lipid.png')
+    adata.raw = adata
     adata = adata[:, adata.var.highly_variable]
     adata.obsm['X_spacial'] = np.array(adata.obs.loc[:, 'X':'Y'])
     # 回归每个细胞的总计数和表达的线粒体基因的百分比的影响。
-    #sc.pp.regress_out(adata, ['total_counts', 'pct_counts_mt'])
+    sc.pp.regress_out(adata, ['total_counts', 'pct_counts_mt'])
     #保存mz值
     mz=adata.var
     mz.to_csv('mz.csv')
     adata.write('./pp_done.h5ad')
     return adata
```

