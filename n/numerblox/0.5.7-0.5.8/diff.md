# Comparing `tmp/numerblox-0.5.7.tar.gz` & `tmp/numerblox-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerblox-0.5.7.tar", last modified: Mon Apr 17 15:41:31 2023, max compression
+gzip compressed data, was "numerblox-0.5.8.tar", last modified: Tue Apr 18 16:54:27 2023, max compression
```

## Comparing `numerblox-0.5.7.tar` & `numerblox-0.5.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-17 15:41:31.393349 numerblox-0.5.7/
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     4767 2023-04-05 12:06:33.000000 numerblox-0.5.7/CONTRIBUTING.md
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    11357 2023-04-05 12:06:33.000000 numerblox-0.5.7/LICENSE
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      111 2023-04-05 12:06:33.000000 numerblox-0.5.7/MANIFEST.in
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    12474 2023-04-17 15:41:31.393349 numerblox-0.5.7/PKG-INFO
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    11651 2023-04-05 12:35:32.000000 numerblox-0.5.7/README.md
-drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-17 15:41:31.389349 numerblox-0.5.7/numerblox/
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       22 2023-04-17 15:39:55.000000 numerblox-0.5.7/numerblox/__init__.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    67939 2023-04-17 15:39:55.000000 numerblox-0.5.7/numerblox/_modidx.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     4073 2023-04-05 12:06:33.000000 numerblox-0.5.7/numerblox/_nbdev.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    22382 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/download.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    70911 2023-04-17 15:39:55.000000 numerblox-0.5.7/numerblox/evaluation.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      103 2023-04-05 12:06:33.000000 numerblox-0.5.7/numerblox/index.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      947 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/key.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      333 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/misc.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    26837 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/model.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     5985 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/model_pipeline.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     6929 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/numerframe.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    15357 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/postprocessing.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    30218 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/preprocessing.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    15925 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/submission.py
-drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-17 15:41:31.393349 numerblox-0.5.7/numerblox.egg-info/
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    12474 2023-04-17 15:41:31.000000 numerblox-0.5.7/numerblox.egg-info/PKG-INFO
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      612 2023-04-17 15:41:31.000000 numerblox-0.5.7/numerblox.egg-info/SOURCES.txt
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)        1 2023-04-17 15:41:31.000000 numerblox-0.5.7/numerblox.egg-info/dependency_links.txt
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       40 2023-04-17 15:41:31.000000 numerblox-0.5.7/numerblox.egg-info/entry_points.txt
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)        1 2023-04-05 12:35:40.000000 numerblox-0.5.7/numerblox.egg-info/not-zip-safe
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      194 2023-04-17 15:41:31.000000 numerblox-0.5.7/numerblox.egg-info/requires.txt
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       10 2023-04-17 15:41:31.000000 numerblox-0.5.7/numerblox.egg-info/top_level.txt
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     1071 2023-04-17 15:39:55.000000 numerblox-0.5.7/settings.ini
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       38 2023-04-17 15:41:31.393349 numerblox-0.5.7/setup.cfg
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     2537 2023-04-05 12:06:33.000000 numerblox-0.5.7/setup.py
+drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-18 16:54:27.747663 numerblox-0.5.8/
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     4767 2023-04-05 12:06:33.000000 numerblox-0.5.8/CONTRIBUTING.md
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    11357 2023-04-05 12:06:33.000000 numerblox-0.5.8/LICENSE
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      111 2023-04-05 12:06:33.000000 numerblox-0.5.8/MANIFEST.in
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    12474 2023-04-18 16:54:27.747663 numerblox-0.5.8/PKG-INFO
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    11651 2023-04-05 12:35:32.000000 numerblox-0.5.8/README.md
+drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-18 16:54:27.743662 numerblox-0.5.8/numerblox/
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       22 2023-04-18 16:53:38.000000 numerblox-0.5.8/numerblox/__init__.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    68222 2023-04-18 16:53:38.000000 numerblox-0.5.8/numerblox/_modidx.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     4073 2023-04-05 12:06:33.000000 numerblox-0.5.8/numerblox/_nbdev.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    22382 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/download.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    71551 2023-04-18 16:53:38.000000 numerblox-0.5.8/numerblox/evaluation.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      103 2023-04-05 12:06:33.000000 numerblox-0.5.8/numerblox/index.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      947 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/key.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      333 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/misc.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    26837 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/model.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     5985 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/model_pipeline.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     6929 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/numerframe.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    15357 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/postprocessing.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    30218 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/preprocessing.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    15925 2023-04-18 11:02:03.000000 numerblox-0.5.8/numerblox/submission.py
+drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-18 16:54:27.747663 numerblox-0.5.8/numerblox.egg-info/
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    12474 2023-04-18 16:54:27.000000 numerblox-0.5.8/numerblox.egg-info/PKG-INFO
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      612 2023-04-18 16:54:27.000000 numerblox-0.5.8/numerblox.egg-info/SOURCES.txt
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)        1 2023-04-18 16:54:27.000000 numerblox-0.5.8/numerblox.egg-info/dependency_links.txt
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       40 2023-04-18 16:54:27.000000 numerblox-0.5.8/numerblox.egg-info/entry_points.txt
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)        1 2023-04-05 12:35:40.000000 numerblox-0.5.8/numerblox.egg-info/not-zip-safe
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      194 2023-04-18 16:54:27.000000 numerblox-0.5.8/numerblox.egg-info/requires.txt
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       10 2023-04-18 16:54:27.000000 numerblox-0.5.8/numerblox.egg-info/top_level.txt
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     1071 2023-04-18 16:53:38.000000 numerblox-0.5.8/settings.ini
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       38 2023-04-18 16:54:27.747663 numerblox-0.5.8/setup.cfg
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     2537 2023-04-05 12:06:33.000000 numerblox-0.5.8/setup.py
```

### Comparing `numerblox-0.5.7/CONTRIBUTING.md` & `numerblox-0.5.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.7/LICENSE` & `numerblox-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.7/PKG-INFO` & `numerblox-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerblox
-Version: 0.5.7
+Version: 0.5.8
 Summary: Tools for solid Numerai pipelines
 Home-page: https://github.com/crowdcent/numerblox/
 Author: Jason Rosenfeld, Carlo Lepelaars and contributors
 Author-email: support@crowdcent.com
 License: Apache Software License 2.0
 Keywords: Numerai,Machine Learning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `numerblox-0.5.7/README.md` & `numerblox-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.7/numerblox/_modidx.py` & `numerblox-0.5.8/numerblox/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,16 @@
                                                                                                    'numerblox/evaluation.py'),
                                       'numerblox.evaluation.BaseEvaluator.mean_std_sharpe': ( 'evaluation.html#baseevaluator.mean_std_sharpe',
                                                                                               'numerblox/evaluation.py'),
                                       'numerblox.evaluation.BaseEvaluator.numerai_corr': ( 'evaluation.html#baseevaluator.numerai_corr',
                                                                                            'numerblox/evaluation.py'),
                                       'numerblox.evaluation.BaseEvaluator.per_era_corrs': ( 'evaluation.html#baseevaluator.per_era_corrs',
                                                                                             'numerblox/evaluation.py'),
+                                      'numerblox.evaluation.BaseEvaluator.per_era_numerai_corrs': ( 'evaluation.html#baseevaluator.per_era_numerai_corrs',
+                                                                                                    'numerblox/evaluation.py'),
                                       'numerblox.evaluation.BaseEvaluator.plot_correlations': ( 'evaluation.html#baseevaluator.plot_correlations',
                                                                                                 'numerblox/evaluation.py'),
                                       'numerblox.evaluation.BaseEvaluator.tbx_mean_std_sharpe': ( 'evaluation.html#baseevaluator.tbx_mean_std_sharpe',
                                                                                                   'numerblox/evaluation.py'),
                                       'numerblox.evaluation.NumeraiClassicEvaluator': ( 'evaluation.html#numeraiclassicevaluator',
                                                                                         'numerblox/evaluation.py'),
                                       'numerblox.evaluation.NumeraiClassicEvaluator.__init__': ( 'evaluation.html#numeraiclassicevaluator.__init__',
```

### Comparing `numerblox-0.5.7/numerblox/_nbdev.py` & `numerblox-0.5.8/numerblox/_nbdev.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.7/numerblox/download.py` & `numerblox-0.5.8/numerblox/download.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.7/numerblox/evaluation.py` & `numerblox-0.5.8/numerblox/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 # %% auto 0
 __all__ = ['FNCV4_FEATURES', 'FNCV3_FEATURES', 'MEDIUM_FEATURES', 'BaseEvaluator', 'NumeraiClassicEvaluator',
            'NumeraiSignalsEvaluator']
 
 # %% ../nbs/07_evaluation.ipynb 4
 import time
-import json
 import numpy as np
 import pandas as pd
 from scipy import stats
 from tqdm.auto import tqdm
 import matplotlib.pyplot as plt
 from typing import Tuple, Union
 from numerapi import SignalsAPI
@@ -92,32 +91,35 @@
         against given target and example prediction column.
         """
         col_stats = pd.DataFrame()
         # Compute stats
         val_corrs = self.per_era_corrs(
             dataf=dataf, pred_col=pred_col, target_col=target_col
         )
-        mean, std, sharpe = self.mean_std_sharpe(era_corrs=val_corrs)
-        max_drawdown = self.max_drawdown(era_corrs=val_corrs)
-        apy = self.apy(era_corrs=val_corrs)
+        val_numerai_corrs = self.per_era_numerai_corrs(
+            dataf=dataf, pred_col=pred_col, target_col=target_col
+        )
+        mean, std, sharpe = self.mean_std_sharpe(era_corrs=val_numerai_corrs)
+        legacy_mean, legacy_std, legacy_sharpe = self.mean_std_sharpe(era_corrs=val_corrs)
+        max_drawdown = self.max_drawdown(era_corrs=val_numerai_corrs)
+        apy = self.apy(era_corrs=val_numerai_corrs)
         example_corr = self.example_correlation(
             dataf=dataf, pred_col=pred_col, example_col=example_col
         )
-        numerai_corr = self.numerai_corr(
-            dataf=dataf, pred_col=pred_col, target_col=target_col
-        )
 
         col_stats.loc[pred_col, "target"] = target_col
         col_stats.loc[pred_col, "mean"] = mean
         col_stats.loc[pred_col, "std"] = std
         col_stats.loc[pred_col, "sharpe"] = sharpe
         col_stats.loc[pred_col, "max_drawdown"] = max_drawdown
         col_stats.loc[pred_col, "apy"] = apy
-        col_stats.loc[pred_col, "numerai_corr"] = numerai_corr
         col_stats.loc[pred_col, "corr_with_example_preds"] = example_corr
+        col_stats.loc[pred_col, "legacy_mean"] = legacy_mean
+        col_stats.loc[pred_col, "legacy_std"] = legacy_std
+        col_stats.loc[pred_col, "legacy_sharpe"] = legacy_sharpe
 
         # Compute intensive stats
         if not self.fast_mode:
             max_feature_exposure = self.max_feature_exposure(
                 dataf=dataf, pred_col=pred_col
             )
             fn_mean, fn_std, fn_sharpe = self.feature_neutral_mean_std_sharpe(
@@ -151,14 +153,22 @@
     ) -> pd.Series:
         """Correlation between prediction and target for each era."""
         return dataf.groupby(dataf[self.era_col]).apply(
             lambda d: self._normalize_uniform(d[pred_col].fillna(0.5)).corr(
                 d[target_col]
             )
         )
+    
+    def per_era_numerai_corrs(
+            self, dataf: pd.DataFrame, pred_col: str, target_col: str
+        ) -> pd.Series:
+        """Numerai Corr between prediction and target for each era."""
+        return dataf.groupby(dataf[self.era_col]).apply(
+            lambda d: self.numerai_corr(d.fillna(0.5), pred_col, target_col)
+            )
 
     def mean_std_sharpe(
         self, era_corrs: pd.Series
     ) -> Tuple[np.float64, np.float64, np.float64]:
         """
         Average, standard deviation and Sharpe ratio for
         correlations per era.
@@ -177,16 +187,16 @@
 
         Assumes original target col as input (i.e. in [0, 1] range).
         """
         # Rank and gaussianize predictions
         ranked_preds = self._normalize_uniform(dataf[pred_col].fillna(0.5), 
                                                method="average")
         gauss_ranked_preds = stats.norm.ppf(ranked_preds)
-        # Transform target from [0...1] to [-2...2] range
-        centered_target = dataf[target_col]*4 - 2
+        # Center target from [0...1] to [-0.5...0.5] range
+        centered_target = dataf[target_col] - 0.5
         # Accentuate tails of predictions and targets
         preds_p15 = np.sign(gauss_ranked_preds) * np.abs(gauss_ranked_preds) ** 1.5
         target_p15 = np.sign(centered_target) * np.abs(centered_target) ** 1.5
         # Pearson correlation
         corr, _ = stats.pearsonr(preds_p15, target_p15)
         return corr
 
@@ -244,15 +254,15 @@
         Feature neutralized mean performance.
         More info: https://docs.numer.ai/tournament/feature-neutral-correlation
         """
         fn = FeatureNeutralizer(pred_name=pred_col,
                                 feature_names=feature_names,
                                 proportion=1.0)
         neutralized_dataf = fn(dataf=dataf)
-        neutral_corrs = self.per_era_corrs(
+        neutral_corrs = self.per_era_numerai_corrs(
             dataf=neutralized_dataf,
             pred_col=f"{pred_col}_neutralized_1.0",
             target_col=target_col,
         )
         mean, std, sharpe = self.mean_std_sharpe(era_corrs=neutral_corrs)
         return mean, std, sharpe
 
@@ -278,19 +288,19 @@
         U = dataf.get_feature_data.corrwith(dataf[pred_col]).values
         E = dataf.get_feature_data.corrwith(dataf[example_col]).values
         exp_dis = 1 - np.dot(U, E) / np.dot(E, E)
         return exp_dis
 
 
     @staticmethod
-    def _neutralize_series(series, by, proportion=1.0):
+    def _neutralize_series(series: pd.Series, by: pd.Series, proportion=1.0) -> pd.Series:
         scores = series.values.reshape(-1, 1)
         exposures = by.values.reshape(-1, 1)
 
-        # this line makes series neutral to a constant column so that it's centered and for sure gets corr 0 with exposures
+        # This line makes series neutral to a constant column so that it's centered and for sure gets corr 0 with exposures
         exposures = np.hstack(
             (exposures, np.array([np.mean(series)] * len(exposures)).reshape(-1, 1))
         )
 
         correction = proportion * (
             exposures.dot(np.linalg.lstsq(exposures, scores, rcond=None)[0])
         )
@@ -352,15 +362,15 @@
         :param target_col: Target column name to compute per era correlations against.
         :param roll_mean: How many eras should be averaged to compute a rolling score.
         """
         validation_by_eras = pd.DataFrame()
         pred_cols = dataf.prediction_cols if not pred_cols else pred_cols
         # Compute per era correlation for each prediction column.
         for pred_col in pred_cols:
-            per_era_corrs = self.per_era_corrs(
+            per_era_corrs = self.per_era_numerai_corrs(
                 dataf, pred_col=pred_col, target_col=target_col
             )
             validation_by_eras.loc[:, pred_col] = per_era_corrs
 
         # Add prepared per era correlation if any.
         if corr_cols is not None:
             for corr_col in corr_cols:
```

### Comparing `numerblox-0.5.7/numerblox/key.py` & `numerblox-0.5.8/numerblox/key.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.7/numerblox/model.py` & `numerblox-0.5.8/numerblox/model.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.7/numerblox/model_pipeline.py` & `numerblox-0.5.8/numerblox/model_pipeline.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.7/numerblox/numerframe.py` & `numerblox-0.5.8/numerblox/numerframe.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.7/numerblox/postprocessing.py` & `numerblox-0.5.8/numerblox/postprocessing.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.7/numerblox/preprocessing.py` & `numerblox-0.5.8/numerblox/preprocessing.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.7/numerblox/submission.py` & `numerblox-0.5.8/numerblox/submission.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.7/numerblox.egg-info/PKG-INFO` & `numerblox-0.5.8/numerblox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerblox
-Version: 0.5.7
+Version: 0.5.8
 Summary: Tools for solid Numerai pipelines
 Home-page: https://github.com/crowdcent/numerblox/
 Author: Jason Rosenfeld, Carlo Lepelaars and contributors
 Author-email: support@crowdcent.com
 License: Apache Software License 2.0
 Keywords: Numerai,Machine Learning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `numerblox-0.5.7/numerblox.egg-info/SOURCES.txt` & `numerblox-0.5.8/numerblox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.7/settings.ini` & `numerblox-0.5.8/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 user = crowdcent
 description = Tools for solid Numerai pipelines
 keywords = Numerai, Machine Learning
 author = Jason Rosenfeld, Carlo Lepelaars and contributors
 author_email = support@crowdcent.com
 copyright = CrowdCent 2023
 branch = master
-version = 0.5.7
+version = 0.5.8
 min_python = 3.7
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 4
 requirements = jupyter eod wandb numpy scipy umap-learn pandas tqdm rich kaggle joblib pyarrow numerapi numerbay lightgbm catboost scikit-learn python-dateutil google-cloud-storage tensorflow pandas_ta
```

### Comparing `numerblox-0.5.7/setup.py` & `numerblox-0.5.8/setup.py`

 * *Files identical despite different names*

