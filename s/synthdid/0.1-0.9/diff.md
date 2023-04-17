# Comparing `tmp/synthdid-0.1.tar.gz` & `tmp/synthdid-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\synthdid-0.1.tar", last modified: Mon Apr 17 17:07:55 2023, max compression
+gzip compressed data, was "dist\synthdid-0.9.tar", last modified: Tue Apr 18 01:24:56 2023, max compression
```

## Comparing `synthdid-0.1.tar` & `synthdid-0.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 17:07:55.520418 synthdid-0.1/
--rw-rw-rw-   0        0        0      430 2023-04-17 17:07:55.519418 synthdid-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-17 17:07:55.520418 synthdid-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1604 2023-04-17 17:07:24.000000 synthdid-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 17:07:55.511420 synthdid-0.1/synthdid/
--rw-rw-rw-   0        0        0        0 2023-04-17 16:48:20.000000 synthdid-0.1/synthdid/__init__.py
--rw-rw-rw-   0        0        0     1701 2023-04-17 16:31:07.000000 synthdid-0.1/synthdid/get_data.py
--rw-rw-rw-   0        0        0     3520 2023-04-17 16:48:20.000000 synthdid-0.1/synthdid/placebo_simulations.py
--rw-rw-rw-   0        0        0     6064 2023-04-17 16:48:20.000000 synthdid-0.1/synthdid/plots.py
--rw-rw-rw-   0        0        0     9247 2023-04-17 16:54:35.000000 synthdid-0.1/synthdid/sdid.py
--rw-rw-rw-   0        0        0     5180 2023-04-17 16:48:20.000000 synthdid-0.1/synthdid/solver.py
--rw-rw-rw-   0        0        0      649 2023-04-17 16:57:31.000000 synthdid-0.1/synthdid/synthdid.py
--rw-rw-rw-   0        0        0     3455 2023-04-17 16:55:39.000000 synthdid-0.1/synthdid/utils.py
--rw-rw-rw-   0        0        0     5043 2023-04-17 16:51:44.000000 synthdid-0.1/synthdid/vcov.py
-drwxrwxrwx   0        0        0        0 2023-04-17 17:07:55.519418 synthdid-0.1/synthdid.egg-info/
--rw-rw-rw-   0        0        0      430 2023-04-17 17:07:55.000000 synthdid-0.1/synthdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-04-17 17:07:55.000000 synthdid-0.1/synthdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 17:07:55.000000 synthdid-0.1/synthdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      623 2023-04-17 17:07:55.000000 synthdid-0.1/synthdid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 17:07:55.000000 synthdid-0.1/synthdid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 01:24:56.255995 synthdid-0.9/
+-rw-rw-rw-   0        0        0      430 2023-04-18 01:24:56.255995 synthdid-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-18 01:24:56.255995 synthdid-0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1604 2023-04-18 00:46:12.000000 synthdid-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 01:24:56.245996 synthdid-0.9/synthdid/
+-rw-rw-rw-   0        0        0        0 2023-04-17 22:50:30.000000 synthdid-0.9/synthdid/__init__.py
+-rw-rw-rw-   0        0        0     1701 2023-04-17 22:50:30.000000 synthdid-0.9/synthdid/get_data.py
+-rw-rw-rw-   0        0        0     3520 2023-04-17 22:50:30.000000 synthdid-0.9/synthdid/placebo_simulations.py
+-rw-rw-rw-   0        0        0     6064 2023-04-17 22:50:30.000000 synthdid-0.9/synthdid/plots.py
+-rw-rw-rw-   0        0        0     9303 2023-04-17 22:50:30.000000 synthdid-0.9/synthdid/sdid.py
+-rw-rw-rw-   0        0        0     5439 2023-04-17 22:50:30.000000 synthdid-0.9/synthdid/solver.py
+-rw-rw-rw-   0        0        0      273 2023-04-18 01:20:15.000000 synthdid-0.9/synthdid/summary.py
+-rw-rw-rw-   0        0        0      774 2023-04-18 01:20:51.000000 synthdid-0.9/synthdid/synthdid.py
+-rw-rw-rw-   0        0        0     3610 2023-04-17 22:50:30.000000 synthdid-0.9/synthdid/utils.py
+-rw-rw-rw-   0        0        0     5043 2023-04-17 22:50:30.000000 synthdid-0.9/synthdid/vcov.py
+drwxrwxrwx   0        0        0        0 2023-04-18 01:24:56.254995 synthdid-0.9/synthdid.egg-info/
+-rw-rw-rw-   0        0        0      430 2023-04-18 01:24:56.000000 synthdid-0.9/synthdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-04-18 01:24:56.000000 synthdid-0.9/synthdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 01:24:56.000000 synthdid-0.9/synthdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      623 2023-04-18 01:24:56.000000 synthdid-0.9/synthdid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 01:24:56.000000 synthdid-0.9/synthdid.egg-info/top_level.txt
```

### Comparing `synthdid-0.1/setup.py` & `synthdid-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         "six==1.16.0",
         "statsmodels==0.13.5",
         "toml==0.10.0",
         "zipp==3.15.0",
     ],
     name="synthdid",
     author="D2CML",
-    version="0.1",
+    version="0.9",
     packages=find_packages(),
     keywords="causal-inference",
     url="https://github.com/d2cml-ai/synthdid.py",
     license="MIT",
     description="Synthdid",
     classifiers=[
         "Intended Audience :: Developers",
```

### Comparing `synthdid-0.1/synthdid/get_data.py` & `synthdid-0.9/synthdid/get_data.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.1/synthdid/placebo_simulations.py` & `synthdid-0.9/synthdid/placebo_simulations.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.1/synthdid/plots.py` & `synthdid-0.9/synthdid/plots.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.1/synthdid/sdid.py` & `synthdid-0.9/synthdid/sdid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np, pandas as pd
-from .utils import panel_matrices, collapse_form, varianza, sparsify_function
+from .utils import panel_matrices, collapse_form, varianza, sparsify_function, projected
 from .solver import fw_step, sc_weight_fw, sc_weight_covariates
 
 
 
 # scol => unit, tcol => time, ycol=> outcome, dcol => treatment
 # data_ref: treated => tunit
 
@@ -127,15 +127,15 @@
 class SDID:
 	def fit(self,# data: pd.DataFrame, unit, time, treatment, outcome, covariates=None, 
 			cov_method="optimized", noise_level=None, eta_omega=None, eta_lambda=1e-6, zeta_omega=None, zeta_lambda=None, omega_intercept=True, lambda_intercept=True, min_decrease=None, max_iter=10000, sparsify=sparsify_function, max_iter_pre_sparsify=100, lambda_estimate=None, omega_estimate=None
 			):
 	# tdf, ttime = panel_matrices(data, unit, time, treatment, outcome, covariates)
 		tdf, ttime, covariates = self.data_ref, self.ttime, self.covariates
 		if (covariates is not None) and (cov_method == "projected"):
-			tdf = projected(tdf)
+			tdf, _, _ = projected(tdf, 'outcome', 'unit', 'time', covariates)
 		
 		T_total = 0
 		break_points = len(ttime)
 		tau_hat, tau_hat_wt = np.zeros(break_points), np.zeros(break_points)
 		N0s, T0s = [], []
 		N1s, T1s = [], []
 		beta_covariate = []
```

### Comparing `synthdid-0.1/synthdid/solver.py` & `synthdid-0.9/synthdid/solver.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 import numpy as np, pandas as pd
 
+def contract3(X, v):
+    
+    assert (len(X.shape) == 3) and (X.shape[0] == len(v))
+    out = np.zeros(X.shape[1: ])
+    
+    if len(v) == 0: return out
+    
+    for ii in range(len(v)):
+        out += v[ii] * X[ii, :, :]
+    
+    return out
+    
 def fw_step(A, b, x, eta, alpha=None):
     x = np.array(x)
     Ax = np.dot(A, x)
     half_grad = np.dot((Ax - b), A) + eta * np.transpose(x)
     i = np.argmin(half_grad)
     if alpha is not None:
         x *= (1 - alpha)
```

### Comparing `synthdid-0.1/synthdid/synthdid.py` & `synthdid-0.9/synthdid/synthdid.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 import itertools, matplotlib.pyplot as plt
 
 from synthdid.utils import panel_matrices
 from synthdid.get_data import quota
 from synthdid.sdid import SDID
 from synthdid.vcov import Variance
 from synthdid.plots import Plots
+from synthdid.summary import Summary
 
-class Synthdid(SDID, Variance, Plots):
+class Synthdid(SDID, Variance, Plots, Summary):
 	def __init__(self, data, unit="unit", time = "time", treatment="treatment", outcome="outcome", covariates = None):
 		self.data = data
 		self.unit, self.time = unit, time
 		self.treatment, self.outcome = treatment, outcome
 		self.covariates = covariates
-		self.data_ref, self.ttime = panel_matrices(data, unit, time, treatment, outcome)
+		self.data_ref, self.ttime = panel_matrices(data, unit, time, treatment, outcome, covariates=covariates)
+		# if covariates is not None:
+		# 	self.data_cov =
```

### Comparing `synthdid-0.1/synthdid/utils.py` & `synthdid-0.9/synthdid/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pandas as pd, numpy as np
 
 def panel_matrices(data: pd.DataFrame(), unit, time, treatment, outcome, covariates = None): #-> data_prep
 	if len(np.unique(data[treatment])) != 2:
 		print("Error")
 
+	data = data.reset_index()
 	data_ref = pd.DataFrame()
 	data_ref[["unit", "time", "outcome"]] = data[[unit, time, outcome]]
 	data_ref["treatment"] = data[treatment].to_numpy()
 	other = data.drop(columns=[unit, time, outcome, treatment])
 
 	unit, time, outcome, treatment = data_ref.columns
 
@@ -30,18 +31,22 @@
 	break_points = np.unique(data_ref.tyear)
 	break_points = break_points[~np.isnan(break_points)]
 
 	units = data_ref[unit]
 	num_col = data_ref.select_dtypes(np.number).columns
 	data_ref = data_ref[num_col].fillna(0)
 	data_ref[unit] = units
+	data_ref = data_ref.sort_values(["treated", "time", "unit"])
 	if covariates is not None:
-		data_ref = pd.concat([data_ref, other], axis = 1)
+		# return data
+		data_cov = data[covariates].loc[data_ref.index]
+		data_ref = pd.concat([data_ref, data_cov], axis = 1)
 		# data_ref[covariates] = data_ref[covariates].fillna(0)s
-	data_ref = data_ref.sort_values(["treated", "time", "unit"])
+		# return data_cov
+		return (data_ref, break_points)
 
 	return (data_ref, break_points)
 
 def projected(data, outcome, unit, time, covariates):
 
   k = len(covariates)
   X = np.array(data[covariates])
```

### Comparing `synthdid-0.1/synthdid/vcov.py` & `synthdid-0.9/synthdid/vcov.py`

 * *Files identical despite different names*

### Comparing `synthdid-0.1/synthdid.egg-info/requires.txt` & `synthdid-0.9/synthdid.egg-info/requires.txt`

 * *Files identical despite different names*

