# Comparing `tmp/ggcorrplot-0.0.1.tar.gz` & `tmp/ggcorrplot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ggcorrplot-0.0.1.tar", last modified: Sun Apr 16 13:01:40 2023, max compression
+gzip compressed data, was "ggcorrplot-0.0.2.tar", last modified: Tue Apr 18 00:15:47 2023, max compression
```

## Comparing `ggcorrplot-0.0.1.tar` & `ggcorrplot-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 13:01:40.629737 ggcorrplot-0.0.1/
--rw-rw-rw-   0        0        0      607 2023-04-16 13:01:40.629737 ggcorrplot-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 13:01:40.601668 ggcorrplot-0.0.1/ggcorrplot/
--rw-rw-rw-   0        0        0       92 2023-04-16 12:46:43.000000 ggcorrplot-0.0.1/ggcorrplot/__init__.py
--rw-rw-rw-   0        0        0     6992 2023-04-16 12:59:05.000000 ggcorrplot-0.0.1/ggcorrplot/ggcorrplot.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:01:40.627463 ggcorrplot-0.0.1/ggcorrplot.egg-info/
--rw-rw-rw-   0        0        0      607 2023-04-16 13:01:40.000000 ggcorrplot-0.0.1/ggcorrplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-04-16 13:01:40.000000 ggcorrplot-0.0.1/ggcorrplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 13:01:40.000000 ggcorrplot-0.0.1/ggcorrplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-04-16 13:01:40.000000 ggcorrplot-0.0.1/ggcorrplot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-16 13:01:40.000000 ggcorrplot-0.0.1/ggcorrplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 13:01:40.630732 ggcorrplot-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1127 2023-04-16 13:01:10.000000 ggcorrplot-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 00:15:47.583216 ggcorrplot-0.0.2/
+-rw-rw-rw-   0        0        0       20 2023-04-16 13:18:57.000000 ggcorrplot-0.0.2/.gitignore
+-rw-rw-rw-   0        0        0      713 2023-04-18 00:15:47.582182 ggcorrplot-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2023-04-18 00:12:08.000000 ggcorrplot-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 00:15:47.552122 ggcorrplot-0.0.2/dist/
+-rw-rw-rw-   0        0        0     3731 2023-04-16 13:01:40.000000 ggcorrplot-0.0.2/dist/ggcorrplot-0.0.1-py3-none-any.whl
+-rw-rw-rw-   0        0        0     3508 2023-04-16 13:01:40.000000 ggcorrplot-0.0.2/dist/ggcorrplot-0.0.1.tar.gz
+drwxrwxrwx   0        0        0        0 2023-04-18 00:15:47.553171 ggcorrplot-0.0.2/ggcorrplot/
+-rw-rw-rw-   0        0        0      137 2023-04-18 00:02:44.000000 ggcorrplot-0.0.2/ggcorrplot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 00:15:47.581007 ggcorrplot-0.0.2/ggcorrplot/__pycache__/
+-rw-rw-rw-   0        0        0      232 2023-04-16 12:46:52.000000 ggcorrplot-0.0.2/ggcorrplot/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5383 2023-04-17 23:47:14.000000 ggcorrplot-0.0.2/ggcorrplot/__pycache__/ggcorrplot.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7705 2023-04-18 00:14:36.000000 ggcorrplot-0.0.2/ggcorrplot/ggcorrplot.py
+drwxrwxrwx   0        0        0        0 2023-04-18 00:15:47.578740 ggcorrplot-0.0.2/ggcorrplot.egg-info/
+-rw-rw-rw-   0        0        0      713 2023-04-18 00:15:47.000000 ggcorrplot-0.0.2/ggcorrplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-04-18 00:15:47.000000 ggcorrplot-0.0.2/ggcorrplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 00:15:47.000000 ggcorrplot-0.0.2/ggcorrplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-04-18 00:15:47.000000 ggcorrplot-0.0.2/ggcorrplot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-18 00:15:47.000000 ggcorrplot-0.0.2/ggcorrplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   484026 2023-04-18 00:13:02.000000 ggcorrplot-0.0.2/ggcorrplot.ipynb
+-rw-rw-rw-   0        0        0       42 2023-04-18 00:15:47.583216 ggcorrplot-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1233 2023-04-17 23:57:38.000000 ggcorrplot-0.0.2/setup.py
```

### Comparing `ggcorrplot-0.0.1/PKG-INFO` & `ggcorrplot-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: ggcorrplot
-Version: 0.0.1
-Summary: Visualization of a Correlation Matrix using 'plotnine'
+Version: 0.0.2
+Summary: Visualization of a Correlation Matrix using plotnine
 Home-page: UNKNOWN
 Author: Duvérier DJIFACK ZEBAZE
 Author-email: duverierdjifack@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 
-The 'ggcorrplot' package can be used to visualize easily a
-    correlation matrix using 'plotnine'. It provides a function for computing a matrix of
-    correlation p-values.
+The ggcorrplot package can be used to visualize easily a correlation matrix using plotnine. It provides a solution for reordering the correlation matrix and displays the significance level on the correlogram. It includes also a function for computing a matrix of correlation p-values.
```

### Comparing `ggcorrplot-0.0.1/ggcorrplot/ggcorrplot.py` & `ggcorrplot-0.0.2/ggcorrplot/ggcorrplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,87 +1,96 @@
-
+# -*- coding: utf-8 -*-
 
 import numpy as np
 import pandas as pd
 import plotnine as pn
 import scipy.stats as st
 import plydata as ply
 from scipy.cluster import hierarchy
+from scipy.spatial.distance import squareform
+
+def get_melt(X):
+    if not isinstance(X,pd.DataFrame):
+        raise ValueError("Error : 'X' must be a DataFrame")
+    return X.stack().rename_axis(('Var1', 'Var2')).reset_index(name='value')
 
 def hc_cormat_order(cormat, method='complete'):
+    if not isinstance(cormat,pd.DataFrame):
+        raise ValueError("Error : 'cormat' must be a DataFrame.")
     X = (1-cormat)/2
-    Z = hierarchy.linkage(X,method=method, metric="euclidean")
+    Z = hierarchy.linkage(squareform(X),method=method, metric="euclidean")
     order = hierarchy.leaves_list(Z)
     return dict({"order":order,"height":Z[:,2],"method":method,
                 "merge":Z[:,:2],"n_obs":Z[:,3],"data":cormat})
 
-
 def match_arg(x, lst):
     return [el for el in lst if x in el][0]
 
 def no_panel():
     return pn.theme(
         axis_title_x=pn.element_blank(),
         axis_title_y=pn.element_blank()
     )
 
 def remove_diag(cormat):
     if cormat is None:
         return cormat
     if not isinstance(cormat,pd.DataFrame):
-        raise ValueError("Error : Need a DataFrame.")
+        raise ValueError("Error : 'cormat' must be a DataFrame.")
     np.fill_diagonal(cormat.values, np.nan)
     return cormat
 
 def get_upper_tri(cormat,show_diag=False):
     if cormat is None:
         return cormat
     if not isinstance(cormat,pd.DataFrame):
-        raise ValueError("Error : Need a DataFrame.")
+        raise ValueError("Error : 'cormat' must be a DataFrame.")
     cormat = pd.DataFrame(np.triu(cormat),index=cormat.index,columns=cormat.columns)
     cormat.values[np.tril_indices(cormat.shape[0], -1)] = np.nan
     if not show_diag:
         np.fill_diagonal(cormat.values,np.nan)
     return cormat
 
 def get_lower_tri(cormat,show_diag=False):
     if cormat is None:
         return cormat
     if not isinstance(cormat,pd.DataFrame):
-        raise ValueError("Error : Need a DataFrame.")
+        raise ValueError("Error : 'cormat' must be a DataFrame.")
     cormat = pd.DataFrame(np.tril(cormat),index=cormat.index,columns=cormat.columns)
     cormat.values[np.triu_indices(cormat.shape[0], 1)] = np.nan
     if not show_diag:
         np.fill_diagonal(cormat.values,np.nan)
     return cormat
 
 def cor_pmat(x,**kwargs):
     if not isinstance(x,pd.DataFrame):
-        raise ValueError("Error : Need a DataFrame.")
+        raise ValueError("Error : 'x' must be a DataFrame.")
     y = np.array(x)
     n = y.shape[1]
     p_mat = np.zeros((n,n))
     np.fill_diagonal(p_mat,0)
     for i in np.arange(0,n-1):
         for j in np.arange(i+1,n):
             tmps = st.pearsonr(y[:,i],y[:,j],**kwargs)
             p_mat[i,j] = p_mat[j,i] = tmps[1]
     p_mat = pd.DataFrame(p_mat,index=x.columns,columns=x.columns)
     return p_mat
 
 def ggcorrplot(x,
                method = "square",
                type = "full",
-               ggtheme =pn.theme_minimal(),
+               ggtheme = pn.theme_minimal(),
                title = None,
                show_legend = True,
                legend_title = "Corr",
                show_diag = None,
                colors = ["blue","white","red"],
                outline_color = "gray",
+               hc_order = False,
+               hc_method = "complete",
                lab = False,
                lab_col = "black",
                lab_size = 11,
                p_mat = None,
                sig_level=0.05,
                insig = "pch",
                pch = 4,
@@ -89,33 +98,39 @@
                pch_cex = 5,
                tl_cex = 12,
                tl_col = "black",
                tl_srt = 45,
                digits = 2):
     
     if not isinstance(x,pd.DataFrame):
-        raise ValueError("Error : 'corr' must be a DataFrame.")
+        raise ValueError("Error : 'x' must be a DataFrame.")
     
     if p_mat is not None:
         if not isinstance(p_mat,pd.DataFrame):
             raise ValueError("Error : 'p_mat' must be a DataFrame.")
 
-
     type = match_arg(type, ["full","lower","upper"])
     method = match_arg(method,["square",'circle'])
     insig = match_arg(insig,["pch","blank"])
 
     if show_diag is None:
         if type == "full":
             show_diag = True
         else:
             show_diag = False
-    x.columns = pd.Categorical(x.columns,categories=x.columns)
+
     corr = x.corr().round(decimals=digits)
 
+    if hc_order:
+        ord = hc_cormat_order(corr,method=hc_method)["order"]
+        corr = corr.iloc[ord,ord]
+        if p_mat is not None:
+            p_mat = p_mat.iloc[ord,ord]
+            p_mat = p_mat.round(decimals=digits)
+
     if not show_diag:
         corr = remove_diag(corr)
         if p_mat is not None:
             p_mat = remove_diag(p_mat)
     
     # Get lower or upper triangle
     if type == "lower":
@@ -124,23 +139,23 @@
             p_mat = get_lower_tri(p_mat,show_diag)
     elif type == "upper":
         corr = get_upper_tri(corr,show_diag)
         if p_mat is not None:
             p_mat = get_upper_tri(corr,show_diag)
     
     # Melt corr and p_mat
-    corr = corr.stack().reset_index()
-    corr.columns = ['Var1','Var2','value']
-
+    corr.columns = pd.Categorical(corr.columns,categories=corr.columns)
+    corr.index = pd.Categorical(corr.columns,categories=corr.columns)
+    corr = get_melt(corr)
+    
     corr = corr >> ply.define(pvalue=np.nan)
     corr = corr >> ply.define(signif=np.nan)
 
     if p_mat is not None:
-        p_mat = p_mat.stack().reset_index()
-        p_mat.columns = ['Var1','Var2','value']
+        p_mat = get_melt(p_mat)
         corr = corr >> ply.define(coef="value")
         corr = corr >> ply.mutate(pvalue=p_mat.value)
         corr["signif"] = np.where(p_mat.value <= sig_level,1,0)
         p_mat = p_mat.query(f'value > {sig_level}')
         if insig == "blank":
             corr = corr >> ply.mutate(value="value*signif")
```

### Comparing `ggcorrplot-0.0.1/ggcorrplot.egg-info/PKG-INFO` & `ggcorrplot-0.0.2/ggcorrplot.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: ggcorrplot
-Version: 0.0.1
-Summary: Visualization of a Correlation Matrix using 'plotnine'
+Version: 0.0.2
+Summary: Visualization of a Correlation Matrix using plotnine
 Home-page: UNKNOWN
 Author: Duvérier DJIFACK ZEBAZE
 Author-email: duverierdjifack@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 
-The 'ggcorrplot' package can be used to visualize easily a
-    correlation matrix using 'plotnine'. It provides a function for computing a matrix of
-    correlation p-values.
+The ggcorrplot package can be used to visualize easily a correlation matrix using plotnine. It provides a solution for reordering the correlation matrix and displays the significance level on the correlogram. It includes also a function for computing a matrix of correlation p-values.
```

### Comparing `ggcorrplot-0.0.1/setup.py` & `ggcorrplot-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
-DESCRIPTION = "Visualization of a Correlation Matrix using 'plotnine'"
-LONG_DESCRIPTION = """The 'ggcorrplot' package can be used to visualize easily a
-    correlation matrix using 'plotnine'. It provides a function for computing a matrix of
-    correlation p-values."""
+VERSION = '0.0.2' 
+DESCRIPTION = "Visualization of a Correlation Matrix using plotnine"
+LONG_DESCRIPTION = """The ggcorrplot package can be used to visualize easily a correlation matrix using plotnine. It provides a solution for reordering the correlation matrix and displays the significance level on the correlogram. It includes also a function for computing a matrix of correlation p-values."""
 
 # Setting up
 setup(
         name="ggcorrplot", 
         version=VERSION,
         author="Duvérier DJIFACK ZEBAZE",
         author_email="duverierdjifack@gmail.com",
```

