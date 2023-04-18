# Comparing `tmp/ml4qc-0.1.8.tar.gz` & `tmp/ml4qc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml4qc-0.1.8.tar", last modified: Wed Jan 11 23:57:51 2023, max compression
+gzip compressed data, was "ml4qc-0.1.9.tar", last modified: Tue Feb 28 16:24:02 2023, max compression
```

## Comparing `ml4qc-0.1.8.tar` & `ml4qc-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2023-01-11 23:57:51.510574 ml4qc-0.1.8/
--rw-r--r--   0 crobert    (501) staff       (20)    11357 2022-09-21 12:34:08.000000 ml4qc-0.1.8/LICENSE
--rw-r--r--   0 crobert    (501) staff       (20)     5890 2023-01-11 23:57:51.510389 ml4qc-0.1.8/PKG-INFO
--rw-r--r--   0 crobert    (501) staff       (20)     5543 2023-01-11 23:41:56.000000 ml4qc-0.1.8/README.rst
--rw-r--r--   0 crobert    (501) staff       (20)       38 2023-01-11 23:57:51.510625 ml4qc-0.1.8/setup.cfg
--rw-r--r--   0 crobert    (501) staff       (20)     1302 2023-01-11 23:57:21.000000 ml4qc-0.1.8/setup.py
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2023-01-11 23:57:51.497160 ml4qc-0.1.8/src/
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2023-01-11 23:57:51.500177 ml4qc-0.1.8/src/ml4qc/
--rw-r--r--   0 crobert    (501) staff       (20)      884 2022-11-22 19:10:05.000000 ml4qc-0.1.8/src/ml4qc/__init__.py
--rw-r--r--   0 crobert    (501) staff       (20)    26802 2023-01-11 18:44:25.000000 ml4qc-0.1.8/src/ml4qc/surveyml.py
--rw-r--r--   0 crobert    (501) staff       (20)    31200 2023-01-10 00:54:07.000000 ml4qc-0.1.8/src/ml4qc/surveymlclassifier.py
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2023-01-11 23:57:51.510019 ml4qc-0.1.8/src/ml4qc.egg-info/
--rw-r--r--   0 crobert    (501) staff       (20)     5890 2023-01-11 23:57:51.000000 ml4qc-0.1.8/src/ml4qc.egg-info/PKG-INFO
--rw-r--r--   0 crobert    (501) staff       (20)      267 2023-01-11 23:57:51.000000 ml4qc-0.1.8/src/ml4qc.egg-info/SOURCES.txt
--rw-r--r--   0 crobert    (501) staff       (20)        1 2023-01-11 23:57:51.000000 ml4qc-0.1.8/src/ml4qc.egg-info/dependency_links.txt
--rw-r--r--   0 crobert    (501) staff       (20)       95 2023-01-11 23:57:51.000000 ml4qc-0.1.8/src/ml4qc.egg-info/requires.txt
--rw-r--r--   0 crobert    (501) staff       (20)        6 2023-01-11 23:57:51.000000 ml4qc-0.1.8/src/ml4qc.egg-info/top_level.txt
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2023-02-28 16:24:02.655936 ml4qc-0.1.9/
+-rw-r--r--   0 crobert    (501) staff       (20)    11357 2022-09-21 12:34:08.000000 ml4qc-0.1.9/LICENSE
+-rw-r--r--   0 crobert    (501) staff       (20)    10654 2023-02-28 16:24:02.655583 ml4qc-0.1.9/PKG-INFO
+-rw-r--r--   0 crobert    (501) staff       (20)    10307 2023-02-28 16:21:02.000000 ml4qc-0.1.9/README.rst
+-rw-r--r--   0 crobert    (501) staff       (20)       38 2023-02-28 16:24:02.655994 ml4qc-0.1.9/setup.cfg
+-rw-r--r--   0 crobert    (501) staff       (20)     1302 2023-02-28 15:40:59.000000 ml4qc-0.1.9/setup.py
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2023-02-28 16:24:02.646077 ml4qc-0.1.9/src/
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2023-02-28 16:24:02.647720 ml4qc-0.1.9/src/ml4qc/
+-rw-r--r--   0 crobert    (501) staff       (20)      884 2022-11-22 19:10:05.000000 ml4qc-0.1.9/src/ml4qc/__init__.py
+-rw-r--r--   0 crobert    (501) staff       (20)    41698 2023-02-28 16:07:58.000000 ml4qc-0.1.9/src/ml4qc/surveyml.py
+-rw-r--r--   0 crobert    (501) staff       (20)    31943 2023-02-25 13:15:28.000000 ml4qc-0.1.9/src/ml4qc/surveymlclassifier.py
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2023-02-28 16:24:02.655221 ml4qc-0.1.9/src/ml4qc.egg-info/
+-rw-r--r--   0 crobert    (501) staff       (20)    10654 2023-02-28 16:24:02.000000 ml4qc-0.1.9/src/ml4qc.egg-info/PKG-INFO
+-rw-r--r--   0 crobert    (501) staff       (20)      267 2023-02-28 16:24:02.000000 ml4qc-0.1.9/src/ml4qc.egg-info/SOURCES.txt
+-rw-r--r--   0 crobert    (501) staff       (20)        1 2023-02-28 16:24:02.000000 ml4qc-0.1.9/src/ml4qc.egg-info/dependency_links.txt
+-rw-r--r--   0 crobert    (501) staff       (20)       95 2023-02-28 16:24:02.000000 ml4qc-0.1.9/src/ml4qc.egg-info/requires.txt
+-rw-r--r--   0 crobert    (501) staff       (20)        6 2023-02-28 16:24:02.000000 ml4qc-0.1.9/src/ml4qc.egg-info/top_level.txt
```

### Comparing `ml4qc-0.1.8/LICENSE` & `ml4qc-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ml4qc-0.1.8/setup.py` & `ml4qc-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup
 
 with open('README.rst') as file:
     readme = file.read()
 
 setup(
     name='ml4qc',
-    version='0.1.8',
+    version='0.1.9',
     packages=['ml4qc'],
     python_requires='>=3.7',
     install_requires=['pandas', 'numpy', 'scikit-learn', 'seaborn', 'matplotlib', 'tensorflow', 'importlib_metadata',
                       'k-means-constrained'],
     package_dir={'': 'src'},
     url='https://github.com/orangechairlabs/ml4qc',
     project_urls={'Documentation': 'https://ml4qc.readthedocs.io/'},
```

### Comparing `ml4qc-0.1.8/src/ml4qc/__init__.py` & `ml4qc-0.1.9/src/ml4qc/__init__.py`

 * *Files identical despite different names*

### Comparing `ml4qc-0.1.8/src/ml4qc/surveymlclassifier.py` & `ml4qc-0.1.9/src/ml4qc/surveymlclassifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,36 +25,44 @@
 import tensorflow as tf
 
 
 class SurveyMLClassifier(SurveyML):
     """Class for using machine learning classification techniques on survey data."""
 
     def __init__(self, x_train_df: pd.DataFrame, y_train_df: pd.DataFrame, x_predict_df: pd.DataFrame = None,
-                 test_size: Union[float, int] = None, cv_when_training: bool = False, n_jobs: int = -2,
-                 random_state: Union[int, np.random.RandomState] = None, verbose: bool = None,
-                 calibration_method: str = None, threshold: str = 'default', threshold_value: float = None):
+                 test_size: Union[float, int] = None, cv_when_training: bool = False,
+                 control_features: list[str] = None, n_jobs: int = -2,
+                 random_state: Union[int, np.random.RandomState] = None, categorical_features: list[str] = None,
+                 verbose: bool = None, calibration_method: str = None, threshold: str = 'default',
+                 threshold_value: float = None):
         """
         Initialize survey data for classification using machine learning techniques.
 
         :param x_train_df: Features for training dataset
         :type x_train_df: pd.DataFrame
         :param y_train_df: Target(s) for training dataset
         :type y_train_df: pd.DataFrame
         :param x_predict_df: Prediction dataset (required unless test_size used to take test set from training set)
         :type x_predict_df: pd.DataFrame
         :param test_size: Float (0, 1) for proportion of training dataset to use for testing; int for number of
             training rows to use for testing; otherwise None to specify prediction set manually in x_predict_df
         :type test_size: Union[float, int]
         :param cv_when_training: True to cross-validate when training models
         :type cv_when_training: bool
+        :param control_features: List of features that should be used as controls (to transform all other features into
+            their residuals, once variation from these features is controlled out via OLS)
+        :type control_features: list[str]
         :param n_jobs: Number of parallel jobs to run during cross-validation (-1 for as many jobs as CPU's, -2 to
             leave one CPU free, etc.)
         :type n_jobs: int
         :param random_state: Fixed random state for reproducible results, otherwise None for random execution
         :type random_state: Union[int, np.random.RandomState]
+        :param categorical_features: List of feature names to force to categorical type ("other"), regardless of how
+            they auto-detect (e.g., for categorical features that might auto-classify as numeric), otherwise None
+        :type categorical_features: list[str]
         :param verbose: True to report verbose results with print() calls
         :type verbose: bool
         :param calibration_method: 'isotonic' or 'sigmoid' to perform probability calibration, otherwise None
         :type calibration_method: str
         :param threshold: Threshold to use for decision boundary: 'default' to let classifiers default to 0.5;
             'optimal_f' to automatically choose based on what maximizes the F score in the training set (defaults to
             F1 score, but you can specify a beta value to use in threshold_value);
@@ -67,15 +75,16 @@
         :type threshold_value: float
 
         Note: Currently, only binary classification problems are supported.
         """
 
         # initialize base class first
         super().__init__(x_train_df=x_train_df, y_train_df=y_train_df, x_predict_df=x_predict_df, test_size=test_size,
-                         cv_when_training=cv_when_training, n_jobs=n_jobs, random_state=random_state, verbose=verbose)
+                         cv_when_training=cv_when_training, control_features=control_features, n_jobs=n_jobs,
+                         random_state=random_state, categorical_features=categorical_features, verbose=verbose)
 
         # confirm that we're set up for binary classification problems (the only problems currently supported)
         unique_vals = self.y_train_df.iloc[:, 0].unique()
         if self.y_train_df.shape[1] != 1 or len(unique_vals) != 2 or 0 not in unique_vals or 1 not in unique_vals:
             raise ValueError("Currently, only binary classification problems are supported, so must have a single "
                              "target column with only 0's and 1's in it.")
```

