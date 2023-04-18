# Comparing `tmp/fastHDMI-1.2.9.tar.gz` & `tmp/fastHDMI-1.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastHDMI-1.2.9.tar", last modified: Wed Jan 11 04:28:24 2023, max compression
+gzip compressed data, was "fastHDMI-1.23.1.tar", last modified: Tue Apr 18 05:52:31 2023, max compression
```

## Comparing `fastHDMI-1.2.9.tar` & `fastHDMI-1.23.1.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-01-11 04:28:24.179685 fastHDMI-1.2.9/
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    34523 2022-11-10 23:21:11.000000 fastHDMI-1.2.9/LICENSE
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    45396 2023-01-11 04:28:24.179685 fastHDMI-1.2.9/PKG-INFO
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     4825 2023-01-05 11:57:51.000000 fastHDMI-1.2.9/README.md
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      996 2023-01-11 04:25:53.000000 fastHDMI-1.2.9/pyproject.toml
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)       38 2023-01-11 04:28:24.179685 fastHDMI-1.2.9/setup.cfg
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-01-11 04:28:24.179685 fastHDMI-1.2.9/src/
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-01-11 04:28:24.179685 fastHDMI-1.2.9/src/fastHDMI/
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)   171269 2023-01-11 04:27:25.000000 fastHDMI-1.2.9/src/fastHDMI/__init__.py
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-01-11 04:28:24.179685 fastHDMI-1.2.9/src/fastHDMI.egg-info/
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    45396 2023-01-11 04:28:24.000000 fastHDMI-1.2.9/src/fastHDMI.egg-info/PKG-INFO
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      201 2023-01-11 04:28:24.000000 fastHDMI-1.2.9/src/fastHDMI.egg-info/SOURCES.txt
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        1 2023-01-11 04:28:24.000000 fastHDMI-1.2.9/src/fastHDMI.egg-info/dependency_links.txt
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        9 2023-01-11 04:28:24.000000 fastHDMI-1.2.9/src/fastHDMI.egg-info/top_level.txt
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-18 05:52:31.393534 fastHDMI-1.23.1/
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    34523 2022-11-10 23:21:11.000000 fastHDMI-1.23.1/LICENSE
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      103 2023-04-17 22:35:24.000000 fastHDMI-1.23.1/MANIFEST.in
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    46504 2023-04-18 05:52:31.393534 fastHDMI-1.23.1/PKG-INFO
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     5931 2023-02-19 04:38:00.000000 fastHDMI-1.23.1/README.md
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     1170 2023-04-18 05:39:49.000000 fastHDMI-1.23.1/pyproject.toml
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)       38 2023-04-18 05:52:31.393534 fastHDMI-1.23.1/setup.cfg
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      298 2023-04-16 23:35:56.000000 fastHDMI-1.23.1/setup.py
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-18 05:52:31.389534 fastHDMI-1.23.1/src/
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-18 05:52:31.389534 fastHDMI-1.23.1/src/fastHDMI/
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)   227176 2023-04-18 05:45:38.000000 fastHDMI-1.23.1/src/fastHDMI/__init__.py
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)   900663 2023-04-18 05:52:31.000000 fastHDMI-1.23.1/src/fastHDMI/cython_fun.c
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     1956 2023-04-17 23:03:00.000000 fastHDMI-1.23.1/src/fastHDMI/cython_fun.pyx
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-18 05:52:31.393534 fastHDMI-1.23.1/src/fastHDMI.egg-info/
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    46504 2023-04-18 05:52:31.000000 fastHDMI-1.23.1/src/fastHDMI.egg-info/PKG-INFO
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      325 2023-04-18 05:52:31.000000 fastHDMI-1.23.1/src/fastHDMI.egg-info/SOURCES.txt
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        1 2023-04-18 05:52:31.000000 fastHDMI-1.23.1/src/fastHDMI.egg-info/dependency_links.txt
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      147 2023-04-18 05:52:31.000000 fastHDMI-1.23.1/src/fastHDMI.egg-info/requires.txt
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        9 2023-04-18 05:52:31.000000 fastHDMI-1.23.1/src/fastHDMI.egg-info/top_level.txt
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-18 05:52:31.393534 fastHDMI-1.23.1/tests/
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     4258 2023-04-17 23:06:01.000000 fastHDMI-1.23.1/tests/test.py
```

### Comparing `fastHDMI-1.2.9/LICENSE` & `fastHDMI-1.23.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastHDMI-1.2.9/PKG-INFO` & `fastHDMI-1.23.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fastHDMI
-Version: 1.2.9
-Summary: Use fast FFT-based mutual information and accelerated gradient method to filter out and optimize nonconvex sparse learning problems on large CSV files or large genetic bed/bim/fam files. Multiprocessing is now available.
+Version: 1.23.1
+Summary: Use FFT-based mutual information and accelerated gradient method to screen variables and optimize nonconvex sparse learning problems on large CSV files or large genetic bed/bim/fam files. Multiprocessing is now available.
 Author-email: Kai Yang <kai.yang2@mail.mcgill.ca>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -670,34 +670,42 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# fastHDMI -- fast High-Dimensional Mutual Information
+# fastHDMI -- fast High-Dimensional Mutual Information estimation
+## Kai Yang
+## <kai.yang2@mail.mcgill.ca>
 
-This packages uses mutual information and accelerated gradient method to screen for important variables from (potentially very) high-dimensional large datasets. As a feature, it can be applied on large `.csv` data in parallel in a memory-efficient manner and use FFT for KDE to estimate the mutual information extremely fast. It also features screening for SNPs and optimize the nonconvex sparse learning problem on large genetic data using plink files (`*.bed/*.bim/*.fam`). The corresponding paper by Yang et al. is coming soon...
+To be rewritten...
+
+This packages uses FFT-based mutual information screening and accelerated gradient method for important variables from (potentially very) high-dimensional large datasets. A `share_memory` option is added for multiprocess computing. As a feature, it can be applied on large `.csv` data in parallel in a memory-efficient manner and use FFT for KDE to estimate the mutual information extremely fast. A tqdm progress bar is now added to be more useful on cloud computing platforms. `verbose` option can take values of `0,1,2`, with `2` being most verbal; `1` being only show progress bar, and `0` being not verbal at all. The corresponding paper by Yang et al. is coming soon...
 
 The available functions are:
-- `continuous_filter_plink` caculates the mutual information between a continuous outcome and a bialletic SNP using FFT. Missing data is acceptable and will be removed. The arguments are:
+- `continuous_screening_plink` caculates the mutual information between a continuous outcome and a bialletic SNP using FFT. Missing data in the input variables is acceptable and will be removed per bivariate calculation. The arguments are:
   * `bed_file`, `bim_file`, `fam_file` are the location of the plink1 files;
   * `outcome`, `outcome_iid` are the outcome values and the iids for the outcome. For genetic data, it is usual that the order of SNP iid and the outcome iid don't match. While SNP iid can be obtained from the plink1 files, outcome iid here is to be declared separately. `outcome_iid` should be a list of strings or a one-dimensional numpy string array.
-  * `a_min`, `a_max` are the minimum and maximum of the continous outcome used to evaluate the support; `N=500` is the default values for grid size for FFT.
+  * `N=500` is the default values for grid size for FFT.
 
-- `binary_filter_plink` works similarly, execpt that `a_min, a_max, N` are not available obviously.
+- `binary_screening_plink` works similarly. 
 
-- `continuous_filter_plink_parallel` and `binary_filter_plink_parallel` are the multiprocessing version of the above two functions, with `core_num` can be used to declare the number of cores to be used for multiprocessing.
+- `continuous_screening_plink_parallel` and `binary_screening_plink_parallel` are the multiprocessing version of the above two functions, with `core_num` can be used to declare the number of cores to be used for multiprocessing.
 
-- `MI_bivariate_continuous` and `MI_binary_continuous` are to calculate mutual information between two continuous variables and binary and continuous variables, respectively.
+- `MI_continuous_continuous` and `MI_binary_continuous` are to calculate mutual information between two continuous variables and binary and continuous variables, respectively. `MI_binary_012` and `MI_012_012` are `jit` complied functions -- the later can be used for clumping for very large genetic datasets.
 
-- `binary_filter_csv`, `continuous_filter_csv`, `binary_filter_csv_parallel`, and `continuous_filter_csv_parallel` are to work on large CSV files directly in a memory efficient manner. **Note that it is assumed the left first column should be the outcome;** if not, use `_usecols` to set the first element to be the outcome column label.
+- `binary_screening_csv`, `continuous_screening_csv`, `binary_screening_csv_parallel`, and `continuous_screening_csv_parallel` are to work on large CSV files directly in a memory efficient manner. **Note that it is assumed the left first column should be the outcome;** if not, use `_usecols` to set the first element to be the outcome column label.
   * `_usecols` is a list of column labels to be used, **the first element should be the outcome. Returned mutual information calculation results match `_usecols`.**
-  * `Pearson_filter_csv_parallel` calculate Pearson's correlation between only the outcome and the covariates in similiar manner -- since `pandas.DataFrame.corr` calculate pairwise Pearson's correlation for the dataframe.
+  * `Pearson_screening_csv_parallel` calculate Pearson's correlation between only the outcome and the covariates in similiar manner -- since `pandas.DataFrame.corr` calculate pairwise Pearson's correlation for the entire dataframe.
+  * `csv_engine` can use `dask` for low memory situations, or `pandas`'s `read_csv` `engine`s, or `fastparquet` engine for a created `parquet` file for faster speed. If `fastparquet` is chosen, declare `parquet_file` as the filepath to the parquet file; if `dask` is chosen to read very large CSV, it might need to specify a larger [`sample`](https://docs.dask.org/en/stable/generated/dask.dataframe.read_csv.html).
+
+- `continuous_skMIscreening_csv_parallel` uses the MI calculation from [`sklearn.feature_selection.mutual_info_regression`](https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.mutual_info_regression.html) to carry out the screening process instead.
 
+- `clump_plink_parallel` and `clump_continuous_csv_parallel` carry out mutual information based clumping in parallel at a very fast speed.
 
 - `UAG_LM_SCAD_MCP`, `UAG_logistic_SCAD_MCP`: these functions find a local minizer for the SCAD/MCP penalized linear models/logistic models. The arguments are:
   * `design_matrix`: the design matrix input, should be a two-dimensional numpy array;
   * `outcome`: the outcome, should be one dimensional numpy array, continuous for linear model, binary for logistic model;
   * `beta_0`: starting value; optional, if not declared, it will be calculated based on the Gauss-Markov theory estimators of $\beta$;
   * `tol`: tolerance parameter; the tolerance parameter is set to be the uniform norm of two iterations;
   * `maxit`: maximum number of iteratios allowed;
@@ -705,10 +713,10 @@
   * `penalty`: could be `"SCAD"` or `"MCP"`;
   * `a=3.7`, `gamma=2`: `a` for SCAD and `gamma` for MCP; it is recommended for `a` to be set as $3.7$;
   * `L_convex`: the L-smoothness constant for the convex component, if not declared, it will be calculated by itself
   * `add_intercept_column`: boolean, should the fucntion add an intercept column?
 
 - `solution_path_LM`, `solution_path_logistic`: calculate the solution path for linear/logistic models; the only difference from above is that `lambda_` is now a one-dimensional numpy array for the values of $\lambda$ to be used.
 
-- `UAG_LM_SCAD_MCP_strongrule`, `UAG_logistic_SCAD_MCP_strongrule` work just like `UAG_LM_SCAD_MCP`, `UAG_logistic_SCAD_MCP` -- except they use strong rule to filter out many covariates before carrying out the optimization step. Same for `solution_path_LM_strongrule` and `solution_path_logistic_strongrule`. Strong rule increases the computational speed dramatically.
+- `UAG_LM_SCAD_MCP_strongrule`, `UAG_logistic_SCAD_MCP_strongrule` work just like `UAG_LM_SCAD_MCP`, `UAG_logistic_SCAD_MCP` -- except they use strong rule to screening out many covariates before carrying out the optimization step. Same for `solution_path_LM_strongrule` and `solution_path_logistic_strongrule`. Strong rule increases the computational speed dramatically.
 
 - `SNP_UAG_LM_SCAD_MCP` and `SNP_UAG_logistic_SCAD_MCP` work similar to `UAG_LM_SCAD_MCP` and `UAG_logistic_SCAD_MCP`; and `SNP_solution_path_LM` and `SNP_solution_path_logistic` work similar to `solution_path_LM`, `solution_path_logistic` -- except that it takes plink1 files so it will be more memory-efficient. Since PCA adjustment is usually used to adjust for population structure, PCA can be given for `pca` as a 2-d array -- each column should be one principal component. The pca version is `SNP_UAG_LM_SCAD_MCP_PCA` and `SNP_UAG_logistic_SCAD_MCP_PCA`.
```

### Comparing `fastHDMI-1.2.9/README.md` & `fastHDMI-1.23.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-# fastHDMI -- fast High-Dimensional Mutual Information
+# fastHDMI -- fast High-Dimensional Mutual Information estimation
+## Kai Yang
+## <kai.yang2@mail.mcgill.ca>
 
-This packages uses mutual information and accelerated gradient method to screen for important variables from (potentially very) high-dimensional large datasets. As a feature, it can be applied on large `.csv` data in parallel in a memory-efficient manner and use FFT for KDE to estimate the mutual information extremely fast. It also features screening for SNPs and optimize the nonconvex sparse learning problem on large genetic data using plink files (`*.bed/*.bim/*.fam`). The corresponding paper by Yang et al. is coming soon...
+To be rewritten...
+
+This packages uses FFT-based mutual information screening and accelerated gradient method for important variables from (potentially very) high-dimensional large datasets. A `share_memory` option is added for multiprocess computing. As a feature, it can be applied on large `.csv` data in parallel in a memory-efficient manner and use FFT for KDE to estimate the mutual information extremely fast. A tqdm progress bar is now added to be more useful on cloud computing platforms. `verbose` option can take values of `0,1,2`, with `2` being most verbal; `1` being only show progress bar, and `0` being not verbal at all. The corresponding paper by Yang et al. is coming soon...
 
 The available functions are:
-- `continuous_filter_plink` caculates the mutual information between a continuous outcome and a bialletic SNP using FFT. Missing data is acceptable and will be removed. The arguments are:
+- `continuous_screening_plink` caculates the mutual information between a continuous outcome and a bialletic SNP using FFT. Missing data in the input variables is acceptable and will be removed per bivariate calculation. The arguments are:
   * `bed_file`, `bim_file`, `fam_file` are the location of the plink1 files;
   * `outcome`, `outcome_iid` are the outcome values and the iids for the outcome. For genetic data, it is usual that the order of SNP iid and the outcome iid don't match. While SNP iid can be obtained from the plink1 files, outcome iid here is to be declared separately. `outcome_iid` should be a list of strings or a one-dimensional numpy string array.
-  * `a_min`, `a_max` are the minimum and maximum of the continous outcome used to evaluate the support; `N=500` is the default values for grid size for FFT.
+  * `N=500` is the default values for grid size for FFT.
 
-- `binary_filter_plink` works similarly, execpt that `a_min, a_max, N` are not available obviously.
+- `binary_screening_plink` works similarly. 
 
-- `continuous_filter_plink_parallel` and `binary_filter_plink_parallel` are the multiprocessing version of the above two functions, with `core_num` can be used to declare the number of cores to be used for multiprocessing.
+- `continuous_screening_plink_parallel` and `binary_screening_plink_parallel` are the multiprocessing version of the above two functions, with `core_num` can be used to declare the number of cores to be used for multiprocessing.
 
-- `MI_bivariate_continuous` and `MI_binary_continuous` are to calculate mutual information between two continuous variables and binary and continuous variables, respectively.
+- `MI_continuous_continuous` and `MI_binary_continuous` are to calculate mutual information between two continuous variables and binary and continuous variables, respectively. `MI_binary_012` and `MI_012_012` are `jit` complied functions -- the later can be used for clumping for very large genetic datasets.
 
-- `binary_filter_csv`, `continuous_filter_csv`, `binary_filter_csv_parallel`, and `continuous_filter_csv_parallel` are to work on large CSV files directly in a memory efficient manner. **Note that it is assumed the left first column should be the outcome;** if not, use `_usecols` to set the first element to be the outcome column label.
+- `binary_screening_csv`, `continuous_screening_csv`, `binary_screening_csv_parallel`, and `continuous_screening_csv_parallel` are to work on large CSV files directly in a memory efficient manner. **Note that it is assumed the left first column should be the outcome;** if not, use `_usecols` to set the first element to be the outcome column label.
   * `_usecols` is a list of column labels to be used, **the first element should be the outcome. Returned mutual information calculation results match `_usecols`.**
-  * `Pearson_filter_csv_parallel` calculate Pearson's correlation between only the outcome and the covariates in similiar manner -- since `pandas.DataFrame.corr` calculate pairwise Pearson's correlation for the dataframe.
+  * `Pearson_screening_csv_parallel` calculate Pearson's correlation between only the outcome and the covariates in similiar manner -- since `pandas.DataFrame.corr` calculate pairwise Pearson's correlation for the entire dataframe.
+  * `csv_engine` can use `dask` for low memory situations, or `pandas`'s `read_csv` `engine`s, or `fastparquet` engine for a created `parquet` file for faster speed. If `fastparquet` is chosen, declare `parquet_file` as the filepath to the parquet file; if `dask` is chosen to read very large CSV, it might need to specify a larger [`sample`](https://docs.dask.org/en/stable/generated/dask.dataframe.read_csv.html).
+
+- `continuous_skMIscreening_csv_parallel` uses the MI calculation from [`sklearn.feature_selection.mutual_info_regression`](https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.mutual_info_regression.html) to carry out the screening process instead.
 
+- `clump_plink_parallel` and `clump_continuous_csv_parallel` carry out mutual information based clumping in parallel at a very fast speed.
 
 - `UAG_LM_SCAD_MCP`, `UAG_logistic_SCAD_MCP`: these functions find a local minizer for the SCAD/MCP penalized linear models/logistic models. The arguments are:
   * `design_matrix`: the design matrix input, should be a two-dimensional numpy array;
   * `outcome`: the outcome, should be one dimensional numpy array, continuous for linear model, binary for logistic model;
   * `beta_0`: starting value; optional, if not declared, it will be calculated based on the Gauss-Markov theory estimators of $\beta$;
   * `tol`: tolerance parameter; the tolerance parameter is set to be the uniform norm of two iterations;
   * `maxit`: maximum number of iteratios allowed;
@@ -29,10 +37,10 @@
   * `penalty`: could be `"SCAD"` or `"MCP"`;
   * `a=3.7`, `gamma=2`: `a` for SCAD and `gamma` for MCP; it is recommended for `a` to be set as $3.7$;
   * `L_convex`: the L-smoothness constant for the convex component, if not declared, it will be calculated by itself
   * `add_intercept_column`: boolean, should the fucntion add an intercept column?
 
 - `solution_path_LM`, `solution_path_logistic`: calculate the solution path for linear/logistic models; the only difference from above is that `lambda_` is now a one-dimensional numpy array for the values of $\lambda$ to be used.
 
-- `UAG_LM_SCAD_MCP_strongrule`, `UAG_logistic_SCAD_MCP_strongrule` work just like `UAG_LM_SCAD_MCP`, `UAG_logistic_SCAD_MCP` -- except they use strong rule to filter out many covariates before carrying out the optimization step. Same for `solution_path_LM_strongrule` and `solution_path_logistic_strongrule`. Strong rule increases the computational speed dramatically.
+- `UAG_LM_SCAD_MCP_strongrule`, `UAG_logistic_SCAD_MCP_strongrule` work just like `UAG_LM_SCAD_MCP`, `UAG_logistic_SCAD_MCP` -- except they use strong rule to screening out many covariates before carrying out the optimization step. Same for `solution_path_LM_strongrule` and `solution_path_logistic_strongrule`. Strong rule increases the computational speed dramatically.
 
 - `SNP_UAG_LM_SCAD_MCP` and `SNP_UAG_logistic_SCAD_MCP` work similar to `UAG_LM_SCAD_MCP` and `UAG_logistic_SCAD_MCP`; and `SNP_solution_path_LM` and `SNP_solution_path_logistic` work similar to `solution_path_LM`, `solution_path_logistic` -- except that it takes plink1 files so it will be more memory-efficient. Since PCA adjustment is usually used to adjust for population structure, PCA can be given for `pca` as a 2-d array -- each column should be one principal component. The pca version is `SNP_UAG_LM_SCAD_MCP_PCA` and `SNP_UAG_logistic_SCAD_MCP_PCA`.
```

### Comparing `fastHDMI-1.2.9/src/fastHDMI/__init__.py` & `fastHDMI-1.23.1/src/fastHDMI/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,205 +1,217 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-import numpy as _np
+import multiprocess as _mp
+import ctypes as _ctypes
+from sklearn.preprocessing import RobustScaler as _scaler
+from sklearn.feature_selection import mutual_info_regression as _mutual_info_regression
+from sklearn.feature_selection import mutual_info_classif as _mutual_info_classif
+from dask import dataframe as _dd
 import pandas as _pd
-from bed_reader import open_bed as _open_bed
 from KDEpy import FFTKDE as _FFTKDE
-import multiprocess as _mp
-from numba import jit as _jit
+# from bed_reader import open_bed as _open_bed
 from numba import njit as _njit
-from sklearn.preprocessing import RobustScaler as _scaler
+from numba import jit as _jit
+import numpy as _np
+from tqdm import tqdm as _tqdm
+import warnings as _warnings
+from fastHDMI.cython_fun import joint_to_mi_cython
+
+_warnings.filterwarnings('ignore')
 
 
 #############################################################################
-################# filtering using mutual information ########################
+############# clumping and screening using mutual information ###############
 #############################################################################
-@_jit(nogil=True, cache=True, parallel=True)
-def MI_continuous_SNP(a,
-                      b,
-                      N=500,
-                      kernel="epa",
-                      bw="silverman",
-                      machine_err=1e-16):
+def _open_bed():
+    print(
+        "bed_reader might have some bugs for this version, causing it not running"
+    )
+    pass
+
+
+# @_njit(cache=True)
+def _nan_inf_to_0(x):
+    """
+    To convert NaN to 0 in nopython mode.
+    """
+    return _np.where(_np.isfinite(x), x, 0.)
+
+
+# @_njit(cache=True)
+def _joint_to_mi(joint, forward_euler_a=1., forward_euler_b=1.):
+    # assume that joint likelihood is of shape (len(a), len(b))
+    # forward_euler step being 1. means discrete r.v.
+    # to scale the cdf to 1.
+    joint /= _np.sum(joint) * forward_euler_a * forward_euler_b
+    log_a_marginal = _np.log(_np.sum(joint, 1)) + _np.log(forward_euler_b)
+    log_a_marginal = _nan_inf_to_0(log_a_marginal)
+    log_b_marginal = _np.log(_np.sum(joint, 0)) + _np.log(forward_euler_a)
+    log_b_marginal = _nan_inf_to_0(log_b_marginal)
+    log_joint = _np.log(joint)
+    log_joint = _nan_inf_to_0(log_joint)
+    mi_temp = _np.sum(
+        joint *
+        (log_joint - log_a_marginal.reshape(-1, 1) -
+         log_b_marginal.reshape(1, -1))) * forward_euler_a * forward_euler_b
+
+    # this is to ensure that estimated MI is positive, to solve an numerical issue
+    mi_temp = _np.max(_np.array([mi_temp, 0.]))
+
+    return mi_temp
+
+
+def MI_continuous_012(a, b, N=500, kernel="epa", bw="silverman", **kwarg):
     """
     calculate mutual information between continuous outcome and an SNP variable of 0,1,2
     assume no missing data
     """
     # first estimate the pmf
-    p0 = _np.sum(b == 0) / len(b)
-    p1 = _np.sum(b == 1) / len(b)
+    p0 = _np.count_nonzero(b == 0) / len(b)
+    p1 = _np.count_nonzero(b == 1) / len(b)
     p2 = 1. - p0 - p1
     _a = _scaler().fit_transform(a.reshape(-1, 1)).flatten()
     # this step is just to get the boundary width for the joint density grid
     # the three conditional density estimates need to be evaluated on the joint density grid
-    a_temp, _ = _FFTKDE(kernel=kernel, bw=bw).fit(data=_a).evaluate(N)
+    a_temp, _ = _FFTKDE(kernel=kernel, bw=bw, **kwarg).fit(data=_a).evaluate(N)
     # estimate cond density
     _b0 = (b == 0)
-    if _np.sum(_b0) > 2:
+    if _np.count_nonzero(_b0) > 2:
         # here proceed to kde only if there are more than 5 data points
-        y_cond_p0 = _FFTKDE(kernel=kernel, bw=bw).fit(data=_a[_b0])
-#         y_cond_p0 = gaussian_kde(_a[_b0])
+        y_cond_p0 = _FFTKDE(kernel=kernel, bw=bw, **kwarg).fit(data=_a[_b0])
     else:
         y_cond_p0 = _np.zeros_like
     _b1 = (b == 1)
-    if _np.sum(_b1) > 2:
-        y_cond_p1 = _FFTKDE(kernel=kernel, bw=bw).fit(data=_a[_b1])
-#         y_cond_p1 = gaussian_kde(_a[_b1]) # this thing uses Scott's rule instead of Silverman defaulted by FFTKDE and R density
+    if _np.count_nonzero(_b1) > 2:
+        y_cond_p1 = _FFTKDE(kernel=kernel, bw=bw, **kwarg).fit(data=_a[_b1])
     else:
         y_cond_p1 = _np.zeros_like
     _b2 = (b == 2)
-    if _np.sum(_b2) > 2:
-        y_cond_p2 = _FFTKDE(kernel=kernel, bw=bw).fit(data=_a[_b2])
-
-
-#         y_cond_p2 = gaussian_kde(_a[_b2])
+    if _np.count_nonzero(_b2) > 2:
+        y_cond_p2 = _FFTKDE(kernel=kernel, bw=bw, **kwarg).fit(data=_a[_b2])
     else:
         y_cond_p2 = _np.zeros_like
-    joint = _np.empty((N, 3))
+    joint = _np.zeros((N, 3))
     joint[:, 0] = y_cond_p0(a_temp) * p0
     joint[:, 1] = y_cond_p1(a_temp) * p1
     joint[:, 2] = y_cond_p2(a_temp) * p2
-    mask = joint < machine_err
     forward_euler_step = a_temp[1] - a_temp[0]
+    mask = joint < 0.
     joint[mask] = 0.
-    # to scale the cdf to 1.
-    joint /= _np.sum(joint) * forward_euler_step
-    #     print("total measure:",  _np.sum(joint)*forward_euler_step)
-    temp_log = _np.log(joint)
-    temp_log = _np.nan_to_num(temp_log, nan=0)
-    temp1 = _np.log(_np.sum(joint, 1))
-    temp1 = _np.nan_to_num(temp1, nan=0)
-    temp_log = temp_log - temp1.reshape(-1, 1)
-    temp2 = _np.log(_np.sum(joint, 0)) + _np.log(forward_euler_step)
-    temp2 = _np.nan_to_num(temp2, nan=0)
-    temp_log = temp_log - temp2.reshape(1, -1)
-    # print(fhat_mat * temp_log)
-    temp_mat = joint * temp_log
-    #     temp_mat =  _np.nan_to_num(temp_mat, nan=0.) # numerical fix
-    mi_temp = _np.sum(temp_mat) * forward_euler_step
 
-    # this is to ensure that estimated MI is positive, to solve an numerical issue
-    if mi_temp < machine_err:
-        mi_temp = machine_err
+    joint = _np.ascontiguousarray(joint)
+
+    mi_temp = joint_to_mi_cython(joint=joint,
+                                 forward_euler_a=forward_euler_step)
 
     return mi_temp
 
 
-@_jit(nogil=True, cache=True, parallel=True)
-def MI_binary_SNP(a, b, machine_err=1e-16):
+# @_njit(cache=True)
+def MI_binary_012(a, b):
     """
     calculate mutual information between binary outcome and an SNP variable of 0,1,2
     assume no missing data
     """
-    # first estimate the pmf of SNP
-    p0 = _np.sum(b == 0) / len(b)
-    p1 = _np.sum(b == 1) / len(b)
-    p2 = 1. - p0 - p1
-    b_marginal = _np.array([p0, p1, p2])
-    # estimate pmf of the binary outcome
-    a_p0 = _np.sum(a == 0) / len(a)
-    a_p1 = _np.sum(a == 1) / len(a)
-    a_marginal = _np.array([a_p0, a_p1]).reshape(-1, 1)
-    # estimate the cond density
-    joint = _np.zeros((2, 3))
+    return MI_012_012(a, b)
+
+
+# @_njit(cache=True)
+def MI_012_012(a, b):
+    """
+    calculate mutual information between two SNPs
+    assume no missing data
+    could be very useful for a MI-based clumping
+    """
+    # estimate the cond pmf
+    joint = _np.zeros((3, 3))
     _b0 = (b == 0)
-    joint[0, 0] = _np.sum(a[_b0] == 0) / len(a)
-    joint[1, 0] = _np.sum(a[_b0] == 1) / len(a)
+    joint[0, 0] = _np.count_nonzero(_np.logical_and(a == 0, _b0)) / len(a)
+    joint[1, 0] = _np.count_nonzero(_np.logical_and(a == 1, _b0)) / len(a)
+    joint[2, 0] = _np.count_nonzero(_np.logical_and(a == 2, _b0)) / len(a)
     _b1 = (b == 1)
-    joint[0, 1] = _np.sum(a[_b1] == 0) / len(a)
-    joint[1, 1] = _np.sum(a[_b1] == 1) / len(a)
+    joint[0, 1] = _np.count_nonzero(_np.logical_and(a == 0, _b1)) / len(a)
+    joint[1, 1] = _np.count_nonzero(_np.logical_and(a == 1, _b1)) / len(a)
+    joint[2, 1] = _np.count_nonzero(_np.logical_and(a == 2, _b1)) / len(a)
     _b2 = (b == 2)
-    joint[0, 2] = _np.sum(a[_b2] == 0) / len(a)
-    joint[1, 2] = _np.sum(a[_b2] == 1) / len(a)
+    joint[0, 2] = _np.count_nonzero(_np.logical_and(a == 0, _b2)) / len(a)
+    joint[1, 2] = _np.count_nonzero(_np.logical_and(a == 1, _b2)) / len(a)
+    joint[2, 2] = _np.count_nonzero(_np.logical_and(a == 2, _b2)) / len(a)
 
-    _ = a_marginal * b_marginal
-    _ = joint / _
-    __ = joint * _np.log(_)
-    __ = _np.nan_to_num(__, nan=0.0)  # for possible nuemrical issues
+    joint = _np.ascontiguousarray(joint)
 
-    mi_temp = _np.sum(__)
-
-    # this is to ensure that estimated MI is positive, to solve an numerical issue
-    if mi_temp < machine_err:
-        mi_temp = machine_err
+    mi_temp = joint_to_mi_cython(joint=joint)
 
     return mi_temp
 
 
-# make this function available
-@_jit(nogil=True, cache=True, parallel=True)
-def MI_bivariate_continuous(a,
-                            b,
-                            a_N=300,
-                            b_N=300,
-                            kernel="epa",
-                            bw="silverman",
-                            norm=2,
-                            machine_err=1e-16):
+def MI_continuous_continuous(a,
+                             b,
+                             a_N=300,
+                             b_N=300,
+                             kernel="epa",
+                             bw="silverman",
+                             norm=2,
+                             **kwarg):
     """
     (Single Core version) calculate mutual information on bivariate continuous r.v..
     """
-    _ = _np.argsort(a)
-    data = _np.hstack((a[_].reshape(-1, 1), b[_].reshape(-1, 1)))
+    _temp = _np.argsort(a)
+    data = _np.hstack((a[_temp].reshape(-1, 1), b[_temp].reshape(-1, 1)))
     _data = _scaler().fit_transform(data)
-    grid, joint = _FFTKDE(kernel=kernel, norm=norm).fit(_data).evaluate(
-        (a_N, b_N))
+    grid, joint = _FFTKDE(kernel=kernel, norm=norm,
+                          **kwarg).fit(_data).evaluate((a_N, b_N))
     joint = joint.reshape(b_N, -1).T
     # this gives joint as a (a_N, b_N) array, following example: https://kdepy.readthedocs.io/en/latest/examples.html#the-effect-of-norms-in-2d
     a_forward_euler_step = grid[b_N, 0] - grid[0, 0]
     b_forward_euler_step = grid[1, 1] - grid[0, 1]
-    mask = joint < machine_err
+    mask = joint < 0.
     joint[mask] = 0.
-    # to scale the cdf to 1.
-    joint /= _np.sum(joint) * a_forward_euler_step * b_forward_euler_step
-    log_a_marginal = _np.log(_np.sum(joint, 1)) + _np.log(b_forward_euler_step)
-    log_a_marginal = _np.nan_to_num(log_a_marginal, nan=0)
-    log_b_marginal = _np.log(_np.sum(joint, 0)) + _np.log(a_forward_euler_step)
-    log_b_marginal = _np.nan_to_num(log_b_marginal, nan=0)
-    log_joint = _np.log(joint)
-    log_joint = _np.nan_to_num(log_joint, nan=0)
-    mi_temp = _np.sum(
-        joint *
-        (log_joint - log_a_marginal.reshape(-1, 1) - log_b_marginal.reshape(
-            1, -1))) * a_forward_euler_step * b_forward_euler_step
 
-    # this is to ensure that estimated MI is positive, to solve an numerical issue
-    if mi_temp < machine_err:
-        mi_temp = machine_err
+    joint = _np.ascontiguousarray(joint)
+
+    mi_temp = joint_to_mi_cython(joint=joint,
+                                 forward_euler_a=a_forward_euler_step,
+                                 forward_euler_b=b_forward_euler_step)
 
     return mi_temp
 
 
-# make this function available
-@_jit(nogil=True, cache=True, parallel=True)
-def MI_binary_continuous(a,
-                         b,
-                         N=500,
-                         kernel="epa",
-                         bw="silverman",
-                         machine_err=1e-16):
-    return MI_continuous_SNP(a=b,
-                             b=a,
-                             N=N,
-                             kernel=kernel,
-                             bw=bw,
-                             machine_err=machine_err)
+def MI_binary_continuous(a, b, N=500, kernel="epa", bw="silverman", **kwarg):
+    return MI_continuous_012(a=b, b=a, N=N, kernel=kernel, bw=bw, **kwarg)
+
+
+@_njit(cache=True)
+def Pearson_to_MI_Gaussian(corr):
+    """
+    Assuming the input variables are bivariate Gaussian, convert their Pearson correlatin to mutual information.
+    """
+    return -.5 * (_np.log(1 + corr) + _np.log(1 - corr))
+
+
+@_njit(cache=True)
+def MI_to_Linfoot(mi):
+    """
+    Convert calcualted mutual information estimator to Linfoot's measure of association.
+    """
+    return (1. - _np.exp(-2. * mi))**.5
 
 
 # outcome_iid should be a  list of strings for identifiers
-def continuous_filter_plink(bed_file,
-                            bim_file,
-                            fam_file,
-                            outcome,
-                            outcome_iid,
-                            N=500,
-                            kernel="epa",
-                            bw="silverman",
-                            machine_err=1e-16):
+def continuous_screening_plink(bed_file,
+                               bim_file,
+                               fam_file,
+                               outcome,
+                               outcome_iid,
+                               N=500,
+                               kernel="epa",
+                               bw="silverman",
+                               verbose=1,
+                               **kwarg):
     """
     (Single Core version) take plink files to calculate the mutual information between the continuous outcome and many SNP variables.
     """
     bed1 = _open_bed(filepath=bed_file,
                      fam_filepath=fam_file,
                      bim_filepath=bim_file)
     gene_iid = _np.array(list(bed1.iid))
@@ -210,35 +222,41 @@
                                       return_indices=True)[1]]
 
     # get genetic indices
     gene_ind = _np.intersect1d(gene_iid,
                                outcome_iid,
                                assume_unique=True,
                                return_indices=True)[1]
-    MI_UKBB = _np.zeros(len(bed1_sid))
-    for j in range(len(MI_UKBB)):
+
+    def _map_foo(j):
         _SNP = bed1.read(_np.s_[:, j], dtype=_np.int8).flatten()
         _SNP = _SNP[gene_ind]  # get gene iid also in outcome iid
         _outcome = outcome[_SNP != -127]  # remove missing SNP in outcome
         _SNP = _SNP[_SNP != -127]  # remove missing SNP
-        MI_UKBB[j] = MI_continuous_SNP(a=_outcome,
-                                       b=_SNP,
-                                       N=N,
-                                       kernel=kernel,
-                                       bw=bw,
-                                       machine_err=machine_err)
+        return MI_continuous_012(a=_outcome,
+                                 b=_SNP,
+                                 N=N,
+                                 kernel=kernel,
+                                 bw=bw,
+                                 **kwarg)
+
+    _iter = range(len(bed1_sid))
+    if verbose > 1:
+        _iter = _tqdm(iter)
+    MI_UKBB = _np.array(list(map(_map_foo, _iter)))
     return MI_UKBB
 
 
-def binary_filter_plink(bed_file,
-                        bim_file,
-                        fam_file,
-                        outcome,
-                        outcome_iid,
-                        machine_err=1e-16):
+def binary_screening_plink(bed_file,
+                           bim_file,
+                           fam_file,
+                           outcome,
+                           outcome_iid,
+                           verbose=1,
+                           **kwarg):
     """
     (Single Core version) take plink files to calculate the mutual information between the binary outcome and many SNP variables.
     """
     bed1 = _open_bed(filepath=bed_file,
                      fam_filepath=fam_file,
                      bim_filepath=bim_file)
     gene_iid = _np.array(list(bed1.iid))
@@ -248,45 +266,53 @@
                                       assume_unique=True,
                                       return_indices=True)[1]]
     # get genetic indices
     gene_ind = _np.intersect1d(gene_iid,
                                outcome_iid,
                                assume_unique=True,
                                return_indices=True)[1]
-    MI_UKBB = _np.zeros(len(bed1_sid))
-    for j in range(len(MI_UKBB)):
+
+    def _map_foo(j):
         _SNP = bed1.read(_np.s_[:, j], dtype=_np.int8).flatten()
         _SNP = _SNP[gene_ind]  # get gene iid also in outcome iid
         _outcome = outcome[_SNP != -127]  # remove missing SNP in outcome
         _SNP = _SNP[_SNP != -127]  # remove missing SNP
-        MI_UKBB[j] = MI_binary_SNP(a=_outcome, b=_SNP, machine_err=machine_err)
+        return MI_binary_012(a=_outcome, b=_SNP, **kwarg)
+
+    _iter = range(len(bed1_sid))
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    MI_UKBB = _np.array(list(map(_map_foo, _iter)))
     return MI_UKBB
 
 
-def continuous_filter_plink_parallel(bed_file,
-                                     bim_file,
-                                     fam_file,
-                                     outcome,
-                                     outcome_iid,
-                                     N=500,
-                                     kernel="epa",
-                                     bw="silverman",
-                                     machine_err=1e-16,
-                                     core_num="NOT DECLARED",
-                                     multp=1):
+def continuous_screening_plink_parallel(bed_file,
+                                        bim_file,
+                                        fam_file,
+                                        outcome,
+                                        outcome_iid,
+                                        N=500,
+                                        kernel="epa",
+                                        bw="silverman",
+                                        core_num="NOT DECLARED",
+                                        multp=10,
+                                        verbose=1,
+                                        **kwarg):
     """
     (Multiprocessing version) take plink files to calculate the mutual information between the continuous outcome and many SNP variables.
     """
+    # check some basic things
     if core_num == "NOT DECLARED":
         core_num = _mp.cpu_count()
     else:
         assert core_num <= _mp.cpu_count(
         ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
     assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
 
+    # read some metadata
     bed1 = _open_bed(filepath=bed_file,
                      fam_filepath=fam_file,
                      bim_filepath=bim_file)
     gene_iid = _np.array(list(bed1.iid))
     bed1_sid = _np.array(list(bed1.sid))
     outcome = outcome[_np.intersect1d(outcome_iid,
                                       gene_iid,
@@ -294,58 +320,62 @@
                                       return_indices=True)[1]]
     # get genetic indices
     gene_ind = _np.intersect1d(gene_iid,
                                outcome_iid,
                                assume_unique=True,
                                return_indices=True)[1]
 
-    def _continuous_filter_plink_slice(_slice):
-        _MI_slice = _np.zeros(len(_slice))
-        k = 0
-        for j in _slice:
+    def _continuous_screening_plink_slice(_slice):
+        def _map_foo(j):
             _SNP = bed1.read(_np.s_[:, j], dtype=_np.int8).flatten()
             _SNP = _SNP[gene_ind]  # get gene iid also in outcome iid
             _outcome = outcome[_SNP != -127]  # remove missing SNP in outcome
             _SNP = _SNP[_SNP != -127]  # remove missing SNP
-            _MI_slice[k] = MI_continuous_SNP(a=_outcome,
-                                             b=_SNP,
-                                             N=N,
-                                             kernel=kernel,
-                                             bw=bw,
-                                             machine_err=machine_err)
-            k += 1
+            return MI_continuous_012(a=_outcome,
+                                     b=_SNP,
+                                     N=N,
+                                     kernel=kernel,
+                                     bw=bw,
+                                     **kwarg)
+
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
         return _MI_slice
 
     # multiprocessing starts here
     ind = _np.arange(len(bed1_sid))
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
     with _mp.Pool(core_num) as pl:
-        MI_UKBB = pl.map(_continuous_filter_plink_slice,
-                         _np.array_split(ind, core_num * multp))
+        MI_UKBB = pl.map(_continuous_screening_plink_slice, _iter)
     MI_UKBB = _np.hstack(MI_UKBB)
     return MI_UKBB
 
 
-def binary_filter_plink_parallel(bed_file,
-                                 bim_file,
-                                 fam_file,
-                                 outcome,
-                                 outcome_iid,
-                                 core_num="NOT DECLARED",
-                                 multp=1,
-                                 machine_err=1e-16):
+def binary_screening_plink_parallel(bed_file,
+                                    bim_file,
+                                    fam_file,
+                                    outcome,
+                                    outcome_iid,
+                                    core_num="NOT DECLARED",
+                                    multp=10,
+                                    verbose=1,
+                                    **kwarg):
     """
     (Multiprocessing version) take plink files to calculate the mutual information between the binary outcome and many SNP variables.
     """
+    # check basic things
     if core_num == "NOT DECLARED":
         core_num = _mp.cpu_count()
     else:
         assert core_num <= _mp.cpu_count(
         ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
     assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
 
+    # read some metadata
     bed1 = _open_bed(filepath=bed_file,
                      fam_filepath=fam_file,
                      bim_filepath=bim_file)
     gene_iid = _np.array(list(bed1.iid))
     bed1_sid = _np.array(list(bed1.sid))
     outcome = outcome[_np.intersect1d(outcome_iid,
                                       gene_iid,
@@ -353,324 +383,1609 @@
                                       return_indices=True)[1]]
     # get genetic indices
     gene_ind = _np.intersect1d(gene_iid,
                                outcome_iid,
                                assume_unique=True,
                                return_indices=True)[1]
 
-    def _binary_filter_plink_slice(_slice):
-        _MI_slice = _np.zeros(len(_slice))
-        k = 0
-        for j in _slice:
+    def _binary_screening_plink_slice(_slice):
+        def _map_foo(j):
             _SNP = bed1.read(_np.s_[:, j], dtype=_np.int8).flatten()
             _SNP = _SNP[gene_ind]  # get gene iid also in outcome iid
             _outcome = outcome[_SNP != -127]  # remove missing SNP in outcome
             _SNP = _SNP[_SNP != -127]  # remove missing SNP
-            _MI_slice[k] = MI_binary_SNP(a=_outcome,
-                                         b=_SNP,
-                                         machine_err=machine_err)
-            k += 1
+            return MI_binary_012(a=_outcome, b=_SNP, **kwarg)
+
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
         return _MI_slice
 
     # multiprocessing starts here
     ind = _np.arange(len(bed1_sid))
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose > 1:
+        _iter = _tqdm(_iter)
     with _mp.Pool(core_num) as pl:
-        MI_UKBB = pl.map(_binary_filter_plink_slice,
-                         _np.array_split(ind, core_num * multp))
+        MI_UKBB = pl.map(_binary_screening_plink_slice, _iter)
     MI_UKBB = _np.hstack(MI_UKBB)
     return MI_UKBB
 
 
-def binary_filter_csv(csv_file,
-                      _usecols=[],
-                      N=500,
-                      kernel="epa",
-                      bw="silverman",
-                      machine_err=1e-16):
+def clump_plink_parallel(bed_file,
+                         bim_file,
+                         fam_file,
+                         clumping_threshold=Pearson_to_MI_Gaussian(.6),
+                         num_SNPS_exam=_np.infty,
+                         core_num="NOT DECLARED",
+                         multp=10,
+                         verbose=1):
+    """
+    (Multiprocessing version) take plink files to calculate the mutual information between the binary outcome and many SNP variables.
+    """
+    # check basic things
+    if core_num == "NOT DECLARED":
+        core_num = _mp.cpu_count()
+    else:
+        assert core_num <= _mp.cpu_count(
+        ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
+    assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
+
+    # read some metadata
+    bed1 = _open_bed(filepath=bed_file,
+                     fam_filepath=fam_file,
+                     bim_filepath=bim_file)
+    bed1_sid = _np.array(list(bed1.sid))
+    if num_SNPS_exam == _np.infty:
+        num_SNPS_exam = len(bed1_sid) - 1
+    keep_cols = _np.arange(
+        len(bed1_sid))  # pruning by keeping all SNPS at the beginning
+    _iter = _np.arange(num_SNPS_exam)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    for current_var_ind in _iter:  # note that here _iter and keep_cols don't need to agree, by the break command comes later
+        if current_var_ind + 1 <= len(keep_cols):
+            outcome = bed1.read(_np.s_[:, current_var_ind],
+                                dtype=_np.int8).flatten()
+            gene_ind = _np.where(outcome != -127)
+            outcome = outcome[gene_ind]
+
+            def _012_012_plink_slice(_slice):
+                def _map_foo(j):
+                    _SNP = bed1.read(_np.s_[:, j], dtype=_np.int8).flatten()
+                    _SNP = _SNP[gene_ind]  # get gene iid also in outcome iid
+                    _outcome = outcome[_SNP !=
+                                       -127]  # remove missing SNP in outcome
+                    _SNP = _SNP[_SNP != -127]  # remove missing SNP
+                    return MI_012_012(a=_outcome, b=_SNP)
+
+                _MI_slice = _np.array(list(map(_map_foo, _slice)))
+                return _MI_slice
+
+            # multiprocessing starts here
+            ind = keep_cols[current_var_ind + 1:]
+            __iter = _np.array_split(ind, core_num * multp)
+            with _mp.Pool(core_num) as pl:
+                MI_UKBB = pl.map(_012_012_plink_slice, __iter)
+            MI_UKBB = _np.hstack(MI_UKBB)
+            keep_cols = _np.hstack(
+                (keep_cols[:current_var_ind + 1],
+                 keep_cols[current_var_ind +
+                           1:][MI_UKBB <= clumping_threshold]))
+        else:
+            break
+    return current_var_ind, bed1_sid[keep_cols]
+
+
+def _read_csv(csv_file, _usecols, csv_engine, parquet_file, sample, verbose=1):
+    """
+    Read a csv file using differnet engines. Use dask to read csv if low in memory.
+    """
+    assert csv_engine in [
+        "dask", "pyarrow", "fastparquet", "c", "python"
+    ], "Only dask and pandas csv engines or fastparquet are supported to read csv files."
+    if _np.array(_usecols).size == 0:
+        if verbose > 1:
+            print(
+                "Variable names not provided -- start reading variable names from csv file now, might take some time, depending on the csv file size."
+            )
+        if csv_engine == "dask":
+            _df = _dd.read_csv(csv_file, sample=sample)
+            _usecols = _np.array(list(_df.columns)[1:])
+        elif csv_engine in ["pyarrow", "c",
+                            "python"]:  # these are pandas CSV engines
+            _df = _pd.read_csv(csv_file,
+                               encoding='unicode_escape',
+                               engine=csv_engine)
+            _usecols = _np.array(_df.columns.to_list()[1:])
+        elif csv_engine == "fastparquet":
+            _df = _pd.read_parquet(parquet_file, engine="fastparquet")
+            _usecols = _np.array(_df.columns.to_list()[1:])
+        if verbose > 1:
+            print("Reading variable names from csv file finished.")
+    else:
+        _usecols = _np.array(_usecols)
+        if csv_engine == "dask":
+            _df = _dd.read_csv(csv_file, names=_usecols, sample=sample)
+        elif csv_engine in ["pyarrow", "c", "python"]:
+            _df = _pd.read_csv(csv_file,
+                               encoding='unicode_escape',
+                               usecols=_usecols,
+                               engine=csv_engine)
+        elif csv_engine == "fastparquet":
+            _df = _pd.read_parquet(parquet_file,
+                                   engine="fastparquet")[_usecols]
+    return _df, _usecols
+
+
+def _read_two_columns(_df, __, csv_engine):
+    """
+    Read two columns from a dataframe object, remove NaN. Use dask to read csv if low in memory.
+    """
+    if csv_engine == "dask":
+        _ = _np.asarray(_df[__].dropna().compute())
+    elif csv_engine in ["pyarrow", "c", "python",
+                        "fastparquet"]:  # these are engines using pandas
+        _ = _df[__].dropna().to_numpy()
+
+    _a = _[:, 0]
+    _b = _[:, 1]
+    return _a, _b
+
+
+def binary_screening_csv(csv_file="_",
+                         _usecols=[],
+                         N=500,
+                         kernel="epa",
+                         bw="silverman",
+                         csv_engine="c",
+                         parquet_file="_",
+                         sample=256000,
+                         verbose=1,
+                         **kwarg):
     """
     Take a (potentionally large) csv file to calculate the mutual information between outcome and covariates.
     The outcome should be binary and the covariates be continuous. 
     If _usecols is given, the returned mutual information will match _usecols. 
     By default, the left first covariate should be the outcome -- use _usecols to adjust if not the case.
     """
+    assert csv_file != "_" or parquet_file != "_", "CSV or parquet filepath should be declared"
     # outcome is the first variable by default; if other specifications are needed, put it the first item in _usecols
+    # read csv
+    _df, _usecols = _read_csv(csv_file=csv_file,
+                              _usecols=_usecols,
+                              csv_engine=csv_engine,
+                              parquet_file=parquet_file,
+                              sample=sample,
+                              verbose=verbose)
+
+    def _map_foo(j):
+        __ = [
+            _usecols[0], _usecols[j + 1]
+        ]  # here using _usecol[j + 1] because the left first column is the outcome
+        _a, _b = _read_two_columns(_df=_df, __=__, csv_engine=csv_engine)
+        return MI_binary_continuous(a=_a,
+                                    b=_b,
+                                    N=N,
+                                    kernel=kernel,
+                                    bw=bw,
+                                    **kwarg)
+
+    _iter = _np.arange(len(_usecols) - 1)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    MI_df = _np.array(list(map(_map_foo, _iter)))
+
+    del _df
+
+    return MI_df
+
+
+def continuous_screening_csv(csv_file="_",
+                             _usecols=[],
+                             a_N=300,
+                             b_N=300,
+                             kernel="epa",
+                             bw="silverman",
+                             norm=2,
+                             csv_engine="c",
+                             parquet_file="_",
+                             sample=256000,
+                             verbose=1,
+                             **kwarg):
+    """
+    Take a (potentionally large) csv file to calculate the mutual information between outcome and covariates.
+    Both the outcome and the covariates should be continuous. 
+    If _usecols is given, the returned mutual information will match _usecols. 
+    By default, the left first covariate should be the outcome -- use _usecols to adjust if not the case.
+    """
+    assert csv_file != "_" or parquet_file != "_", "CSV or parquet filepath should be declared"
+    # read csv
+    _df, _usecols = _read_csv(csv_file=csv_file,
+                              _usecols=_usecols,
+                              csv_engine=csv_engine,
+                              parquet_file=parquet_file,
+                              sample=sample,
+                              verbose=verbose)
+
+    def _map_foo(j):
+        __ = [
+            _usecols[0], _usecols[j + 1]
+        ]  # here using _usecol[j + 1] because the left first column is the outcome
+        _a, _b = _read_two_columns(_df=_df, __=__, csv_engine=csv_engine)
+        return MI_continuous_continuous(a=_a,
+                                        b=_b,
+                                        a_N=a_N,
+                                        b_N=b_N,
+                                        kernel=kernel,
+                                        bw=bw,
+                                        norm=norm,
+                                        **kwarg)
+
+    _iter = _np.arange(len(_usecols) - 1)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    MI_df = _np.array(list(map(_map_foo, _iter)))
+
+    del _df
+
+    return MI_df
+
+
+def binary_screening_csv_parallel(csv_file="_",
+                                  _usecols=[],
+                                  N=500,
+                                  kernel="epa",
+                                  bw="silverman",
+                                  core_num="NOT DECLARED",
+                                  multp=10,
+                                  csv_engine="c",
+                                  parquet_file="_",
+                                  sample=256000,
+                                  verbose=1,
+                                  share_memory=True,
+                                  **kwarg):
+    """
+    (Multiprocessing version) Take a (potentionally large) csv file to calculate the mutual information between outcome and covariates.
+    The outcome should be binary and the covariates be continuous. 
+    If _usecols is given, the returned mutual information will match _usecols. 
+    By default, the left first covariate should be the outcome -- use _usecols to adjust if not the case.
+    share_memory is to indicate whether to share the dataframe in memory to 
+    multiple processes -- if set to False, each process will copy the entire dataframe respectively. However, 
+    to read very large dataframe using dask, this option should usually be turned off.
+    """
+    # check some basic things
+    assert csv_file != "_" or parquet_file != "_", "CSV or parquet filepath should be declared"
+
+    if core_num == "NOT DECLARED":
+        core_num = _mp.cpu_count()
+    else:
+        assert core_num <= _mp.cpu_count(
+        ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
+    assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
+
+    # read csv
+    _df, _usecols = _read_csv(csv_file=csv_file,
+                              _usecols=_usecols,
+                              csv_engine=csv_engine,
+                              parquet_file=parquet_file,
+                              sample=sample,
+                              verbose=verbose)
+
+    # share_memory for multiprocess
+    if share_memory == True:
+        # the origingal dataframe is df, store the columns/dtypes pairs
+        df_dtypes_dict = dict(list(zip(_df.columns, _df.dtypes)))
+        # declare a shared Array with data from df
+        mparr = _mp.Array(_ctypes.c_double, _df.values.reshape(-1))
+        # create a new df based on the shared array
+        _df = _pd.DataFrame(_np.frombuffer(mparr.get_obj()).reshape(_df.shape),
+                            columns=_df.columns).astype(df_dtypes_dict)
+
+    def _binary_screening_csv_slice(_slice):
+        def _map_foo(j):
+            __ = [
+                _usecols[0], _usecols[j]
+            ]  # here using _usecol[j] because only input variables indices were splitted
+            _a, _b = _read_two_columns(_df=_df, __=__, csv_engine=csv_engine)
+            return MI_binary_continuous(a=_a,
+                                        b=_b,
+                                        N=N,
+                                        kernel=kernel,
+                                        bw=bw,
+                                        **kwarg)
+
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
+        return _MI_slice
+
+    # multiprocessing starts here
+
+    ind = _np.arange(
+        1, len(_usecols)
+    )  # starting from 1 because the first left column should be the outcome
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    with _mp.Pool(core_num) as pl:
+        MI_df = pl.map(_binary_screening_csv_slice, _iter)
+    MI_df = _np.hstack(MI_df)
+
+    del _df
+
+    return MI_df
+
+
+def continuous_screening_csv_parallel(csv_file="_",
+                                      _usecols=[],
+                                      a_N=300,
+                                      b_N=300,
+                                      kernel="epa",
+                                      bw="silverman",
+                                      norm=2,
+                                      core_num="NOT DECLARED",
+                                      multp=10,
+                                      csv_engine="c",
+                                      parquet_file="_",
+                                      sample=256000,
+                                      verbose=1,
+                                      share_memory=True,
+                                      **kwarg):
+    """
+    (Multiprocessing version) Take a (potentionally large) csv file to calculate the mutual information between outcome and covariates.
+    Both the outcome and the covariates should be continuous. 
+    If _usecols is given, the returned mutual information will match _usecols. 
+    By default, the left first covariate should be the outcome -- use _usecols to adjust if not the case.
+    share_memory is to indicate whether to share the dataframe in memory to 
+    multiple processes -- if set to False, each process will copy the entire dataframe respectively. However, 
+    to read very large dataframe using dask, this option should usually be turned off.
+    """
+    # check some basic things
+    assert csv_file != "_" or parquet_file != "_", "CSV or parquet filepath should be declared"
+
+    if core_num == "NOT DECLARED":
+        core_num = _mp.cpu_count()
+    else:
+        assert core_num <= _mp.cpu_count(
+        ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
+    assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
+
+    # read csv
+    _df, _usecols = _read_csv(csv_file=csv_file,
+                              _usecols=_usecols,
+                              csv_engine=csv_engine,
+                              parquet_file=parquet_file,
+                              sample=sample,
+                              verbose=verbose)
+
+    # share_memory for multiprocess
+    if share_memory == True:
+        # the origingal dataframe is df, store the columns/dtypes pairs
+        df_dtypes_dict = dict(list(zip(_df.columns, _df.dtypes)))
+        # declare a shared Array with data from df
+        mparr = _mp.Array(_ctypes.c_double, _df.values.reshape(-1))
+        # create a new df based on the shared array
+        _df = _pd.DataFrame(_np.frombuffer(mparr.get_obj()).reshape(_df.shape),
+                            columns=_df.columns).astype(df_dtypes_dict)
+
+    def _continuous_screening_csv_slice(_slice):
+        def _map_foo(j):
+            __ = [
+                _usecols[0], _usecols[j]
+            ]  # here using _usecol[j] because only input variables indices were splitted
+            _a, _b = _read_two_columns(_df=_df, __=__, csv_engine=csv_engine)
+            return MI_continuous_continuous(a=_a,
+                                            b=_b,
+                                            a_N=a_N,
+                                            b_N=b_N,
+                                            kernel=kernel,
+                                            bw=bw,
+                                            norm=norm,
+                                            **kwarg)
+
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
+        return _MI_slice
+
+    # multiprocessing starts here
+    ind = _np.arange(
+        1, len(_usecols)
+    )  # starting from 1 because the first left column should be the outcome
+
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    with _mp.Pool(core_num) as pl:
+        MI_df = pl.map(_continuous_screening_csv_slice, _iter)
+    MI_df = _np.hstack(MI_df)
+
+    del _df
+
+    return MI_df
+
+
+def binary_skMI_screening_csv_parallel(csv_file="_",
+                                       _usecols=[],
+                                       n_neighbors=3,
+                                       core_num="NOT DECLARED",
+                                       multp=10,
+                                       csv_engine="c",
+                                       parquet_file="_",
+                                       sample=256000,
+                                       verbose=1,
+                                       share_memory=True,
+                                       **kwarg):
+    """
+    (Multiprocessing version) Take a (potentionally large) csv file to calculate the mutual information between outcome and covariates.
+    Both the outcome and the covariates should be binary. 
+    If _usecols is given, the returned mutual information will match _usecols. 
+    By default, the left first covariate should be the outcome -- use _usecols to adjust if not the case.
+    share_memory is to indicate whether to share the dataframe in memory to 
+    multiple processes -- if set to False, each process will copy the entire dataframe respectively. However, 
+    to read very large dataframe using dask, this option should usually be turned off.
+    """
+    # check some basic things
+    assert csv_file != "_" or parquet_file != "_", "CSV or parquet filepath should be declared"
+
+    if core_num == "NOT DECLARED":
+        core_num = _mp.cpu_count()
+    else:
+        assert core_num <= _mp.cpu_count(
+        ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
+    assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
+
+    # read csv
+    _df, _usecols = _read_csv(csv_file=csv_file,
+                              _usecols=_usecols,
+                              csv_engine=csv_engine,
+                              parquet_file=parquet_file,
+                              sample=sample,
+                              verbose=verbose)
+
+    # share_memory for multiprocess
+    if share_memory == True:
+        # the origingal dataframe is df, store the columns/dtypes pairs
+        df_dtypes_dict = dict(list(zip(_df.columns, _df.dtypes)))
+        # declare a shared Array with data from df
+        mparr = _mp.Array(_ctypes.c_double, _df.values.reshape(-1))
+        # create a new df based on the shared array
+        _df = _pd.DataFrame(_np.frombuffer(mparr.get_obj()).reshape(_df.shape),
+                            columns=_df.columns).astype(df_dtypes_dict)
+
+    def _binary_skMI_df_slice(_slice):
+        def _map_foo(j):
+            __ = [
+                _usecols[0], _usecols[j]
+            ]  # here using _usecol[j] because only input variables indices were splitted
+            _a, _b = _read_two_columns(_df=_df, __=__, csv_engine=csv_engine)
+            return _mutual_info_classif(y=_a.reshape(-1, 1),
+                                        X=_b.reshape(-1, 1),
+                                        n_neighbors=n_neighbors,
+                                        discrete_features=False,
+                                        **kwarg)[0]
+
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
+        return _MI_slice
+
+    # multiprocessing starts here
+    ind = _np.arange(
+        1, len(_usecols)
+    )  # starting from 1 because the first left column should be the outcome
+
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    with _mp.Pool(core_num) as pl:
+        MI_df = pl.map(_binary_skMI_df_slice, _iter)
+    MI_df = _np.hstack(MI_df)
+
+    del _df
+
+    return MI_df
+
+
+def continuous_skMI_screening_csv_parallel(csv_file="_",
+                                           _usecols=[],
+                                           n_neighbors=3,
+                                           core_num="NOT DECLARED",
+                                           multp=10,
+                                           csv_engine="c",
+                                           parquet_file="_",
+                                           sample=256000,
+                                           verbose=1,
+                                           share_memory=True,
+                                           **kwarg):
+    """
+    (Multiprocessing version) Take a (potentionally large) csv file to calculate the mutual information between outcome and covariates.
+    Both the outcome and the covariates should be continuous. 
+    If _usecols is given, the returned mutual information will match _usecols. 
+    By default, the left first covariate should be the outcome -- use _usecols to adjust if not the case.
+    share_memory is to indicate whether to share the dataframe in memory to 
+    multiple processes -- if set to False, each process will copy the entire dataframe respectively. However, 
+    to read very large dataframe using dask, this option should usually be turned off.
+    """
+    # check some basic things
+    assert csv_file != "_" or parquet_file != "_", "CSV or parquet filepath should be declared"
+
+    if core_num == "NOT DECLARED":
+        core_num = _mp.cpu_count()
+    else:
+        assert core_num <= _mp.cpu_count(
+        ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
+    assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
+
+    # read csv
+    _df, _usecols = _read_csv(csv_file=csv_file,
+                              _usecols=_usecols,
+                              csv_engine=csv_engine,
+                              parquet_file=parquet_file,
+                              sample=sample,
+                              verbose=verbose)
+
+    # share_memory for multiprocess
+    if share_memory == True:
+        # the origingal dataframe is df, store the columns/dtypes pairs
+        df_dtypes_dict = dict(list(zip(_df.columns, _df.dtypes)))
+        # declare a shared Array with data from df
+        mparr = _mp.Array(_ctypes.c_double, _df.values.reshape(-1))
+        # create a new df based on the shared array
+        _df = _pd.DataFrame(_np.frombuffer(mparr.get_obj()).reshape(_df.shape),
+                            columns=_df.columns).astype(df_dtypes_dict)
+
+    def _continuous_skMI_df_slice(_slice):
+        def _map_foo(j):
+            __ = [
+                _usecols[0], _usecols[j]
+            ]  # here using _usecol[j] because only input variables indices were splitted
+            _a, _b = _read_two_columns(_df=_df, __=__, csv_engine=csv_engine)
+            return _mutual_info_regression(y=_a.reshape(-1, 1),
+                                           X=_b.reshape(-1, 1),
+                                           n_neighbors=n_neighbors,
+                                           discrete_features=False,
+                                           **kwarg)[0]
+
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
+        return _MI_slice
+
+    # multiprocessing starts here
+    ind = _np.arange(
+        1, len(_usecols)
+    )  # starting from 1 because the first left column should be the outcome
+
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    with _mp.Pool(core_num) as pl:
+        MI_df = pl.map(_continuous_skMI_df_slice, _iter)
+    MI_df = _np.hstack(MI_df)
+
+    del _df
+
+    return MI_df
+
+
+def Pearson_screening_csv_parallel(csv_file="_",
+                                   _usecols=[],
+                                   core_num="NOT DECLARED",
+                                   multp=10,
+                                   csv_engine="c",
+                                   parquet_file="_",
+                                   sample=256000,
+                                   verbose=1,
+                                   share_memory=True):
+    """
+    (Multiprocessing version) Take a (potentionally large) csv file to calculate the Pearson's correlation between outcome and covariates.
+    If _usecols is given, the returned Pearson correlation will match _usecols. 
+    By default, the left first covariate should be the outcome -- use _usecols to adjust if not the case.
+    This function accounts for missing data better than the Pearson's correlation matrix function provided by numpy.
+    share_memory is to indicate whether to share the dataframe in memory to 
+    multiple processes -- if set to False, each process will copy the entire dataframe respectively. However, 
+    to read very large dataframe using dask, this option should usually be turned off.    """
+    # check some basic things
+    assert csv_file != "_" or parquet_file != "_", "CSV or parquet filepath should be declared"
+
+    if core_num == "NOT DECLARED":
+        core_num = _mp.cpu_count()
+    else:
+        assert core_num <= _mp.cpu_count(
+        ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
+    assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
+
+    # read csv
+    _df, _usecols = _read_csv(csv_file=csv_file,
+                              _usecols=_usecols,
+                              csv_engine=csv_engine,
+                              parquet_file=parquet_file,
+                              sample=sample,
+                              verbose=verbose)
+
+    # share_memory for multiprocess
+    if share_memory == True:
+        # the origingal dataframe is df, store the columns/dtypes pairs
+        df_dtypes_dict = dict(list(zip(_df.columns, _df.dtypes)))
+        # declare a shared Array with data from df
+        mparr = _mp.Array(_ctypes.c_double, _df.values.reshape(-1))
+        # create a new df based on the shared array
+        _df = _pd.DataFrame(_np.frombuffer(mparr.get_obj()).reshape(_df.shape),
+                            columns=_df.columns).astype(df_dtypes_dict)
+
+    def _Pearson_screening_df_slice(_slice):
+        def _map_foo(j):
+            __ = [
+                _usecols[0], _usecols[j]
+            ]  # here using _usecol[j] because only input variables indices were splitted
+            _a, _b = _read_two_columns(_df=_df, __=__, csv_engine=csv_engine)
+            # returned Pearson correlation is a symmetric matrix
+            _a -= _np.mean(_a)
+            _a /= _np.std(_a)
+            _b -= _np.mean(_b)
+            _b /= _np.std(_b)
+            #             return _np.corrcoef(_a, _b)[0, 1]
+            return _a @ _b / len(_a)
+
+        _pearson_slice = _np.array(list(map(_map_foo, _slice)))
+        return _pearson_slice
+
+    # multiprocessing starts here
+    ind = _np.arange(
+        1, len(_usecols)
+    )  # starting from 1 because the first left column should be the outcome
+
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    with _mp.Pool(core_num) as pl:
+        Pearson_df = pl.map(_Pearson_screening_df_slice, _iter)
+    Pearson_df = _np.hstack(Pearson_df)
+
+    del _df
+
+    return Pearson_df
+
+
+def clump_continuous_csv_parallel(
+        csv_file="_",
+        _usecols=[],
+        a_N=300,
+        b_N=300,
+        kernel="epa",
+        bw="silverman",
+        norm=2,
+        clumping_threshold=Pearson_to_MI_Gaussian(.6),
+        num_vars_exam=_np.infty,
+        core_num="NOT DECLARED",
+        multp=10,
+        csv_engine="c",
+        parquet_file="_",
+        sample=256000,
+        verbose=1,
+        share_memory=True,
+        **kwarg):
+    """
+    Perform clumping based on mutual information thresholding
+    The clumping process starts from the left to right, preserve input variables under the clumping threshold
+    share_memory is to indicate whether to share the dataframe in memory to 
+    multiple processes -- if set to False, each process will copy the entire dataframe respectively. However, 
+    to read very large dataframe using dask, this option should usually be turned off.    """
+    # initialization
+    _, keep_cols = _read_csv(csv_file=csv_file,
+                             _usecols=_usecols,
+                             csv_engine="dask",
+                             parquet_file=parquet_file,
+                             sample=sample,
+                             verbose=verbose)
+
+    del _
+
+    if num_vars_exam == _np.infty:
+        num_vars_exam = len(keep_cols) - 1
+    _iter = _np.arange(num_vars_exam)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    for current_var_ind in _iter:  # note that here _iter and keep_cols don't need to agree, by the break command comes later
+        if current_var_ind + 1 <= len(keep_cols):
+            _MI = continuous_screening_csv_parallel(
+                csv_file=csv_file,
+                _usecols=keep_cols[current_var_ind:],
+                core_num=core_num,
+                multp=multp,
+                csv_engine=csv_engine,
+                parquet_file=parquet_file,
+                sample=sample,
+                verbose=0,
+                share_memory=share_memory,
+                **kwarg)
+            # current_var_ind + 1 since the current variable will be included anyway
+            keep_cols = _np.hstack(
+                (keep_cols[:current_var_ind + 1],
+                 keep_cols[current_var_ind + 1:][_MI <= clumping_threshold]))
+        else:
+            break
+    return current_var_ind, keep_cols
+
+
+def binary_screening_dataframe(dataframe="_",
+                               _usecols=[],
+                               N=500,
+                               kernel="epa",
+                               bw="silverman",
+                               csv_engine="c",
+                               verbose=1,
+                               **kwarg):
+    """
+    Take a (potentionally large) csv file to calculate the mutual information between outcome and covariates.
+    The outcome should be binary and the covariates be continuous. 
+    If _usecols is given, the returned mutual information will match _usecols. 
+    By default, the left first covariate should be the outcome -- use _usecols to adjust if not the case.
+    """
+    _df = dataframe
     if _np.array(_usecols).size == 0:
-        print(
-            "Variable names not provided -- start reading variable names from csv file now, might take some time, depending on the csv file size."
-        )
-        _usecols = _pd.read_csv(csv_file, index_col=0,
-                                nrows=0).columns.tolist()
-        print("Reading variable names from csv file finished.")
+        _usecols = _np.array(_df.columns.to_list()[1:])
     else:
         _usecols = _np.array(_usecols)
-    MI_csv = _np.empty(len(_usecols) - 1)
-    for j in _np.arange(len(_usecols) - 1):
+
+    def _map_foo(j):
         __ = [
             _usecols[0], _usecols[j + 1]
         ]  # here using _usecol[j + 1] because the left first column is the outcome
-        _ = _pd.read_csv(csv_file,
-                         skipinitialspace=True,
-                         usecols=__,
-                         encoding='unicode_escape').dropna()
-        _a = _[_usecols[0]].to_numpy()
-        _b = _[_usecols[j + 1]].to_numpy()
-        MI_csv[j] = MI_binary_continuous(a=_a,
-                                         b=_b,
-                                         N=N,
-                                         kernel=kernel,
-                                         bw=bw,
-                                         machine_err=machine_err)
-    return MI_csv
-
-
-def continuous_filter_csv(csv_file,
-                          _usecols=[],
-                          a_N=300,
-                          b_N=300,
-                          kernel="epa",
-                          bw="silverman",
-                          norm=2,
-                          machine_err=1e-16):
+        _a, _b = _read_two_columns(_df=_df, __=__, csv_engine=csv_engine)
+        return MI_binary_continuous(a=_a,
+                                    b=_b,
+                                    N=N,
+                                    kernel=kernel,
+                                    bw=bw,
+                                    **kwarg)
+
+    _iter = _np.arange(len(_usecols) - 1)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    MI_df = _np.array(list(map(_map_foo, _iter)))
+
+    return MI_df
+
+
+def continuous_screening_dataframe(dataframe="_",
+                                   _usecols=[],
+                                   a_N=300,
+                                   b_N=300,
+                                   kernel="epa",
+                                   bw="silverman",
+                                   norm=2,
+                                   csv_engine="c",
+                                   verbose=1,
+                                   **kwarg):
     """
     Take a (potentionally large) csv file to calculate the mutual information between outcome and covariates.
     Both the outcome and the covariates should be continuous. 
     If _usecols is given, the returned mutual information will match _usecols. 
     By default, the left first covariate should be the outcome -- use _usecols to adjust if not the case.
     """
+    _df = dataframe
     if _np.array(_usecols).size == 0:
-        print(
-            "Variable names not provided -- start reading variable names from csv file now, might take some time, depending on the csv file size."
-        )
-        _usecols = _pd.read_csv(csv_file, index_col=0,
-                                nrows=0).columns.tolist()
-        print("Reading variable names from csv file finished.")
+        _usecols = _np.array(_df.columns.to_list()[1:])
     else:
         _usecols = _np.array(_usecols)
-    MI_csv = _np.empty(len(_usecols) - 1)
-    for j in _np.arange(len(_usecols) - 1):
+
+    def _map_foo(j):
         __ = [
             _usecols[0], _usecols[j + 1]
         ]  # here using _usecol[j + 1] because the left first column is the outcome
-        _ = _pd.read_csv(csv_file,
-                         skipinitialspace=True,
-                         usecols=__,
-                         encoding='unicode_escape').dropna()
-        _a = _[_usecols[0]].to_numpy()
-        _b = _[_usecols[j + 1]].to_numpy()
-        MI_csv[j] = MI_bivariate_continuous(a=_a,
+        _a, _b = _read_two_columns(_df=_df, __=__, csv_engine=csv_engine)
+        return MI_continuous_continuous(a=_a,
+                                        b=_b,
+                                        a_N=a_N,
+                                        b_N=b_N,
+                                        kernel=kernel,
+                                        bw=bw,
+                                        norm=norm,
+                                        **kwarg)
+
+    _iter = _np.arange(len(_usecols) - 1)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    MI_df = _np.array(list(map(_map_foo, _iter)))
+
+    return MI_df
+
+
+def binary_screening_dataframe_parallel(dataframe="_",
+                                        _usecols=[],
+                                        N=500,
+                                        kernel="epa",
+                                        bw="silverman",
+                                        core_num="NOT DECLARED",
+                                        multp=10,
+                                        csv_engine="c",
+                                        verbose=1,
+                                        share_memory=True,
+                                        **kwarg):
+    """
+    (Multiprocessing version) Take a (potentionally large) csv file to calculate the mutual information between outcome and covariates.
+    The outcome should be binary and the covariates be continuous. 
+    If _usecols is given, the returned mutual information will match _usecols. 
+    By default, the left first covariate should be the outcome -- use _usecols to adjust if not the case.
+    share_memory is to indicate whether to share the dataframe in memory to 
+    multiple processes -- if set to False, each process will copy the entire dataframe respectively. However, 
+    to read very large dataframe using dask, this option should usually be turned off.
+    """
+    if core_num == "NOT DECLARED":
+        core_num = _mp.cpu_count()
+    else:
+        assert core_num <= _mp.cpu_count(
+        ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
+    assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
+
+    _df = dataframe
+    if _np.array(_usecols).size == 0:
+        _usecols = _np.array(_df.columns.to_list()[1:])
+    else:
+        _usecols = _np.array(_usecols)
+
+    # share_memory for multiprocess
+    if share_memory == True:
+        # the origingal dataframe is df, store the columns/dtypes pairs
+        df_dtypes_dict = dict(list(zip(_df.columns, _df.dtypes)))
+        # declare a shared Array with data from df
+        mparr = _mp.Array(_ctypes.c_double, _df.values.reshape(-1))
+        # create a new df based on the shared array
+        _df = _pd.DataFrame(_np.frombuffer(mparr.get_obj()).reshape(_df.shape),
+                            columns=_df.columns).astype(df_dtypes_dict)
+
+    def _binary_screening_csv_slice(_slice):
+        def _map_foo(j):
+            __ = [
+                _usecols[0], _usecols[j]
+            ]  # here using _usecol[j] because only input variables indices were splitted
+            _a, _b = _read_two_columns(_df=_df, __=__, csv_engine=csv_engine)
+            return MI_binary_continuous(a=_a,
+                                        b=_b,
+                                        N=N,
+                                        kernel=kernel,
+                                        bw=bw,
+                                        **kwarg)
+
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
+        return _MI_slice
+
+    # multiprocessing starts here
+
+    ind = _np.arange(
+        1, len(_usecols)
+    )  # starting from 1 because the first left column should be the outcome
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    with _mp.Pool(core_num) as pl:
+        MI_df = pl.map(_binary_screening_csv_slice, _iter)
+    MI_df = _np.hstack(MI_df)
+
+    return MI_df
+
+
+def continuous_screening_dataframe_parallel(dataframe="_",
+                                            _usecols=[],
+                                            a_N=300,
+                                            b_N=300,
+                                            kernel="epa",
+                                            bw="silverman",
+                                            norm=2,
+                                            core_num="NOT DECLARED",
+                                            multp=10,
+                                            csv_engine="c",
+                                            verbose=1,
+                                            share_memory=True,
+                                            **kwarg):
+    """
+    (Multiprocessing version) Take a (potentionally large) csv file to calculate the mutual information between outcome and covariates.
+    Both the outcome and the covariates should be continuous. 
+    If _usecols is given, the returned mutual information will match _usecols. 
+    By default, the left first covariate should be the outcome -- use _usecols to adjust if not the case.
+    share_memory is to indicate whether to share the dataframe in memory to 
+    multiple processes -- if set to False, each process will copy the entire dataframe respectively. However, 
+    to read very large dataframe using dask, this option should usually be turned off.
+    """
+    if core_num == "NOT DECLARED":
+        core_num = _mp.cpu_count()
+    else:
+        assert core_num <= _mp.cpu_count(
+        ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
+    assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
+
+    _df = dataframe
+    if _np.array(_usecols).size == 0:
+        _usecols = _np.array(_df.columns.to_list()[1:])
+    else:
+        _usecols = _np.array(_usecols)
+
+    # share_memory for multiprocess
+    if share_memory == True:
+        # the origingal dataframe is df, store the columns/dtypes pairs
+        df_dtypes_dict = dict(list(zip(_df.columns, _df.dtypes)))
+        # declare a shared Array with data from df
+        mparr = _mp.Array(_ctypes.c_double, _df.values.reshape(-1))
+        # create a new df based on the shared array
+        _df = _pd.DataFrame(_np.frombuffer(mparr.get_obj()).reshape(_df.shape),
+                            columns=_df.columns).astype(df_dtypes_dict)
+
+    def _continuous_screening_csv_slice(_slice):
+        def _map_foo(j):
+            __ = [
+                _usecols[0], _usecols[j]
+            ]  # here using _usecol[j] because only input variables indices were splitted
+            _a, _b = _read_two_columns(_df=_df, __=__, csv_engine=csv_engine)
+            return MI_continuous_continuous(a=_a,
                                             b=_b,
                                             a_N=a_N,
                                             b_N=b_N,
                                             kernel=kernel,
                                             bw=bw,
                                             norm=norm,
-                                            machine_err=machine_err)
-    return MI_csv
+                                            **kwarg)
 
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
+        return _MI_slice
 
-def binary_filter_csv_parallel(csv_file,
-                               _usecols=[],
-                               N=500,
-                               kernel="epa",
-                               bw="silverman",
-                               machine_err=1e-16,
-                               core_num="NOT DECLARED",
-                               multp=1):
+    # multiprocessing starts here
+    ind = _np.arange(
+        1, len(_usecols)
+    )  # starting from 1 because the first left column should be the outcome
+
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    with _mp.Pool(core_num) as pl:
+        MI_df = pl.map(_continuous_screening_csv_slice, _iter)
+    MI_df = _np.hstack(MI_df)
+
+    return MI_df
+
+
+def binary_skMI_screening_dataframe_parallel(dataframe="_",
+                                             _usecols=[],
+                                             n_neighbors=3,
+                                             core_num="NOT DECLARED",
+                                             multp=10,
+                                             csv_engine="c",
+                                             verbose=1,
+                                             share_memory=True,
+                                             **kwarg):
     """
     (Multiprocessing version) Take a (potentionally large) csv file to calculate the mutual information between outcome and covariates.
-    The outcome should be binary and the covariates be continuous. 
+    Both the outcome and the covariates should be binary. 
     If _usecols is given, the returned mutual information will match _usecols. 
     By default, the left first covariate should be the outcome -- use _usecols to adjust if not the case.
+    share_memory is to indicate whether to share the dataframe in memory to 
+    multiple processes -- if set to False, each process will copy the entire dataframe respectively. However, 
+    to read very large dataframe using dask, this option should usually be turned off.
     """
     if core_num == "NOT DECLARED":
         core_num = _mp.cpu_count()
     else:
         assert core_num <= _mp.cpu_count(
         ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
     assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
 
+    _df = dataframe
     if _np.array(_usecols).size == 0:
-        print(
-            "Variable names not provided -- start reading variable names from csv file now, might take some time, depending on the csv file size."
-        )
-        _usecols = _pd.read_csv(csv_file, index_col=0,
-                                nrows=0).columns.tolist()
-        print("Reading variable names from csv file finished.")
+        _usecols = _np.array(_df.columns.to_list()[1:])
     else:
         _usecols = _np.array(_usecols)
 
-    def _binary_filter_csv_slice(_slice):
-        _MI_slice = _np.zeros(
-            len(_slice))  # returned MI should be of the same length as slice
-        k = 0
-        for j in _slice:
+    # share_memory for multiprocess
+    if share_memory == True:
+        # the origingal dataframe is df, store the columns/dtypes pairs
+        df_dtypes_dict = dict(list(zip(_df.columns, _df.dtypes)))
+        # declare a shared Array with data from df
+        mparr = _mp.Array(_ctypes.c_double, _df.values.reshape(-1))
+        # create a new df based on the shared array
+        _df = _pd.DataFrame(_np.frombuffer(mparr.get_obj()).reshape(_df.shape),
+                            columns=_df.columns).astype(df_dtypes_dict)
+
+    def _binary_skMI_df_slice(_slice):
+        def _map_foo(j):
             __ = [
                 _usecols[0], _usecols[j]
             ]  # here using _usecol[j] because only input variables indices were splitted
-            _ = _pd.read_csv(csv_file,
-                             skipinitialspace=True,
-                             usecols=__,
-                             encoding='unicode_escape').dropna()
-            _a = _[_usecols[0]].to_numpy()
-            _b = _[_usecols[j]].to_numpy()
-            _MI_slice[k] = MI_binary_continuous(a=_a,
-                                                b=_b,
-                                                N=N,
-                                                kernel=kernel,
-                                                bw=bw,
-                                                machine_err=machine_err)
-            k += 1
+            _a, _b = _read_two_columns(_df=_df, __=__, csv_engine=csv_engine)
+            return _mutual_info_classif(y=_a.reshape(-1, 1),
+                                        X=_b.reshape(-1, 1),
+                                        n_neighbors=n_neighbors,
+                                        discrete_features=False,
+                                        **kwarg)[0]
+
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
         return _MI_slice
 
     # multiprocessing starts here
     ind = _np.arange(
         1, len(_usecols)
     )  # starting from 1 because the first left column should be the outcome
+
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
     with _mp.Pool(core_num) as pl:
-        MI_csv = pl.map(_binary_filter_csv_slice,
-                        _np.array_split(ind, core_num * multp))
-    MI_csv = _np.hstack(MI_csv)
-    return MI_csv
+        MI_df = pl.map(_binary_skMI_df_slice, _iter)
+    MI_df = _np.hstack(MI_df)
 
+    return MI_df
 
-def continuous_filter_csv_parallel(csv_file,
-                                   _usecols=[],
-                                   a_N=300,
-                                   b_N=300,
-                                   kernel="epa",
-                                   bw="silverman",
-                                   norm=2,
-                                   machine_err=1e-16,
-                                   core_num="NOT DECLARED",
-                                   multp=1):
+
+def continuous_skMI_screening_dataframe_parallel(dataframe="_",
+                                                 _usecols=[],
+                                                 n_neighbors=3,
+                                                 core_num="NOT DECLARED",
+                                                 multp=10,
+                                                 csv_engine="c",
+                                                 verbose=1,
+                                                 share_memory=True,
+                                                 **kwarg):
     """
     (Multiprocessing version) Take a (potentionally large) csv file to calculate the mutual information between outcome and covariates.
     Both the outcome and the covariates should be continuous. 
     If _usecols is given, the returned mutual information will match _usecols. 
     By default, the left first covariate should be the outcome -- use _usecols to adjust if not the case.
+    share_memory is to indicate whether to share the dataframe in memory to 
+    multiple processes -- if set to False, each process will copy the entire dataframe respectively. However, 
+    to read very large dataframe using dask, this option should usually be turned off.
     """
     if core_num == "NOT DECLARED":
         core_num = _mp.cpu_count()
     else:
         assert core_num <= _mp.cpu_count(
         ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
     assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
 
+    _df = dataframe
     if _np.array(_usecols).size == 0:
-        print(
-            "Variable names not provided -- start reading variable names from csv file now, might take some time, depending on the csv file size."
-        )
-        _usecols = _pd.read_csv(csv_file, index_col=0,
-                                nrows=0).columns.tolist()
-        print("Reading variable names from csv file finished.")
+        _usecols = _np.array(_df.columns.to_list()[1:])
     else:
         _usecols = _np.array(_usecols)
 
-    def _binary_filter_csv_slice(_slice):
-        _MI_slice = _np.zeros(
-            len(_slice))  # returned MI should be of the same length as slice
-        k = 0
-        for j in _slice:
+    # share_memory for multiprocess
+    if share_memory == True:
+        # the origingal dataframe is df, store the columns/dtypes pairs
+        df_dtypes_dict = dict(list(zip(_df.columns, _df.dtypes)))
+        # declare a shared Array with data from df
+        mparr = _mp.Array(_ctypes.c_double, _df.values.reshape(-1))
+        # create a new df based on the shared array
+        _df = _pd.DataFrame(_np.frombuffer(mparr.get_obj()).reshape(_df.shape),
+                            columns=_df.columns).astype(df_dtypes_dict)
+
+    def _continuous_skMI_df_slice(_slice):
+        def _map_foo(j):
             __ = [
                 _usecols[0], _usecols[j]
             ]  # here using _usecol[j] because only input variables indices were splitted
-            _ = _pd.read_csv(csv_file,
-                             skipinitialspace=True,
-                             usecols=__,
-                             encoding='unicode_escape').dropna()
-            _a = _[_usecols[0]].to_numpy()
-            _b = _[_usecols[j]].to_numpy()
-            _MI_slice[k] = MI_bivariate_continuous(a=_a,
-                                                   b=_b,
-                                                   a_N=a_N,
-                                                   b_N=b_N,
-                                                   kernel=kernel,
-                                                   bw=bw,
-                                                   norm=norm,
-                                                   machine_err=machine_err)
-            k += 1
+            _a, _b = _read_two_columns(_df=_df, __=__, csv_engine=csv_engine)
+            return _mutual_info_regression(y=_a.reshape(-1, 1),
+                                           X=_b.reshape(-1, 1),
+                                           n_neighbors=n_neighbors,
+                                           discrete_features=False,
+                                           **kwarg)[0]
+
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
         return _MI_slice
 
     # multiprocessing starts here
     ind = _np.arange(
         1, len(_usecols)
     )  # starting from 1 because the first left column should be the outcome
+
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
     with _mp.Pool(core_num) as pl:
-        MI_csv = pl.map(_binary_filter_csv_slice,
-                        _np.array_split(ind, core_num * multp))
-    MI_csv = _np.hstack(MI_csv)
-    return MI_csv
+        MI_df = pl.map(_continuous_skMI_df_slice, _iter)
+    MI_df = _np.hstack(MI_df)
+
+    return MI_df
 
 
-def Pearson_filter_csv_parallel(csv_file,
-                                _usecols=[],
-                                core_num="NOT DECLARED",
-                                multp=1):
+def Pearson_screening_dataframe_parallel(dataframe="_",
+                                         _usecols=[],
+                                         core_num="NOT DECLARED",
+                                         multp=10,
+                                         csv_engine="c",
+                                         verbose=1,
+                                         share_memory=True):
     """
     (Multiprocessing version) Take a (potentionally large) csv file to calculate the Pearson's correlation between outcome and covariates.
     If _usecols is given, the returned Pearson correlation will match _usecols. 
     By default, the left first covariate should be the outcome -- use _usecols to adjust if not the case.
     This function accounts for missing data better than the Pearson's correlation matrix function provided by numpy.
+    share_memory is to indicate whether to share the dataframe in memory to 
+    multiple processes -- if set to False, each process will copy the entire dataframe respectively. However, 
+    to read very large dataframe using dask, this option should usually be turned off.    
     """
     if core_num == "NOT DECLARED":
         core_num = _mp.cpu_count()
     else:
         assert core_num <= _mp.cpu_count(
         ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
     assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
 
+    _df = dataframe
     if _np.array(_usecols).size == 0:
-        print(
-            "Variable names not provided -- start reading variable names from csv file now, might take some time, depending on the csv file size."
-        )
-        _usecols = _pd.read_csv(csv_file, index_col=0,
-                                nrows=0).columns.tolist()
-        print("Reading variable names from csv file finished.")
+        _usecols = _np.array(_df.columns.to_list()[1:])
     else:
         _usecols = _np.array(_usecols)
 
-    def _Pearson_filter_csv_slice(_slice):
-        _pearson_slice = _np.zeros(
-            len(_slice))  # returned MI should be of the same length as slice
-        k = 0
-        for j in _slice:
+    # share_memory for multiprocess
+    if share_memory == True:
+        # the origingal dataframe is df, store the columns/dtypes pairs
+        df_dtypes_dict = dict(list(zip(_df.columns, _df.dtypes)))
+        # declare a shared Array with data from df
+        mparr = _mp.Array(_ctypes.c_double, _df.values.reshape(-1))
+        # create a new df based on the shared array
+        _df = _pd.DataFrame(_np.frombuffer(mparr.get_obj()).reshape(_df.shape),
+                            columns=_df.columns).astype(df_dtypes_dict)
+
+    def _Pearson_screening_df_slice(_slice):
+        def _map_foo(j):
             __ = [
                 _usecols[0], _usecols[j]
             ]  # here using _usecol[j] because only input variables indices were splitted
-            _ = _pd.read_csv(csv_file,
-                             skipinitialspace=True,
-                             usecols=__,
-                             encoding='unicode_escape').dropna()
-            _a = _[_usecols[0]].to_numpy()
-            _b = _[_usecols[j]].to_numpy()
+            _a, _b = _read_two_columns(_df=_df, __=__, csv_engine=csv_engine)
             # returned Pearson correlation is a symmetric matrix
-            _pearson_slice[k] = _np.corrcoef(_a, _b)[0, 1]
-            k += 1
+            _a -= _np.mean(_a)
+            _a /= _np.std(_a)
+            _b -= _np.mean(_b)
+            _b /= _np.std(_b)
+            #             return _np.corrcoef(_a, _b)[0, 1]
+            return _a @ _b / len(_a)
+
+        _pearson_slice = _np.array(list(map(_map_foo, _slice)))
         return _pearson_slice
 
     # multiprocessing starts here
     ind = _np.arange(
         1, len(_usecols)
     )  # starting from 1 because the first left column should be the outcome
+
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    with _mp.Pool(core_num) as pl:
+        Pearson_df = pl.map(_Pearson_screening_df_slice, _iter)
+    Pearson_df = _np.hstack(Pearson_df)
+
+    return Pearson_df
+
+
+def clump_continuous_dataframe_parallel(
+        dataframe="_",
+        _usecols=[],
+        a_N=300,
+        b_N=300,
+        kernel="epa",
+        bw="silverman",
+        norm=2,
+        clumping_threshold=Pearson_to_MI_Gaussian(.6),
+        num_vars_exam=_np.infty,
+        core_num="NOT DECLARED",
+        multp=10,
+        csv_engine="c",
+        verbose=1,
+        share_memory=True,
+        **kwarg):
+    """
+    Perform clumping based on mutual information thresholding
+    The clumping process starts from the left to right, preserve input variables under the clumping threshold
+    share_memory is to indicate whether to share the dataframe in memory to 
+    multiple processes -- if set to False, each process will copy the entire dataframe respectively. However, 
+    to read very large dataframe using dask, this option should usually be turned off.    """
+    # initialization
+    _df = dataframe
+    if _np.array(_usecols).size == 0:
+        _usecols = _np.array(_df.columns.to_list()[1:])
+    else:
+        _usecols = _np.array(_usecols)
+
+    if num_vars_exam == _np.infty:
+        num_vars_exam = len(keep_cols) - 1
+    _iter = _np.arange(num_vars_exam)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    for current_var_ind in _iter:  # note that here _iter and keep_cols don't need to agree, by the break command comes later
+        if current_var_ind + 1 <= len(keep_cols):
+            _MI = continuous_screening_dataframe_parallel(
+                dataframe=dataframe,
+                _usecols=keep_cols[current_var_ind:],
+                core_num=core_num,
+                multp=multp,
+                csv_engine=csv_engine,
+                parquet_file=parquet_file,
+                sample=sample,
+                verbose=0,
+                share_memory=share_memory,
+                **kwarg)
+            # current_var_ind + 1 since the current variable will be included anyway
+            keep_cols = _np.hstack(
+                (keep_cols[:current_var_ind + 1],
+                 keep_cols[current_var_ind + 1:][_MI <= clumping_threshold]))
+        else:
+            break
+    return current_var_ind, keep_cols
+
+
+def continuous_skMI_array_parallel(X,
+                                   y,
+                                   drop_na=True,
+                                   n_neighbors=3,
+                                   core_num="NOT DECLARED",
+                                   multp=10,
+                                   verbose=1,
+                                   **kwarg):
+    """
+    (Multiprocessing version) Calculate the mutual information using sklearn implementation between outcome and covariates.
+    The outcome should be binary and the covariates be continuous. 
+    If drop_na is set to be True, the NaN values will be dropped in a bivariate manner. 
+    """
+    # check some basic things
+    if core_num == "NOT DECLARED":
+        core_num = _mp.cpu_count()
+    else:
+        assert core_num <= _mp.cpu_count(
+        ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
+    assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
+
+    def _continuous_skMI_array_slice(_slice):
+        def _map_foo(j):
+            _a, _b = y.copy(), X[:, j].copy()
+            if drop_na == True:
+                _keep = _np.logical_not(
+                    _np.logical_or(_np.isnan(_a), _np.isnan(_b)))
+                _a, _b = _a[_keep], _b[_keep]
+            return _mutual_info_regression(y=_a.reshape(-1, 1),
+                                           X=_b.reshape(-1, 1),
+                                           n_neighbors=n_neighbors,
+                                           discrete_features=False,
+                                           **kwarg)[0]
+
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
+        return _MI_slice
+
+    # multiprocessing starts here
+    ind = _np.arange(X.shape[1])
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    with _mp.Pool(core_num) as pl:
+        MI_array = pl.map(_continuous_skMI_array_slice, _iter)
+    MI_array = _np.hstack(MI_array)
+    return MI_array
+
+
+def binary_screening_array(X,
+                           y,
+                           drop_na=True,
+                           N=500,
+                           kernel="epa",
+                           bw="silverman",
+                           verbose=1,
+                           **kwarg):
+    """
+    Take a numpy file to calculate the mutual information between outcome and covariates.
+    The outcome should be binary and the covariates be continuous. 
+    If drop_na is set to be True, the NaN values will be dropped in a bivariate manner. 
+    """
+    def _map_foo(j):
+        _a, _b = y.copy(), X[:, j].copy()
+        if drop_na == True:
+            _keep = _np.logical_not(
+                _np.logical_or(_np.isnan(_a), _np.isnan(_b)))
+            _a, _b = _a[_keep], _b[_keep]
+        return MI_binary_continuous(a=_a,
+                                    b=_b,
+                                    N=N,
+                                    kernel=kernel,
+                                    bw=bw,
+                                    **kwarg)
+
+    _iter = _np.arange(X.shape[1])
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    MI_array = _np.array(list(map(_map_foo, _iter)))
+    return MI_array
+
+
+def continuous_screening_array(X,
+                               y,
+                               drop_na=True,
+                               a_N=300,
+                               b_N=300,
+                               kernel="epa",
+                               bw="silverman",
+                               norm=2,
+                               verbose=1,
+                               **kwarg):
+    """
+    Take a numpy file to calculate the mutual information between outcome and covariates.
+    The outcome should be continuous and the covariates be continuous. 
+    If drop_na is set to be True, the NaN values will be dropped in a bivariate manner. 
+    """
+    def _map_foo(j):
+        _a, _b = y.copy(), X[:, j].copy()
+        if drop_na == True:
+            _keep = _np.logical_not(
+                _np.logical_or(_np.isnan(_a), _np.isnan(_b)))
+            _a, _b = _a[_keep], _b[_keep]
+        return MI_continuous_continuous(a=_a,
+                                        b=_b,
+                                        a_N=a_N,
+                                        b_N=b_N,
+                                        kernel=kernel,
+                                        bw=bw,
+                                        norm=norm,
+                                        **kwarg)
+
+    _iter = _np.arange(X.shape[1])
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    MI_array = _np.array(list(map(_map_foo, _iter)))
+    return MI_array
+
+
+def binary_screening_array_parallel(X,
+                                    y,
+                                    drop_na=True,
+                                    N=500,
+                                    kernel="epa",
+                                    bw="silverman",
+                                    core_num="NOT DECLARED",
+                                    multp=10,
+                                    verbose=1,
+                                    **kwarg):
+    """
+    (Multiprocessing version) Calculate the mutual information between outcome and covariates.
+    The outcome should be binary and the covariates be continuous. 
+    If drop_na is set to be True, the NaN values will be dropped in a bivariate manner. 
+    """
+    # check some basic things
+    if core_num == "NOT DECLARED":
+        core_num = _mp.cpu_count()
+    else:
+        assert core_num <= _mp.cpu_count(
+        ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
+    assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
+
+    def _binary_screening_array_slice(_slice):
+        def _map_foo(j):
+            _a, _b = y.copy(), X[:, j].copy()
+            if drop_na == True:
+                _keep = _np.logical_not(
+                    _np.logical_or(_np.isnan(_a), _np.isnan(_b)))
+                _a, _b = _a[_keep], _b[_keep]
+            return MI_binary_continuous(a=_a,
+                                        b=_b,
+                                        N=N,
+                                        kernel=kernel,
+                                        bw=bw,
+                                        **kwarg)
+
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
+        return _MI_slice
+
+    # multiprocessing starts here
+    ind = _np.arange(
+        X.shape[1]
+    )  # starting from 1 because the first left column should be the outcome
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    with _mp.Pool(core_num) as pl:
+        MI_array = pl.map(_binary_screening_csv_slice, _iter)
+    MI_array = _np.hstack(MI_array)
+    return MI_array
+
+
+def continuous_screening_array_parallel(X,
+                                        y,
+                                        drop_na=True,
+                                        a_N=300,
+                                        b_N=300,
+                                        kernel="epa",
+                                        bw="silverman",
+                                        norm=2,
+                                        core_num="NOT DECLARED",
+                                        multp=10,
+                                        verbose=1,
+                                        **kwarg):
+    """
+    (Multiprocessing version) Calculate the mutual information between outcome and covariates.
+    The outcome should be continuous and the covariates be continuous. 
+    If drop_na is set to be True, the NaN values will be dropped in a bivariate manner. 
+    """
+    # check some basic things
+    if core_num == "NOT DECLARED":
+        core_num = _mp.cpu_count()
+    else:
+        assert core_num <= _mp.cpu_count(
+        ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
+    assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
+
+    def _continuous_screening_array_slice(_slice):
+        def _map_foo(j):
+            _a, _b = y.copy(), X[:, j].copy()
+            if drop_na == True:
+                _keep = _np.logical_not(
+                    _np.logical_or(_np.isnan(_a), _np.isnan(_b)))
+                _a, _b = _a[_keep], _b[_keep]
+            return MI_continuous_continuous(a=_a,
+                                            b=_b,
+                                            a_N=a_N,
+                                            b_N=b_N,
+                                            kernel=kernel,
+                                            bw=bw,
+                                            norm=norm,
+                                            **kwarg)
+
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
+        return _MI_slice
+
+    # multiprocessing starts here
+    ind = _np.arange(X.shape[1])
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    with _mp.Pool(core_num) as pl:
+        MI_array = pl.map(_continuous_screening_array_slice, _iter)
+    MI_array = _np.hstack(MI_array)
+    return MI_array
+
+
+def binary_skMI_array_parallel(X,
+                               y,
+                               drop_na=True,
+                               n_neighbors=3,
+                               core_num="NOT DECLARED",
+                               multp=10,
+                               verbose=1,
+                               **kwarg):
+    """
+    (Multiprocessing version) Calculate the mutual information using sklearn implementation between outcome and covariates.
+    The outcome should be binary and the covariates be binary. 
+    If drop_na is set to be True, the NaN values will be dropped in a bivariate manner. 
+    """
+    # check some basic things
+    if core_num == "NOT DECLARED":
+        core_num = _mp.cpu_count()
+    else:
+        assert core_num <= _mp.cpu_count(
+        ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
+    assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
+
+    def _binary_skMI_array_slice(_slice):
+        def _map_foo(j):
+            _a, _b = y.copy(), X[:, j].copy()
+            if drop_na == True:
+                _keep = _np.logical_not(
+                    _np.logical_or(_np.isnan(_a), _np.isnan(_b)))
+                _a, _b = _a[_keep], _b[_keep]
+            return _mutual_info_classif(y=_a.reshape(-1, 1),
+                                        X=_b.reshape(-1, 1),
+                                        n_neighbors=n_neighbors,
+                                        discrete_features=False,
+                                        **kwarg)[0]
+
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
+        return _MI_slice
+
+    # multiprocessing starts here
+    ind = _np.arange(X.shape[1])
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    with _mp.Pool(core_num) as pl:
+        MI_array = pl.map(_binary_skMI_array_slice, _iter)
+    MI_array = _np.hstack(MI_array)
+    return MI_array
+
+
+def continuous_skMI_array_parallel(X,
+                                   y,
+                                   drop_na=True,
+                                   n_neighbors=3,
+                                   core_num="NOT DECLARED",
+                                   multp=10,
+                                   verbose=1,
+                                   **kwarg):
+    """
+    (Multiprocessing version) Calculate the mutual information using sklearn implementation between outcome and covariates.
+    The outcome should be binary and the covariates be continuous. 
+    If drop_na is set to be True, the NaN values will be dropped in a bivariate manner. 
+    """
+    # check some basic things
+    if core_num == "NOT DECLARED":
+        core_num = _mp.cpu_count()
+    else:
+        assert core_num <= _mp.cpu_count(
+        ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
+    assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
+
+    def _continuous_skMI_array_slice(_slice):
+        def _map_foo(j):
+            _a, _b = y.copy(), X[:, j].copy()
+            if drop_na == True:
+                _keep = _np.logical_not(
+                    _np.logical_or(_np.isnan(_a), _np.isnan(_b)))
+                _a, _b = _a[_keep], _b[_keep]
+            return _mutual_info_regression(y=_a.reshape(-1, 1),
+                                           X=_b.reshape(-1, 1),
+                                           n_neighbors=n_neighbors,
+                                           discrete_features=False,
+                                           **kwarg)[0]
+
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
+        return _MI_slice
+
+    # multiprocessing starts here
+    ind = _np.arange(X.shape[1])
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
+    with _mp.Pool(core_num) as pl:
+        MI_array = pl.map(_continuous_skMI_array_slice, _iter)
+    MI_array = _np.hstack(MI_array)
+    return MI_array
+
+
+def continuous_Pearson_array_parallel(X,
+                                      y,
+                                      drop_na=True,
+                                      n_neighbors=3,
+                                      core_num="NOT DECLARED",
+                                      multp=10,
+                                      verbose=1):
+    """
+    (Multiprocessing version) Calculate the mutual information using sklearn implementation between outcome and covariates.
+    The outcome should be binary and the covariates be continuous. 
+    If drop_na is set to be True, the NaN values will be dropped in a bivariate manner. 
+    """
+    # check some basic things
+    if core_num == "NOT DECLARED":
+        core_num = _mp.cpu_count()
+    else:
+        assert core_num <= _mp.cpu_count(
+        ), "Declared number of cores used for multiprocessing should not exceed number of cores on this machine."
+    assert core_num >= 2, "Multiprocessing should not be used on single-core machines."
+
+    def _continuous_Pearson_array_slice(_slice):
+        def _map_foo(j):
+            _a, _b = y.copy(), X[:, j].copy()
+            if drop_na == True:
+                _keep = _np.logical_not(
+                    _np.logical_or(_np.isnan(_a), _np.isnan(_b)))
+                _a, _b = _a[_keep], _b[_keep]
+            _a -= _np.mean(_a)
+            _a /= _np.std(_a)
+            _b -= _np.mean(_b)
+            _b /= _np.std(_b)
+            return _a @ _b / len(_a)
+
+        _MI_slice = _np.array(list(map(_map_foo, _slice)))
+        return _MI_slice
+
+    # multiprocessing starts here
+    ind = _np.arange(X.shape[1])
+    _iter = _np.array_split(ind, core_num * multp)
+    if verbose >= 1:
+        _iter = _tqdm(_iter)
     with _mp.Pool(core_num) as pl:
-        Pearson_csv = pl.map(_Pearson_filter_csv_slice,
-                             _np.array_split(ind, core_num * multp))
-    Pearson_csv = _np.hstack(Pearson_csv)
-    return Pearson_csv
+        MI_array = pl.map(_continuous_Pearson_array_slice, _iter)
+    MI_array = _np.hstack(MI_array)
+    return MI_array
 
 
 ##################################################################
-################ some fudamentals things #########################
+################### some fudamentals things ######################
 ##################################################################
 ######################################  some SCAD and MCP things  #######################################
 @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def soft_thresholding(x, lambda_):
     '''
-    To calculate soft-thresholding mapping of a given ONE-DIMENSIONAL tensor, BESIDES THE FIRST TERM (so beta_0 will not be penalized).
-    This function is to be used for calculation involving L1 penalty term later.
+    To calculate soft-thresholding mapping of a given ONE-DIMENSIONAL tensor, BESIDES THE FIRST TERM (so beta_0 will not be penalized). 
+    This function is to be used for calculation involving L1 penalty term later. 
     '''
     return _np.hstack((_np.array([x[0]]),
                        _np.where(
                            _np.abs(x[1:]) > lambda_,
                            x[1:] - _np.sign(x[1:]) * lambda_, 0)))
 
 
@@ -679,15 +1994,15 @@
 
 @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def SCAD(x, lambda_, a=3.7):
     '''
     To calculate SCAD penalty value;
     #x can be a multi-dimensional tensor;
     lambda_, a are scalars;
-    Fan and Li suggests to take a as 3.7
+    Fan and Li suggests to take a as 3.7 
     '''
     # here I notice the function is de facto a function of absolute value of x, therefore take absolute value first to simplify calculation
     x = _np.abs(x)
     temp = _np.where(
         x <= lambda_, lambda_ * x,
         _np.where(x < a * lambda_,
                   (2 * a * lambda_ * x - x**2 - lambda_**2) / (2 * (a - 1)),
@@ -695,115 +2010,118 @@
     temp[0] = 0.  # this is to NOT penalize intercept beta later
     return temp
 
 
 @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def SCAD_grad(x, lambda_, a=3.7):
     '''
-    To calculate the gradient of SCAD wrt. input x;
-    #x can be a multi-dimensional tensor.
+    To calculate the gradient of SCAD wrt. input x; 
+    #x can be a multi-dimensional tensor. 
     '''
     # here decompose x to sign and its absolute value for easier calculation
     sgn = _np.sign(x)
     x = _np.abs(x)
     temp = _np.where(
         x <= lambda_, lambda_ * sgn,
         _np.where(x < a * lambda_, (a * lambda_ * sgn - sgn * x) / (a - 1), 0))
     temp[0] = 0.  # this is to NOT penalize intercept beta later
     return temp
 
 
 @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def MCP(x, lambda_, gamma):
     '''
-    To calculate MCP penalty value;
-    #x can be a multi-dimensional tensor.
+    To calculate MCP penalty value; 
+    #x can be a multi-dimensional tensor. 
     '''
     # the function is a function of absolute value of x
     x = _np.abs(x)
     temp = _np.where(x <= gamma * lambda_, lambda_ * x - x**2 / (2 * gamma),
                      .5 * gamma * lambda_**2)
     temp[0] = 0.  # this is to NOT penalize intercept beta later
     return temp
 
 
 @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def MCP_grad(x, lambda_, gamma):
     '''
-    To calculate MCP gradient wrt. input x;
-    #x can be a multi-dimensional tensor.
+    To calculate MCP gradient wrt. input x; 
+    #x can be a multi-dimensional tensor. 
     '''
     temp = _np.where(
         _np.abs(x) < gamma * lambda_,
         lambda_ * _np.sign(x) - x / gamma, _np.zeros_like(x))
     temp[0] = 0.  # this is to NOT penalize intercept beta later
     return temp
 
 
 @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def SCAD_concave(x, lambda_, a=3.7):
     '''
-    The value of concave part of SCAD penalty;
-    #x can be a multi-dimensional tensor.
+    The value of concave part of SCAD penalty; 
+    #x can be a multi-dimensional tensor. 
     '''
     x = _np.abs(x)
     temp = _np.where(
         x <= lambda_, 0.,
         _np.where(x < a * lambda_,
                   (lambda_ * x - (x**2 + lambda_**2) / 2) / (a - 1),
                   (a + 1) / 2 * lambda_**2 - lambda_ * x))
     temp[0] = 0.  # this is to NOT penalize intercept beta later
     return temp
 
 
 @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def SCAD_concave_grad(x, lambda_, a=3.7):
     '''
-    The gradient of concave part of SCAD penalty wrt. input x;
-    #x can be a multi-dimensional tensor.
+    The gradient of concave part of SCAD penalty wrt. input x; 
+    #x can be a multi-dimensional tensor. 
     '''
     sgn = _np.sign(x)
     x = _np.abs(x)
     temp = _np.where(
         x <= lambda_, 0.,
         _np.where(x < a * lambda_, (lambda_ * sgn - sgn * x) / (a - 1),
                   -lambda_ * sgn))
     temp[0] = 0.  # this is to NOT penalize intercept beta later
     return temp
 
 
 @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def MCP_concave(x, lambda_, gamma):
     '''
-    The value of concave part of MCP penalty;
-    #x can be a multi-dimensional tensor.
+    The value of concave part of MCP penalty; 
+    #x can be a multi-dimensional tensor. 
     '''
     # similiar as in MCP
     x = _np.abs(x)
     temp = _np.where(x <= gamma * lambda_, -(x**2) / (2 * gamma),
                      (gamma * lambda_**2) / 2 - lambda_ * x)
     temp[0] = 0.  # this is to NOT penalize intercept beta later
     return temp
 
 
 @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def MCP_concave_grad(x, lambda_, gamma):
     '''
-    The gradient of concave part of MCP penalty wrt. input x;
-    #x can be a multi-dimensional tensor.
+    The gradient of concave part of MCP penalty wrt. input x; 
+    #x can be a multi-dimensional tensor. 
     '''
     temp = _np.where(
         _np.abs(x) < gamma * lambda_, -x / gamma, -lambda_ * _np.sign(x))
     temp[0] = 0.  # this is to NOT penalize intercept beta later
     return temp
 
+
 ##################################################################
 ######## some fudamentals things for the PCA versions ############
 ##################################################################
 ######################################  some SCAD and MCP things  #######################################
+
+
 @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def soft_thresholding_PCA(x, lambda_, pca_p):
     '''
     To calculate soft-thresholding mapping of a given ONE-DIMENSIONAL tensor, BESIDES THE FIRST TERM (so beta_0 will not be penalized).
     This function is to be used for calculation involving L1 penalty term later.
     '''
     return _np.hstack(
@@ -932,15 +2250,14 @@
     '''
     temp = _np.where(
         _np.abs(x) < gamma * lambda_, -x / gamma, -lambda_ * _np.sign(x))
     temp[0:pca_p + 1] = 0.  # this is to NOT penalize intercept beta later
     return temp
 
 
-
 ##################################################################
 ###################### LM AG numba version  ######################
 ##################################################################
 @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def _update_smooth_grad_convex_LM(N, X, beta_md, y):
     '''
     Update the gradient of the smooth convex objective component.
@@ -1080,19 +2397,20 @@
         L = _np.linalg.norm(_np.array([L_convex, 1. / (a - 1)]), ord=_np.infty)
         opt_beta = .99 / L
         while ((not converged) or (k < 3)) and k <= maxit:
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
-            else:  # restarting
+            else:  # restartings
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -1116,16 +2434,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -1304,16 +2623,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2. / (
                     1. + (1. + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1. - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -1337,16 +2657,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1. + (1. + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1. - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -1463,15 +2784,14 @@
             a=a,
             gamma=gamma,
             add_intercept_column=False)[1]
         beta_mat[j + 1, :] = _new_beta
     return beta_mat[1:, :]
 
 
-
 ##################################################################
 ########### LM AG SNP version using bed-reader ###################
 ##################################################################
 # @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def _SNP_update_smooth_grad_convex_LM(N, SNP_ind, bed, beta_md, y,
                                       outcome_iid):
     '''
@@ -1597,15 +2917,15 @@
                                return_indices=True)[1]]
         _y -= _np.mean(_y)
         for j in SNP_ind:
             _X = bed.read(_np.s_[:, j], dtype=_np.float64).flatten()
             _X = _X[gene_ind]  # get gene iid also in outcome iid
             _X -= _np.mean(_X)
             _[j] = _X @ _y / N
-        beta = _  #_np.sign(_)
+        beta = _  # _np.sign(_)
         beta = _np.hstack((_np.array([0]), beta))
     else:
         beta = beta_0
     # passing other parameters
     smooth_grad = _np.ones(p + 1)
     beta_ag = beta.copy()
     beta_md = beta.copy()
@@ -1624,16 +2944,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -1660,16 +2981,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -1732,15 +3054,15 @@
                            return_indices=True)[1]]
     _y -= _np.mean(_y)
     for j in SNP_ind:
         _X = bed.read(_np.s_[:, j], dtype=_np.float64).flatten()
         _X = _X[gene_ind]  # get gene iid also in outcome iid
         _X -= _np.mean(_X)
         _[j] = _X @ _y / N
-    beta = _  #_np.sign(_)
+    beta = _  # _np.sign(_)
     beta = _np.hstack((_np.array([0]), beta)).reshape(1, -1)
 
     beta_mat = _np.zeros((len(lambda_) + 1, p + 1))
     beta_mat = _np.repeat(beta, len(lambda_) + 1, axis=0)
     for j in range(len(lambda_)):
         beta_mat[j + 1, :] = SNP_UAG_LM_SCAD_MCP(bed_file=bed_file,
                                                  bim_file=bim_file,
@@ -1755,15 +3077,14 @@
                                                  penalty=penalty,
                                                  outcome_iid=outcome_iid,
                                                  a=a,
                                                  gamma=gamma)[1]
     return beta_mat[1:, :]
 
 
-
 ##################################################################
 ######### LM AG SNP PCA version using bed-reader #################
 ##################################################################
 # @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def _SNP_update_smooth_grad_convex_LM_PCA(N, SNP_ind, bed, beta_md, y,
                                           outcome_iid, pca_p, pca):
     '''
@@ -1898,15 +3219,15 @@
                                return_indices=True)[1]]
         _y -= _np.mean(_y)
         for j in SNP_ind:
             _X = bed.read(_np.s_[:, j], dtype=_np.float64).flatten()
             _X = _X[gene_ind]  # get gene iid also in outcome iid
             _X -= _np.mean(_X)
             _[j] = _X @ _y / N / _np.var(_X)
-        beta = _  #_np.sign(_)
+        beta = _  # _np.sign(_)
         _pca = _y @ pca[gene_ind, :] / N
         beta = _np.hstack((_np.array([_np.mean(_y)]), _pca, beta))
     else:
         beta = beta_0
     # passing other parameters
     smooth_grad = _np.ones(p + 1 + pca_p)
     beta_ag = beta.copy()
@@ -1926,16 +3247,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -1966,16 +3288,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -2044,15 +3367,15 @@
                            return_indices=True)[1]]
     _y -= _np.mean(_y)
     for j in SNP_ind:
         _X = bed.read(_np.s_[:, j], dtype=_np.float64).flatten()
         _X = _X[gene_ind]  # get gene iid also in outcome iid
         _X -= _np.mean(_X)
         _[j] = _X @ _y / N / _np.var(_X)
-    beta = _  #_np.sign(_)
+    beta = _  # _np.sign(_)
     _pca = _y @ pca[gene_ind, :] / N
     beta = _np.hstack((_np.array([_np.mean(_y)]), _pca, beta)).reshape(1, -1)
     beta_mat = _np.repeat(beta, len(lambda_) + 1, axis=0)
     for j in range(len(lambda_)):
         beta_mat[j + 1, :] = SNP_UAG_LM_SCAD_MCP_PCA(bed_file=bed_file,
                                                      bim_file=bim_file,
                                                      fam_file=fam_file,
@@ -2066,18 +3389,21 @@
                                                      _lambda=lambda_[j],
                                                      penalty=penalty,
                                                      outcome_iid=outcome_iid,
                                                      a=a,
                                                      gamma=gamma)[1]
     return beta_mat[1:, :]
 
+
 ###################################################################################
 ########### LM AG SNP version using bed-reader, multiprocess ######################
 ###################################################################################
 # @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
+
+
 def _SNP_update_smooth_grad_convex_LM_parallel(N, SNP_ind, bed, beta_md, y,
                                                outcome_iid, core_num, multp):
     '''
     Update the gradient of the smooth convex objective component.
     '''
     p = len(list(bed.sid))
     gene_iid = _np.array(list(bed.iid))
@@ -2280,15 +3606,15 @@
         _splited_array = [
             __array for __array in _splited_array if __array.size != 0
         ]
         with _mp.Pool(core_num) as pl:
             _XTy = pl.map(__parallel_assign, _splited_array)
         _XTy = _np.hstack(_XTy)
         beta = _np.zeros(p + 1)
-        beta[SNP_ind + 1] = _  #_np.sign(_XTy)
+        beta[SNP_ind + 1] = _  # _np.sign(_XTy)
     else:
         beta = beta_0
     # passing other parameters
     smooth_grad = _np.ones(p + 1)
     beta_ag = beta.copy()
     beta_md = beta.copy()
     k = 0
@@ -2306,16 +3632,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -2344,16 +3671,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -2429,15 +3757,14 @@
         import numpy as _np
         _X = bed.read(_np.s_[:, _ind],
                       dtype=_np.float64).flatten().reshape(-1, len(_ind))
         _X = _X[gene_ind, :]  # get gene iid also in outcome iid
         _X -= _np.mean(_X, 0).reshape(1, -1)
         return _y @ _X / N
 
-
 #         k = 0
 #         __ = _np.zeros(len(_ind))
 #         for j in _ind:
 #             _X = bed.read(_np.s_[:, j], dtype=_np.float64).flatten()
 #             _X = _X[gene_ind]  # get gene iid also in outcome iid
 #             _X -= _np.mean(_X)
 #             __[k] = _X @ _y / N
@@ -2450,15 +3777,15 @@
     _splited_array = [
         __array for __array in _splited_array if __array.size != 0
     ]
     with _mp.Pool(core_num) as pl:
         _XTy = pl.map(__parallel_assign, _splited_array)
     _XTy = _np.hstack(_XTy)
     beta = _np.zeros(p + 1)
-    beta[SNP_ind + 1] = _XTy  #_np.sign(_XTy)
+    beta[SNP_ind + 1] = _XTy  # _np.sign(_XTy)
     beta = beta.reshape(1, -1)
 
     beta_mat = _np.zeros((len(lambda_) + 1, p + 1))
     beta_mat = _np.repeat(beta, len(lambda_) + 1, axis=0)
     for j in range(len(lambda_)):
         beta_mat[j + 1, :] = SNP_UAG_LM_SCAD_MCP_parallel(
             bed_file=bed_file,
@@ -2476,15 +3803,14 @@
             a=a,
             gamma=gamma,
             core_num=core_num,
             multp=multp)[1]
     return beta_mat[1:, :]
 
 
-
 ##################################################################
 ################### logistic AG numba version  ###################
 ##################################################################
 @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def _update_smooth_grad_convex_logistic(N, X, beta_md, y):
     '''
     Update the gradient of the smooth convex objective component.
@@ -2615,16 +3941,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -2648,16 +3975,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -2837,16 +4165,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2. / (
                     1. + (1. + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1. - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -2870,16 +4199,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1. + (1. + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1. - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -2996,15 +4326,14 @@
             a=a,
             gamma=gamma,
             add_intercept_column=False)[1]
         beta_mat[j + 1, :] = _new_beta
     return beta_mat[1:, :]
 
 
-
 ############################################################################
 ############# logistic SNP version with bed-reader #########################
 ############################################################################
 # @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def _SNP_update_smooth_grad_convex_logistic(N, SNP_ind, bed, beta_md, y,
                                             outcome_iid):
     '''
@@ -3159,16 +4488,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -3195,16 +4525,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -3268,15 +4599,15 @@
     _y = _y.astype(dtype=_np.float64)
     _y -= _np.mean(_y)
     for j in SNP_ind:
         _X = bed.read(_np.s_[:, j], dtype=_np.float64).flatten()
         _X = _X[gene_ind]  # get gene iid also in outcome iid
         _X -= _np.mean(_X)
         _[j] = _X @ _y / N
-    beta = _  #_np.sign(_)
+    beta = _  # _np.sign(_)
     beta = _np.hstack((_np.array([0]), beta)).reshape(1, -1)
 
     beta_mat = _np.zeros((len(lambda_) + 1, p + 1))
     beta_mat = _np.repeat(beta, len(lambda_) + 1, axis=0)
     for j in range(len(lambda_)):
         beta_mat[j + 1, :] = SNP_UAG_logistic_SCAD_MCP(bed_file=bed_file,
                                                        bim_file=bim_file,
@@ -3291,15 +4622,14 @@
                                                        penalty=penalty,
                                                        outcome_iid=outcome_iid,
                                                        a=a,
                                                        gamma=gamma)[1]
     return beta_mat[1:, :]
 
 
-
 ############################################################################
 ########### logistic SNP PCA version with bed-reader #######################
 ############################################################################
 # @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
 def _SNP_update_smooth_grad_convex_logistic_PCA(N, SNP_ind, bed, beta_md, y,
                                                 outcome_iid, pca_p, pca):
     '''
@@ -3437,15 +4767,15 @@
         _y = _y.astype(dtype=_np.float64)
         _y -= _np.mean(_y)
         for j in SNP_ind:
             _X = bed.read(_np.s_[:, j], dtype=_np.float64).flatten()
             _X = _X[gene_ind]  # get gene iid also in outcome iid
             _X -= _np.mean(_X)
             _[j] = _X @ _y / N / _np.var(_X)
-        beta = _  #_np.sign(_)
+        beta = _  # _np.sign(_)
         _pca = _y @ pca[gene_ind, :] / N / _np.var(pca[gene_ind, :], 0)
         beta = _np.hstack((_np.array([0.]), _pca, beta))
 #         beta = _np.sign(beta)
     else:
         beta = beta_0
     # passing other parameters
     smooth_grad = _np.ones(p + 1 + pca_p)
@@ -3466,16 +4796,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -3506,16 +4837,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -3585,15 +4917,15 @@
     _y = _y.astype(dtype=_np.float64)
     _y -= _np.mean(_y)
     for j in SNP_ind:
         _X = bed.read(_np.s_[:, j], dtype=_np.float64).flatten()
         _X = _X[gene_ind]  # get gene iid also in outcome iid
         _X -= _np.mean(_X)
         _[j] = _X @ _y / N / _np.var(_X)
-    beta = _  #_np.sign(_)
+    beta = _  # _np.sign(_)
     _pca = _y @ pca[gene_ind, :] / N / _np.var(pca[gene_ind, :], 0)
     beta = _np.hstack((_np.array([0.]), _pca, beta)).reshape(1, -1)
     #     beta = _np.sign(beta)
     beta_mat = _np.repeat(beta, len(lambda_) + 1, axis=0)
     for j in range(len(lambda_)):
         beta_mat[j + 1, :] = SNP_UAG_logistic_SCAD_MCP_PCA(
             bed_file=bed_file,
@@ -3609,18 +4941,21 @@
             _lambda=lambda_[j],
             penalty=penalty,
             outcome_iid=outcome_iid,
             a=a,
             gamma=gamma)[1]
     return beta_mat[1:, :]
 
+
 ##############################################################################################
 ################ logsitic AG SNP bed-reader version with multiprocess ########################
 ##############################################################################################
 # @_jit(nopython=True, cache=True, parallel=True, fastmath=True, nogil=True)
+
+
 def _SNP_update_smooth_grad_convex_logistic_parallel(N, SNP_ind, bed, beta_md,
                                                      y, outcome_iid, core_num,
                                                      multp):
     '''
     Update the gradient of the smooth convex objective component.
     '''
     p = bed.sid_count
@@ -3850,16 +5185,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -3888,16 +5224,17 @@
             k += 1
             if old_speed_norm > speed_norm and k - restart_k >= 3:  # in this case, restart
                 opt_alpha = 1.  # restarting
                 restart_k = k  # restarting
             else:  # restarting
                 opt_alpha = 2 / (
                     1 + (1 + 4. / opt_alpha**2)**.5
-                )  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
-            opt_lambda = opt_beta / opt_alpha  #parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+                )  # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            # parameter settings based on minimizing Ghadimi and Lan's rate of convergence error upper bound
+            opt_lambda = opt_beta / opt_alpha
             beta_md_old = beta_md.copy()  # restarting
             beta_md = (1 - opt_alpha) * beta_ag + opt_alpha * beta
             old_speed_norm = speed_norm  # restarting
             speed_norm = _np.linalg.norm(beta_md - beta_md_old,
                                          ord=2)  # restarting
             converged = (_np.linalg.norm(beta_md - beta_md_old, ord=_np.infty)
                          < tol)
@@ -3995,15 +5332,15 @@
     _splited_array = [
         __array for __array in _splited_array if __array.size != 0
     ]
     with _mp.Pool(core_num) as pl:
         _XTy = pl.map(__parallel_assign, _splited_array)
     _XTy = _np.hstack(_XTy)
     beta = _np.zeros(p + 1)
-    beta[SNP_ind + 1] = _XTy  #_np.sign(_XTy)
+    beta[SNP_ind + 1] = _XTy  # _np.sign(_XTy)
     beta = beta.reshape(1, -1)
 
     beta_mat = _np.zeros((len(lambda_) + 1, p + 1))
     beta_mat = _np.repeat(beta, len(lambda_) + 1, axis=0)
     for j in range(len(lambda_)):
         beta_mat[j + 1, :] = SNP_UAG_logistic_SCAD_MCP_parallel(
             bed_file=bed_file,
```

### Comparing `fastHDMI-1.2.9/src/fastHDMI.egg-info/PKG-INFO` & `fastHDMI-1.23.1/src/fastHDMI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fastHDMI
-Version: 1.2.9
-Summary: Use fast FFT-based mutual information and accelerated gradient method to filter out and optimize nonconvex sparse learning problems on large CSV files or large genetic bed/bim/fam files. Multiprocessing is now available.
+Version: 1.23.1
+Summary: Use FFT-based mutual information and accelerated gradient method to screen variables and optimize nonconvex sparse learning problems on large CSV files or large genetic bed/bim/fam files. Multiprocessing is now available.
 Author-email: Kai Yang <kai.yang2@mail.mcgill.ca>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -670,34 +670,42 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# fastHDMI -- fast High-Dimensional Mutual Information
+# fastHDMI -- fast High-Dimensional Mutual Information estimation
+## Kai Yang
+## <kai.yang2@mail.mcgill.ca>
 
-This packages uses mutual information and accelerated gradient method to screen for important variables from (potentially very) high-dimensional large datasets. As a feature, it can be applied on large `.csv` data in parallel in a memory-efficient manner and use FFT for KDE to estimate the mutual information extremely fast. It also features screening for SNPs and optimize the nonconvex sparse learning problem on large genetic data using plink files (`*.bed/*.bim/*.fam`). The corresponding paper by Yang et al. is coming soon...
+To be rewritten...
+
+This packages uses FFT-based mutual information screening and accelerated gradient method for important variables from (potentially very) high-dimensional large datasets. A `share_memory` option is added for multiprocess computing. As a feature, it can be applied on large `.csv` data in parallel in a memory-efficient manner and use FFT for KDE to estimate the mutual information extremely fast. A tqdm progress bar is now added to be more useful on cloud computing platforms. `verbose` option can take values of `0,1,2`, with `2` being most verbal; `1` being only show progress bar, and `0` being not verbal at all. The corresponding paper by Yang et al. is coming soon...
 
 The available functions are:
-- `continuous_filter_plink` caculates the mutual information between a continuous outcome and a bialletic SNP using FFT. Missing data is acceptable and will be removed. The arguments are:
+- `continuous_screening_plink` caculates the mutual information between a continuous outcome and a bialletic SNP using FFT. Missing data in the input variables is acceptable and will be removed per bivariate calculation. The arguments are:
   * `bed_file`, `bim_file`, `fam_file` are the location of the plink1 files;
   * `outcome`, `outcome_iid` are the outcome values and the iids for the outcome. For genetic data, it is usual that the order of SNP iid and the outcome iid don't match. While SNP iid can be obtained from the plink1 files, outcome iid here is to be declared separately. `outcome_iid` should be a list of strings or a one-dimensional numpy string array.
-  * `a_min`, `a_max` are the minimum and maximum of the continous outcome used to evaluate the support; `N=500` is the default values for grid size for FFT.
+  * `N=500` is the default values for grid size for FFT.
 
-- `binary_filter_plink` works similarly, execpt that `a_min, a_max, N` are not available obviously.
+- `binary_screening_plink` works similarly. 
 
-- `continuous_filter_plink_parallel` and `binary_filter_plink_parallel` are the multiprocessing version of the above two functions, with `core_num` can be used to declare the number of cores to be used for multiprocessing.
+- `continuous_screening_plink_parallel` and `binary_screening_plink_parallel` are the multiprocessing version of the above two functions, with `core_num` can be used to declare the number of cores to be used for multiprocessing.
 
-- `MI_bivariate_continuous` and `MI_binary_continuous` are to calculate mutual information between two continuous variables and binary and continuous variables, respectively.
+- `MI_continuous_continuous` and `MI_binary_continuous` are to calculate mutual information between two continuous variables and binary and continuous variables, respectively. `MI_binary_012` and `MI_012_012` are `jit` complied functions -- the later can be used for clumping for very large genetic datasets.
 
-- `binary_filter_csv`, `continuous_filter_csv`, `binary_filter_csv_parallel`, and `continuous_filter_csv_parallel` are to work on large CSV files directly in a memory efficient manner. **Note that it is assumed the left first column should be the outcome;** if not, use `_usecols` to set the first element to be the outcome column label.
+- `binary_screening_csv`, `continuous_screening_csv`, `binary_screening_csv_parallel`, and `continuous_screening_csv_parallel` are to work on large CSV files directly in a memory efficient manner. **Note that it is assumed the left first column should be the outcome;** if not, use `_usecols` to set the first element to be the outcome column label.
   * `_usecols` is a list of column labels to be used, **the first element should be the outcome. Returned mutual information calculation results match `_usecols`.**
-  * `Pearson_filter_csv_parallel` calculate Pearson's correlation between only the outcome and the covariates in similiar manner -- since `pandas.DataFrame.corr` calculate pairwise Pearson's correlation for the dataframe.
+  * `Pearson_screening_csv_parallel` calculate Pearson's correlation between only the outcome and the covariates in similiar manner -- since `pandas.DataFrame.corr` calculate pairwise Pearson's correlation for the entire dataframe.
+  * `csv_engine` can use `dask` for low memory situations, or `pandas`'s `read_csv` `engine`s, or `fastparquet` engine for a created `parquet` file for faster speed. If `fastparquet` is chosen, declare `parquet_file` as the filepath to the parquet file; if `dask` is chosen to read very large CSV, it might need to specify a larger [`sample`](https://docs.dask.org/en/stable/generated/dask.dataframe.read_csv.html).
+
+- `continuous_skMIscreening_csv_parallel` uses the MI calculation from [`sklearn.feature_selection.mutual_info_regression`](https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.mutual_info_regression.html) to carry out the screening process instead.
 
+- `clump_plink_parallel` and `clump_continuous_csv_parallel` carry out mutual information based clumping in parallel at a very fast speed.
 
 - `UAG_LM_SCAD_MCP`, `UAG_logistic_SCAD_MCP`: these functions find a local minizer for the SCAD/MCP penalized linear models/logistic models. The arguments are:
   * `design_matrix`: the design matrix input, should be a two-dimensional numpy array;
   * `outcome`: the outcome, should be one dimensional numpy array, continuous for linear model, binary for logistic model;
   * `beta_0`: starting value; optional, if not declared, it will be calculated based on the Gauss-Markov theory estimators of $\beta$;
   * `tol`: tolerance parameter; the tolerance parameter is set to be the uniform norm of two iterations;
   * `maxit`: maximum number of iteratios allowed;
@@ -705,10 +713,10 @@
   * `penalty`: could be `"SCAD"` or `"MCP"`;
   * `a=3.7`, `gamma=2`: `a` for SCAD and `gamma` for MCP; it is recommended for `a` to be set as $3.7$;
   * `L_convex`: the L-smoothness constant for the convex component, if not declared, it will be calculated by itself
   * `add_intercept_column`: boolean, should the fucntion add an intercept column?
 
 - `solution_path_LM`, `solution_path_logistic`: calculate the solution path for linear/logistic models; the only difference from above is that `lambda_` is now a one-dimensional numpy array for the values of $\lambda$ to be used.
 
-- `UAG_LM_SCAD_MCP_strongrule`, `UAG_logistic_SCAD_MCP_strongrule` work just like `UAG_LM_SCAD_MCP`, `UAG_logistic_SCAD_MCP` -- except they use strong rule to filter out many covariates before carrying out the optimization step. Same for `solution_path_LM_strongrule` and `solution_path_logistic_strongrule`. Strong rule increases the computational speed dramatically.
+- `UAG_LM_SCAD_MCP_strongrule`, `UAG_logistic_SCAD_MCP_strongrule` work just like `UAG_LM_SCAD_MCP`, `UAG_logistic_SCAD_MCP` -- except they use strong rule to screening out many covariates before carrying out the optimization step. Same for `solution_path_LM_strongrule` and `solution_path_logistic_strongrule`. Strong rule increases the computational speed dramatically.
 
 - `SNP_UAG_LM_SCAD_MCP` and `SNP_UAG_logistic_SCAD_MCP` work similar to `UAG_LM_SCAD_MCP` and `UAG_logistic_SCAD_MCP`; and `SNP_solution_path_LM` and `SNP_solution_path_logistic` work similar to `solution_path_LM`, `solution_path_logistic` -- except that it takes plink1 files so it will be more memory-efficient. Since PCA adjustment is usually used to adjust for population structure, PCA can be given for `pca` as a 2-d array -- each column should be one principal component. The pca version is `SNP_UAG_LM_SCAD_MCP_PCA` and `SNP_UAG_logistic_SCAD_MCP_PCA`.
```

