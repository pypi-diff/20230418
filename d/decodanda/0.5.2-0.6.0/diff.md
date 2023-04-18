# Comparing `tmp/decodanda-0.5.2.tar.gz` & `tmp/decodanda-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decodanda-0.5.2.tar", last modified: Wed Feb 22 19:30:33 2023, max compression
+gzip compressed data, was "decodanda-0.6.0.tar", last modified: Tue Apr 18 20:21:06 2023, max compression
```

## Comparing `decodanda-0.5.2.tar` & `decodanda-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-02-22 19:30:33.695068 decodanda-0.5.2/
--rw-r--r--   0 lorenzo    (501) staff       (20)    35149 2023-02-15 23:52:18.000000 decodanda-0.5.2/LICENSE.md
--rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-02-22 19:30:33.694703 decodanda-0.5.2/PKG-INFO
--rw-r--r--   0 lorenzo    (501) staff       (20)    35652 2023-02-20 04:52:59.000000 decodanda-0.5.2/README.md
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-02-22 19:30:33.692318 decodanda-0.5.2/decodanda/
--rw-r--r--   0 lorenzo    (501) staff       (20)      251 2023-02-17 22:21:32.000000 decodanda-0.5.2/decodanda/__init__.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    90638 2023-02-22 19:27:21.000000 decodanda-0.5.2/decodanda/classes.py
--rw-r--r--   0 lorenzo    (501) staff       (20)     1194 2023-02-15 00:18:50.000000 decodanda-0.5.2/decodanda/imports.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    11247 2023-02-17 19:33:24.000000 decodanda-0.5.2/decodanda/in_time.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    39339 2023-02-17 17:08:36.000000 decodanda-0.5.2/decodanda/utilities.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    19659 2023-02-16 22:56:04.000000 decodanda-0.5.2/decodanda/visualize.py
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-02-22 19:30:33.694239 decodanda-0.5.2/decodanda.egg-info/
--rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-02-22 19:30:33.000000 decodanda-0.5.2/decodanda.egg-info/PKG-INFO
--rw-r--r--   0 lorenzo    (501) staff       (20)      324 2023-02-22 19:30:33.000000 decodanda-0.5.2/decodanda.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)        1 2023-02-22 19:30:33.000000 decodanda-0.5.2/decodanda.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)      109 2023-02-22 19:30:33.000000 decodanda-0.5.2/decodanda.egg-info/requires.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)       10 2023-02-22 19:30:33.000000 decodanda-0.5.2/decodanda.egg-info/top_level.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)       38 2023-02-22 19:30:33.695186 decodanda-0.5.2/setup.cfg
--rw-r--r--   0 lorenzo    (501) staff       (20)     1388 2023-02-22 19:29:19.000000 decodanda-0.5.2/setup.py
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:21:06.437799 decodanda-0.6.0/
+-rw-r--r--   0 lorenzo    (501) staff       (20)    35149 2023-02-15 23:52:18.000000 decodanda-0.6.0/LICENSE.md
+-rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-18 20:21:06.437451 decodanda-0.6.0/PKG-INFO
+-rw-r--r--   0 lorenzo    (501) staff       (20)    35652 2023-02-20 04:52:59.000000 decodanda-0.6.0/README.md
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:21:06.434348 decodanda-0.6.0/decodanda/
+-rw-r--r--   0 lorenzo    (501) staff       (20)      251 2023-02-17 22:21:32.000000 decodanda-0.6.0/decodanda/__init__.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    97881 2023-04-18 20:06:07.000000 decodanda-0.6.0/decodanda/classes.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1194 2023-02-15 00:18:50.000000 decodanda-0.6.0/decodanda/imports.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    11247 2023-02-17 19:33:24.000000 decodanda-0.6.0/decodanda/in_time.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    39339 2023-02-17 17:08:36.000000 decodanda-0.6.0/decodanda/utilities.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    19659 2023-02-16 22:56:04.000000 decodanda-0.6.0/decodanda/visualize.py
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-04-18 20:21:06.436972 decodanda-0.6.0/decodanda.egg-info/
+-rw-r--r--   0 lorenzo    (501) staff       (20)      991 2023-04-18 20:21:06.000000 decodanda-0.6.0/decodanda.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzo    (501) staff       (20)      324 2023-04-18 20:21:06.000000 decodanda-0.6.0/decodanda.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)        1 2023-04-18 20:21:06.000000 decodanda-0.6.0/decodanda.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)      109 2023-04-18 20:21:06.000000 decodanda-0.6.0/decodanda.egg-info/requires.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)       10 2023-04-18 20:21:06.000000 decodanda-0.6.0/decodanda.egg-info/top_level.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)       38 2023-04-18 20:21:06.437924 decodanda-0.6.0/setup.cfg
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1388 2023-04-18 20:19:01.000000 decodanda-0.6.0/setup.py
```

### Comparing `decodanda-0.5.2/LICENSE.md` & `decodanda-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `decodanda-0.5.2/PKG-INFO` & `decodanda-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decodanda
-Version: 0.5.2
+Version: 0.6.0
 Summary: A python package for neural decoding with built-in best practices.
 Home-page: https://github.com/lposani/decodanda
 Author: Lorenzo Posani
 Author-email: lorenzo.posani@gmail.com
 Keywords: python,decoding,neuroscience,ccgp,neural activity,population activity,neural decoding,geometry
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `decodanda-0.5.2/README.md` & `decodanda-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `decodanda-0.5.2/decodanda/classes.py` & `decodanda-0.6.0/decodanda/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU General Public License for more details.
 #
 
 import copy
 from typing import Tuple, Union
+
+import scipy.stats.stats
 from numpy import ndarray
 from .imports import *
 from .utilities import generate_binary_words, string_bool, sample_training_testing_from_rasters, CrossValidator, \
     log_dichotomy, hamming, sample_from_rasters, generate_dichotomies, semantic_score, z_pval, DictSession, \
-    contiguous_chunking, non_contiguous_mask
+    contiguous_chunking, non_contiguous_mask, cosine
 from .visualize import corr_scatter, visualize_decoding, plot_perfs_null_model
 
 
 # Main class
 
 class Decodanda:
     def __init__(self,
@@ -183,15 +185,14 @@
 
         The constructor divides the data into conditions using the ``stimulus`` and ``action`` values
         and stores them in the ``self.conditioned_rasters`` object.
         This condition structure is the basis for all the balanced decoding analyses.
 
         """
 
-
         # casting single session to a list so that it is compatible with all loops below
         if type(data) != list:
             data = [data]
 
         # handling dictionaries as sessions
 
         # TODO: change default behavior with dictionaries instead of data structures
@@ -338,19 +339,19 @@
         training_array_B = []
         testing_array_A = []
         testing_array_B = []
 
         # allow for unbalanced dichotomies
         n_conditions_A = float(len(dic[0]))
         n_conditions_B = float(len(dic[1]))
-        fraction = n_conditions_A/n_conditions_B
+        fraction = n_conditions_A / n_conditions_B
 
         for d in set_A:
             training, testing = sample_training_testing_from_rasters(self.conditioned_rasters[d],
-                                                                     int(ndata/fraction),
+                                                                     int(ndata / fraction),
                                                                      training_fraction,
                                                                      self.conditioned_trial_index[d],
                                                                      debug=self._debug,
                                                                      testing_trials=testing_trials)
             if self._debug:
                 plt.title('Condition A')
                 print("Sampling for condition A, d=%s" % d)
@@ -386,18 +387,18 @@
             corr_scatter(selectivity_training, selectivity_testing, 'Selectivity (training)', 'Selectivity (testing)')
 
         if self._zscore:
             big_raster = np.vstack([training_array_A, training_array_B, testing_array_A, testing_array_B])
             big_mean = np.nanmean(big_raster, 0)
             big_std = np.nanstd(big_raster, 0)
             big_std[big_std == 0] = np.inf
-            training_array_A = (training_array_A - big_mean)/big_std
-            training_array_B = (training_array_B - big_mean)/big_std
-            testing_array_A = (testing_array_A - big_mean)/big_std
-            testing_array_B = (testing_array_B - big_mean)/big_std
+            training_array_A = (training_array_A - big_mean) / big_std
+            training_array_B = (training_array_B - big_mean) / big_std
+            testing_array_A = (testing_array_A - big_mean) / big_std
+            testing_array_B = (testing_array_B - big_mean) / big_std
 
         self._train(training_array_A, training_array_B, label_A, label_B)
 
         if hasattr(self.classifier, 'coef_'):
             if dic_key and not shuffled:
                 if dic_key not in self.decoding_weights.keys():
                     self.decoding_weights[dic_key] = []
@@ -407,15 +408,15 @@
                     self.decoding_weights_null[dic_key] = []
                 self.decoding_weights_null[dic_key].append(self.classifier.coef_)
 
         performance = self._test(testing_array_A, testing_array_B, label_A, label_B)
 
         return performance
 
-    # Dichotomy decoding functions
+    # Dichotomy analysis functions
 
     def decode_dichotomy(self, dichotomy: Union[str, list], training_fraction: float,
                          cross_validations: int = 10, ndata: Optional[int] = None,
                          shuffled: bool = False, parallel: bool = False,
                          testing_trials: Optional[list] = None,
                          dic_key: Optional[str] = None, **kwargs) -> ndarray:
         """
@@ -542,15 +543,19 @@
                 performances[i] = self._one_cv_step(dic=dic, training_fraction=training_fraction, ndata=ndata,
                                                     shuffled=shuffled, testing_trials=testing_trials, dic_key=dic_key)
 
         if shuffled:
             self._order_conditioned_rasters()
         return np.asarray(performances)
 
-    def CCGP_dichotomy(self, dichotomy, resamplings=3, ndata: Optional[int] = None, max_semantic_dist=1, shuffled=False):
+    def CCGP_dichotomy(self, dichotomy: Union[str, list],
+                       resamplings: int = 3,
+                       ndata: Optional[int] = None,
+                       max_semantic_dist: int = 1,
+                       shuffled: bool = False):
         """
         Function that performs the cross-condition generalization performance analysis (CCGP, Bernardi et al. 2020, Cell)
         for a given variable, specified through its corresponding dichotomy. This function tests how well a given
         coding strategy for the given variable generalizes when the other variables are changed.
 
 
         Parameters
@@ -688,21 +693,96 @@
                             rotation_A = np.arange(testing_array_A.shape[1]).astype(int)
                             rotation_B = np.arange(testing_array_B.shape[1]).astype(int)
                             np.random.shuffle(rotation_A)
                             np.random.shuffle(rotation_B)
                             testing_array_A = testing_array_A[:, rotation_A]
                             testing_array_B = testing_array_B[:, rotation_A]
 
+                        if self._zscore:
+                            big_raster = np.vstack(
+                                [training_array_A, training_array_B, testing_array_A, testing_array_B])
+                            big_mean = np.nanmean(big_raster, 0)
+                            big_std = np.nanstd(big_raster, 0)
+                            big_std[big_std == 0] = np.inf
+                            training_array_A = (training_array_A - big_mean) / big_std
+                            training_array_B = (training_array_B - big_mean) / big_std
+                            testing_array_A = (testing_array_A - big_mean) / big_std
+                            testing_array_B = (testing_array_B - big_mean) / big_std
+
                         self._train(training_array_A, training_array_B, label_A, label_B)
                         performance = self._test(testing_array_A, testing_array_B, label_A, label_B)
                         performances.append(performance)
 
             all_performances.append(performances)
         return np.nanmean(all_performances, 0)
 
+    def parallelism_score_dichotomy(self, dichotomy: Union[str, list],
+                                    max_semantic_dist: int = 1,
+                                    shuffled: bool = False,
+                                    method: str = 'pearson',
+                                    return_combinations: bool = False):
+        if type(dichotomy) == str:
+            dic = self._dichotomy_from_key(dichotomy)
+        else:
+            dic = dichotomy
+
+        ndata = 2 * self._max_conditioned_data
+
+        coding_directions = []
+
+        set_A = dic[0]
+        set_B = dic[1]
+
+        for i in range(len(set_A)):
+            for j in range(len(set_B)):
+                test_condition_A = set_A[i]
+                test_condition_B = set_B[j]
+                if hamming(string_bool(test_condition_A), string_bool(test_condition_B)) <= max_semantic_dist:
+                    testing_array_A = sample_from_rasters(self.conditioned_rasters[test_condition_A], ndata=ndata)
+                    testing_array_B = sample_from_rasters(self.conditioned_rasters[test_condition_B], ndata=ndata)
+
+                    if shuffled:
+                        rotation_A = np.arange(testing_array_A.shape[1]).astype(int)
+                        rotation_B = np.arange(testing_array_B.shape[1]).astype(int)
+                        np.random.shuffle(rotation_A)
+                        np.random.shuffle(rotation_B)
+                        testing_array_A = testing_array_A[:, rotation_A]
+                        testing_array_B = testing_array_B[:, rotation_A]
+
+                    if self._zscore:
+                        big_raster = np.vstack([testing_array_A, testing_array_B])
+                        big_mean = np.nanmean(big_raster, 0)
+                        big_std = np.nanstd(big_raster, 0)
+                        big_std[big_std == 0] = np.inf
+                        testing_array_A = (testing_array_A - big_mean) / big_std
+                        testing_array_B = (testing_array_B - big_mean) / big_std
+
+                    vA = np.nanmean(testing_array_A, 0)
+                    vB = np.nanmean(testing_array_B, 0)
+                    coding_directions.append(vB - vA)
+
+        parallelism_scores = []
+        for i in range(len(coding_directions)):
+            for j in range(i + 1, len(coding_directions)):
+                if method == 'pearson':
+                    parallelism_scores.append(scipy.stats.pearsonr(coding_directions[i], coding_directions[j])[0])
+                elif method == 'cosine':
+                    parallelism_scores.append(cosine(coding_directions[i], coding_directions[j]))
+                elif method == 'spearman':
+                    parallelism_scores.append(scipy.stats.spearmanr(coding_directions[i], coding_directions[j])[0])
+                else:
+                    raise ValueError(
+                        "The specified method is not supported, please use one of: pearson, cosine, spearman")
+        if return_combinations:
+            return np.asarray(parallelism_scores)
+        else:
+            return np.nanmean(parallelism_scores)
+
+    # Dichotomy analysis functions with null model
+
     def decode_with_nullmodel(self, dichotomy: Union[str, list],
                               training_fraction: float,
                               cross_validations: int = 10,
                               nshuffles: int = 10,
                               ndata: Optional[int] = None,
                               parallel: bool = False,
                               return_CV: bool = False,
@@ -849,15 +929,20 @@
 
         if plot:
             visualize_decoding(self, dic, d_performances, null_model_performances,
                                training_fraction=training_fraction, ndata=ndata, testing_trials=testing_trials)
 
         return data_performance, null_model_performances
 
-    def CCGP_with_nullmodel(self, dichotomy, resamplings=5, nshuffles=25, ndata: Optional[int] = None, max_semantic_dist=1, return_combinations=False):
+    def CCGP_with_nullmodel(self, dichotomy: Union[str, list],
+                            resamplings: int = 5,
+                            nshuffles: int = 25,
+                            ndata: Optional[int] = None,
+                            max_semantic_dist: int = 1,
+                            return_combinations: bool = False):
 
         """
                 Function that performs the cross-condition generalization performance analysis (CCGP, Bernardi et al. 2020, Cell)
                 for a given variable, specified through its corresponding dichotomy.
 
                     This function tests how well a given coding strategy for the given variable generalizes
                 when the other variables are changed and compares the
@@ -941,15 +1026,16 @@
                 >>> perf, null = dec.CCGP_with_nullmodel('stimulus', nshuffles=10)
                 >>> perf
                 0.85
                 >>> null
                 [0.44, 0.48, ..., 0.54] # 10 values
                 """
 
-        performances = self.CCGP_dichotomy(dichotomy=dichotomy, resamplings=resamplings, ndata=ndata, max_semantic_dist=max_semantic_dist)
+        performances = self.CCGP_dichotomy(dichotomy=dichotomy, resamplings=resamplings, ndata=ndata,
+                                           max_semantic_dist=max_semantic_dist)
 
         if return_combinations:
             ccgp = performances
         else:
             ccgp = np.nanmean(performances)
 
         if self._verbose and nshuffles:
@@ -968,15 +1054,43 @@
             if return_combinations:
                 shuffled_ccgp.append(performances)
             else:
                 shuffled_ccgp.append(np.nanmean(performances))
 
         return ccgp, shuffled_ccgp
 
-    # Analysis functions for semantic dichotomies
+    def PS_with_nullmodel(self, dichotomy: Union[str, list],
+                          nshuffles: int = 25,
+                          max_semantic_dist: int = 1,
+                          method: str = 'pearson',
+                          return_combinations: bool = False):
+
+        scores = self.parallelism_score_dichotomy(dichotomy=dichotomy,
+                                                  method=method,
+                                                  max_semantic_dist=max_semantic_dist,
+                                                  return_combinations=return_combinations)
+
+        if self._verbose and nshuffles:
+            print("\t\t[PS_with_nullmodel]\t\t----- Data: <p> = %.2f -----\n" % np.nanmean(scores))
+            count = tqdm(range(nshuffles))
+        else:
+            count = range(nshuffles)
+
+        shuffled_scores = []
+        for n in count:
+            scores_null = self.parallelism_score_dichotomy(dichotomy=dichotomy,
+                                                           method=method,
+                                                           max_semantic_dist=max_semantic_dist,
+                                                           return_combinations=return_combinations,
+                                                           shuffled=True)
+            shuffled_scores.append(scores_null)
+
+        return scores, shuffled_scores
+
+    # Decoding analysis for semantic dichotomies
 
     def decode(self, training_fraction: float,
                cross_validations: int = 10,
                nshuffles: int = 10,
                ndata: Optional[int] = None,
                parallel: bool = False,
                non_semantic: bool = False,
@@ -1038,15 +1152,15 @@
         testing_trials:
             if specified, data sampled from the specified trial numbers will be used for testing, and the remaining ones for training.
         non_semantic:
             if True, non-semantic dichotomies (i.e., dichotomies that do not correspond to a variable) will also be decoded.
         plot:
             if True, a visualization of the decoding results is shown.
         ax:
-            if specified and ``plot=True``, the results will be duplayed in the specified axis instead of a new figure.
+            if specified and ``plot=True``, the results will be displayed in the specified axis instead of a new figure.
         plot_all:
             if True, a more in-depth visualization of the decoding results and of the decoded data is shown.
 
 
         Returns
         -------
             perfs:
@@ -1125,17 +1239,20 @@
         if plot:
             if not ax:
                 f, ax = plt.subplots(figsize=(0.5 + 1.8 * len(perfs.keys()), 3.5))
             plot_perfs_null_model(perfs, perfs_nullmodel, ylabel='Decoding performance', ax=ax, **kwargs)
 
         return perfs, perfs_nullmodel
 
+    # Geometrical analysis for semantic dichotomies
+
     def CCGP(self, resamplings=5,
              nshuffles: int = 25,
              ndata: Optional[int] = None,
+             max_semantic_dist: int = 1,
              plot: bool = False,
              ax: Optional[plt.Axes] = None,
              **kwargs):
 
         """
         Main function that performs the cross-condition generalization performance analysis (CCGP, Bernardi et al. 2020, Cell)
         for the variables specified through the ``conditions`` dictionary.
@@ -1154,14 +1271,18 @@
                 The number of iterations for each decoding analysis. The returned performance value is the average over these resamplings.
             nshuffles:
                 The number of null-model iterations for the CCGP analysis.
             ndata:
                 The number of data points (population vectors) sampled for training and for testing for each condition.
             max_semantic_dist:
                 The maximum semantic distance (number of variables that change value) between conditions in the held-out pair used to test the classifier.
+            plot:
+                if True, a visualization of the decoding results is shown.
+            ax:
+                if specified and ``plot=True``, the results will be displayed in the specified axis instead of a new figure.
 
         Returns
         -------
             performance: mean of performance values for each cross-condition training-testing split.
             null: a list of null values for the generalization performance
 
         See Also
@@ -1209,25 +1330,53 @@
         for key, dic in zip(semantic_keys, semantic_dics):
             if self._verbose:
                 print("\nTesting CCGP for semantic dichotomy: ", key)
             data_ccgp, null_ccgps = self.CCGP_with_nullmodel(dichotomy=dic,
                                                              resamplings=resamplings,
                                                              nshuffles=nshuffles,
                                                              ndata=ndata,
-                                                             max_semantic_dist=1)
+                                                             max_semantic_dist=max_semantic_dist)
             ccgp[key] = data_ccgp
             ccgp_nullmodel[key] = null_ccgps
 
         if plot:
             if not ax:
                 f, ax = plt.subplots(figsize=(0.5 + 1.8 * len(semantic_dics), 3.5))
             plot_perfs_null_model(ccgp, ccgp_nullmodel, ylabel='CCGP', ax=ax, **kwargs)
 
         return ccgp, ccgp_nullmodel
 
+    def PS(self, nshuffles: int = 25,
+           max_semantic_dist: int = 1,
+           method: str = 'pearson',
+           plot: bool = False,
+           ax: Optional[plt.Axes] = None,
+           **kwargs):
+
+        semantic_dics, semantic_keys = self._find_semantic_dichotomies()
+
+        ps = {}
+        ps_nullmodel = {}
+        for key, dic in zip(semantic_keys, semantic_dics):
+            if self._verbose:
+                print("\nTesting PS for semantic dichotomy: ", key)
+            data_ps, null_ps = self.PS_with_nullmodel(dichotomy=dic,
+                                                      nshuffles=nshuffles,
+                                                      method=method,
+                                                      max_semantic_dist=max_semantic_dist)
+            ps[key] = data_ps
+            ps_nullmodel[key] = null_ps
+
+        if plot:
+            if not ax:
+                f, ax = plt.subplots(figsize=(0.5 + 1.8 * len(semantic_dics), 3.5))
+            plot_perfs_null_model(ps, ps_nullmodel, ylabel='Parallelism Score', ax=ax, ylow=-1.05, yhigh=1.05, chance=0, **kwargs)
+
+        return ps, ps_nullmodel
+
     def semantic_score_geometry(self,
                                 training_fraction: float = 0.75,
                                 cross_validations: int = 10,
                                 nshuffles: int = 10,
                                 ndata: Optional[int] = None,
                                 visualize=True):
         """
@@ -1421,15 +1570,15 @@
                 # select bins conditioned on the semantic behavioural vector
                 conditioned_raster = array[mask, :]
 
                 # Define trial logic
                 def condition_no(cond):
                     no = 0
                     for i in range(len(cond)):
-                        no += cond[i]*10**(i+2)
+                        no += cond[i] * 10 ** (i + 2)
                     return no
 
                 if self._trial_attr is not None:
                     conditioned_trial = getattr(session, self._trial_attr)[mask]
                 elif self._trial_chunk is None:
                     if self._verbose:
                         print('[Decodanda]\tUsing contiguous chunks of the same labels as trials.')
@@ -1543,15 +1692,15 @@
         return dichotomies
 
     def _powerchotomies(self):
         conditions = list(self._semantic_vectors.keys())
         powerset = list(chain.from_iterable(combinations(conditions, r) for r in range(1, len(conditions))))
         dichotomies = {}
         for i in range(len(powerset)):
-            for j in range(i+1, len(powerset)):
+            for j in range(i + 1, len(powerset)):
                 if len(np.unique(powerset[i] + powerset[j])) == len(conditions):
                     if len(powerset[i] + powerset[j]) == len(conditions):
                         dic = [list(powerset[i]), list(powerset[j])]
                         dichotomies[_powerchotomy_to_key(dic)] = dic
         return dichotomies
 
     def _dic_key(self, dic):
@@ -1679,15 +1828,16 @@
         else:
             for n in range(self.n_brains):
                 # select conditioned rasters
                 for iteration in range(10):
                     all_conditions = list(self._semantic_vectors.keys())
                     all_data = np.vstack([self.conditioned_rasters[cond][n] for cond in all_conditions])
                     all_trials = np.hstack([self.conditioned_trial_index[cond][n] for cond in all_conditions])
-                    all_n_trials = {cond: len(np.unique(self.conditioned_trial_index[cond][n])) for cond in all_conditions}
+                    all_n_trials = {cond: len(np.unique(self.conditioned_trial_index[cond][n])) for cond in
+                                    all_conditions}
 
                     unique_trials = np.unique(all_trials)
                     np.random.shuffle(unique_trials)
 
                     i = 0
                     for cond in all_conditions:
                         cond_trials = unique_trials[i:i + all_n_trials[cond]]
@@ -1868,17 +2018,18 @@
                     sampling = np.random.choice(t2, t1, replace=False)
                 if sampling_strategy == 'ordered':
                     sampling = np.arange(t1, dtype=int)
                 list(d2.conditioned_rasters.values())[i][n] = list(d2.conditioned_rasters.values())[i][n][sampling, :]
                 list(d2.conditioned_trial_index.values())[i][n] = list(d2.conditioned_trial_index.values())[i][n][
                     sampling]
 
-            print("Balancing data for d1: %u, d2: %u - now d1: %u, d2: %u" % (
-                t1, t2, list(d1.conditioned_rasters.values())[i][n].shape[0],
-                list(d2.conditioned_rasters.values())[i][n].shape[0]))
+            if d1._verbose:
+                print("Balancing data for d1: %u, d2: %u - now d1: %u, d2: %u" % (
+                    t1, t2, list(d1.conditioned_rasters.values())[i][n].shape[0],
+                    list(d2.conditioned_rasters.values())[i][n].shape[0]))
 
     for w in d1.conditioned_rasters.keys():
         d1.ordered_conditioned_rasters[w] = d1.conditioned_rasters[w].copy()
         d1.ordered_conditioned_trial_index[w] = d1.conditioned_trial_index[w].copy()
         d2.ordered_conditioned_rasters[w] = d2.conditioned_rasters[w].copy()
         d2.ordered_conditioned_trial_index[w] = d2.conditioned_trial_index[w].copy()
 
@@ -1910,15 +2061,15 @@
             '%s' % discrete_dict[key][0]: lambda d, k=key: getattr(d, k) == discrete_dict[k][0],
             '%s' % discrete_dict[key][1]: lambda d, k=key: getattr(d, k) == discrete_dict[k][1],
         }
     return conditions
 
 
 def _powerchotomy_to_key(dic):
-    return '_'.join(dic[0])+'_v_'+'_'.join(dic[1])
+    return '_'.join(dic[0]) + '_v_' + '_'.join(dic[1])
 
 
 class _NullmodelIterator(object):  # necessary for parallelization of null model iterations
     def __init__(self, data, conditions, decodanda_params, analysis_params):
         self.data = data
         self.conditions = conditions
         self.decodanda_params = decodanda_params
@@ -1940,8 +2091,7 @@
                 print("\nTesting null decoding performance for semantic dichotomy: ", key)
             dec._shuffle_conditioned_arrays(dic)
             performance = dec.decode_dichotomy(dic, **self.analysis_params)
             perfs[key] = np.nanmean(performance)
             dec._order_conditioned_rasters()
 
         return perfs
-
```

### Comparing `decodanda-0.5.2/decodanda/imports.py` & `decodanda-0.6.0/decodanda/imports.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.5.2/decodanda/in_time.py` & `decodanda-0.6.0/decodanda/in_time.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.5.2/decodanda/utilities.py` & `decodanda-0.6.0/decodanda/utilities.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.5.2/decodanda/visualize.py` & `decodanda-0.6.0/decodanda/visualize.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.5.2/decodanda.egg-info/PKG-INFO` & `decodanda-0.6.0/decodanda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decodanda
-Version: 0.5.2
+Version: 0.6.0
 Summary: A python package for neural decoding with built-in best practices.
 Home-page: https://github.com/lposani/decodanda
 Author: Lorenzo Posani
 Author-email: lorenzo.posani@gmail.com
 Keywords: python,decoding,neuroscience,ccgp,neural activity,population activity,neural decoding,geometry
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `decodanda-0.5.2/setup.py` & `decodanda-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.5.2'
+VERSION = '0.6.0'
 DESCRIPTION = 'A python package for neural decoding with built-in best practices.'
 LONG_DESCRIPTION = 'Decodanda (dog latin for "to be decoded") is a best-practices-made-easy Python package for decoding neural data. Decodanda is designed to expose a user-friendly and flexible interface for population activity decoding, with a series of built-in best practices to avoid the most common pitfalls. In addition, Decodanda exposes a series of functions to compute the Cross-Condition Generalization Performance (CCGP, Bernardi et al. 2020) for the geometrical analysis of neural population activity.'
 
 setup(
     name="decodanda",
     version=VERSION,
     author="Lorenzo Posani",
```

