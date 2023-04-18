# Comparing `tmp/skshift-0.1.3.tar.gz` & `tmp/skshift-0.1.4.tar.gz`

## Comparing `skshift-0.1.3.tar` & `skshift-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 skshift-0.1.3/HowTo.md
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 skshift-0.1.3/Makefile
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 skshift-0.1.3/README.rst
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 skshift-0.1.3/requirements.txt
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 skshift-0.1.3/tutorial.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 skshift-0.1.3/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 skshift-0.1.3/docs/make.bat
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 skshift-0.1.3/docs/source/conf.py
--rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 skshift-0.1.3/docs/source/explanationTutorial.rst
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 skshift-0.1.3/docs/source/index.rst
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 skshift-0.1.3/docs/source/installation.rst
--rw-r--r--   0        0        0    18603 2020-02-02 00:00:00.000000 skshift-0.1.3/docs/source/images/breastShapGlobal.png
--rw-r--r--   0        0        0    25344 2020-02-02 00:00:00.000000 skshift-0.1.3/docs/source/images/breastShapLocal.png
--rw-r--r--   0        0        0    45221 2020-02-02 00:00:00.000000 skshift-0.1.3/docs/source/images/folksShapLocal.png
--rw-r--r--   0        0        0    44661 2020-02-02 00:00:00.000000 skshift-0.1.3/docs/source/images/folksShapLocalMI.png
--rw-r--r--   0        0        0    30922 2020-02-02 00:00:00.000000 skshift-0.1.3/docs/source/images/folkstShapGlobal.png
--rw-r--r--   0        0        0    30734 2020-02-02 00:00:00.000000 skshift-0.1.3/docs/source/images/folkstShapGlobalMI.png
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 skshift-0.1.3/skshift/__init__.py
--rw-r--r--   0        0        0     8503 2020-02-02 00:00:00.000000 skshift-0.1.3/skshift/audits.py
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 skshift-0.1.3/skshift/distributionshift.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 skshift-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 skshift-0.1.3/tests/test_audit.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 skshift-0.1.3/tests/test_explanationShift2.py
--rw-r--r--   0        0        0     6041 2020-02-02 00:00:00.000000 skshift-0.1.3/tests/test_explanationshift.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 skshift-0.1.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 skshift-0.1.3/LICENSE
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 skshift-0.1.3/README.md
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 skshift-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 skshift-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 skshift-0.1.4/HowTo.md
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 skshift-0.1.4/Makefile
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 skshift-0.1.4/README.rst
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 skshift-0.1.4/requirements.txt
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 skshift-0.1.4/tutorial.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 skshift-0.1.4/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 skshift-0.1.4/docs/make.bat
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 skshift-0.1.4/docs/source/conf.py
+-rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 skshift-0.1.4/docs/source/explanationTutorial.rst
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 skshift-0.1.4/docs/source/index.rst
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 skshift-0.1.4/docs/source/installation.rst
+-rw-r--r--   0        0        0    18603 2020-02-02 00:00:00.000000 skshift-0.1.4/docs/source/images/breastShapGlobal.png
+-rw-r--r--   0        0        0    25344 2020-02-02 00:00:00.000000 skshift-0.1.4/docs/source/images/breastShapLocal.png
+-rw-r--r--   0        0        0    45221 2020-02-02 00:00:00.000000 skshift-0.1.4/docs/source/images/folksShapLocal.png
+-rw-r--r--   0        0        0    44661 2020-02-02 00:00:00.000000 skshift-0.1.4/docs/source/images/folksShapLocalMI.png
+-rw-r--r--   0        0        0    30922 2020-02-02 00:00:00.000000 skshift-0.1.4/docs/source/images/folkstShapGlobal.png
+-rw-r--r--   0        0        0    30734 2020-02-02 00:00:00.000000 skshift-0.1.4/docs/source/images/folkstShapGlobalMI.png
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 skshift-0.1.4/skshift/__init__.py
+-rw-r--r--   0        0        0     8503 2020-02-02 00:00:00.000000 skshift-0.1.4/skshift/audits.py
+-rw-r--r--   0        0        0     7370 2020-02-02 00:00:00.000000 skshift-0.1.4/skshift/distributionshift.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 skshift-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 skshift-0.1.4/tests/test_audit.py
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 skshift-0.1.4/tests/test_explanationShift2.py
+-rw-r--r--   0        0        0     6041 2020-02-02 00:00:00.000000 skshift-0.1.4/tests/test_explanationshift.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 skshift-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 skshift-0.1.4/LICENSE
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 skshift-0.1.4/README.md
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 skshift-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 skshift-0.1.4/PKG-INFO
```

### Comparing `skshift-0.1.3/HowTo.md` & `skshift-0.1.4/HowTo.md`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/tutorial.py` & `skshift-0.1.4/tutorial.py`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/docs/Makefile` & `skshift-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/docs/make.bat` & `skshift-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/docs/source/conf.py` & `skshift-0.1.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/docs/source/explanationTutorial.rst` & `skshift-0.1.4/docs/source/explanationTutorial.rst`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/docs/source/index.rst` & `skshift-0.1.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/docs/source/installation.rst` & `skshift-0.1.4/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/docs/source/images/breastShapGlobal.png` & `skshift-0.1.4/docs/source/images/breastShapGlobal.png`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/docs/source/images/breastShapLocal.png` & `skshift-0.1.4/docs/source/images/breastShapLocal.png`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/docs/source/images/folksShapLocal.png` & `skshift-0.1.4/docs/source/images/folksShapLocal.png`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/docs/source/images/folksShapLocalMI.png` & `skshift-0.1.4/docs/source/images/folksShapLocalMI.png`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/docs/source/images/folkstShapGlobal.png` & `skshift-0.1.4/docs/source/images/folkstShapGlobal.png`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/docs/source/images/folkstShapGlobalMI.png` & `skshift-0.1.4/docs/source/images/folkstShapGlobalMI.png`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/skshift/audits.py` & `skshift-0.1.4/skshift/audits.py`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/skshift/distributionshift.py` & `skshift-0.1.4/tests/test_audit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,154 +1,187 @@
-from sklearn.base import BaseEstimator, ClassifierMixin
-from sklearn.utils.validation import check_X_y, check_is_fitted
+from skshift import ExplanationAudit
+
+from sklearn.ensemble import GradientBoostingClassifier, GradientBoostingRegressor
+from sklearn.linear_model import LogisticRegression, LinearRegression
+from sklearn.model_selection import train_test_split
+from sklearn.datasets import make_blobs
 import pandas as pd
-import shap
+import numpy as np
+
+
+X, y = make_blobs(n_samples=1000, centers=2, n_features=5, random_state=0)
+X = pd.DataFrame(X, columns=["a", "b", "c", "d", "e"])
+# Protected att
+X["a"] = np.where(X["a"] > X["a"].mean(), 1, 0)
+X_tr, X_te, y_tr, y_te = train_test_split(X, y, test_size=0.5, random_state=0)
+
+
+def test_get_splits():
+    detector = ExplanationAudit(
+        model=GradientBoostingRegressor(), gmodel=LogisticRegression()
+    )
+    N = 1000
+    X, y = make_blobs(n_samples=N, centers=2, n_features=5, random_state=0)
+    X = pd.DataFrame(X, columns=["a", "b", "c", "d", "e"])
+    # Binarize
+    X["a"] = np.where(X["a"] > X["a"].mean(), 1, 0)
+
+    detector.get_split_data(X, y, Z="a", n1=0.6, n2=0.5)
+    assert detector.X_tr.shape == (N * 0.4, 5)
+    assert detector.X_val.shape == (N * 0.6 * 0.5, 5)
+    assert detector.X_te.shape == (N * 0.6 * 0.5, 5)
 
+    assert len(set(detector.y_tr)) > 1
+    assert len(set(detector.y_val)) > 1
+    assert len(set(detector.y_te)) > 1
 
-class ExplanationShiftDetector(BaseEstimator, ClassifierMixin):
+
+def test_return_shapDF():
+    """
+    If X is dataframe, return shap values as dataframe.
     """
-    Given a model, and two datasets (source,test), we want to know if the behaviour of the model is different bt train and test.
-    We can do this by computing the shap values of the model on the two datasets, and then train a classifier to distinguish between the two datasets.
+    XX = pd.DataFrame(X, columns=["a", "b", "c", "d", "e"])
 
-    Example
-    -------
-    >>> from sklearn.model_selection import train_test_split
-    >>> from sklearn.datasets import make_blobs
-    >>> from skshift import ExplanationShiftDetector
-    >>> from xgboost import XGBRegressor
-    >>> from sklearn.linear_model import LogisticRegression
-
-    >>> X, y = make_blobs(n_samples=2000, centers=2, n_features=5, random_state=0)
-    >>> X_tr, X_te, y_tr, y_te = train_test_split(X, y, test_size=0.5, random_state=0)
-    >>> X_ood,y_ood = make_blobs(n_samples=1000, centers=1, n_features=5, random_state=0)
-
-    >>> detector = ExplanationShiftDetector(model=XGBRegressor(),gmodel=LogisticRegression())
-    >>> detector.fit(X_tr, y_tr, X_ood)
-    >>> detector.get_auc_val()
-    # 0.76
-    >>> detector.fit(X_tr, y_tr, X_te)
-    >>> detector.get_auc_val()
-    # 0.5
-    """
-
-    def __init__(
-        self,
-        model,
-        gmodel,
-        algorithm: str = "auto",
-        masker: bool = False,
-        data_masker: pd.DataFrame = None,
-    ):
-        """
-        Parameters
-        ----------
-        model : sklearn model
-            Model to be used to compute the shap values.
-        gmodel : sklearn model
-            Model to be used to distinguish between the two datasets.
-        space : str, optional
-            Space in which the gmodel is learned. Can be 'explanation' or 'input' or 'predictions'. Default is 'explanation'.
-
-        algorithm : "auto", "permutation", "partition", "tree", or "linear"
-                The algorithm used to estimate the Shapley values. There are many different algorithms that
-                can be used to estimate the Shapley values (and the related value for constrained games), each
-                of these algorithms have various tradeoffs and are preferrable in different situations. By
-                default the "auto" options attempts to make the best choice given the passed model and masker,
-                but this choice can always be overriden by passing the name of a specific algorithm. The type of
-                algorithm used will determine what type of subclass object is returned by this constructor, and
-                you can also build those subclasses directly if you prefer or need more fine grained control over
-                their options.
-
-        masker : bool,
-                The masker object is used to define the background distribution over which the Shapley values
-                are estimated. Is a boolean that indicates if the masker should be used or not. If True, the masker is used.
-                If False, the masker is not used. The background distribution is the same distribution as we are calculating the Shapley values.
-                TODO Decide which masker distribution is better to use, options are: train data, hold out data, ood data
-        """
-
-        self.model = model
-        self.detector = gmodel
-        self.explainer = None
-        self.algorithm = algorithm
-        self.masker = masker
-        self.data_masker = data_masker
-
-    def fit_detector(self, X, X_ood):
-        try:
-            check_is_fitted(self.model)
-        except:
-            raise ValueError(
-                "Model is not fitted yet, to use this method the model must be fitted."
-            )
+    esd = ExplanationAudit(model=LinearRegression(), gmodel=LogisticRegression())
+    esd.fit_model(XX, y)
+    ex = esd.get_explanations(XX)
+    assert all([a == b for a, b in zip(ex.columns, XX.columns)])
 
-        # Get explanations
-        S_val = self.get_explanations(X)
-        S_ood = self.get_explanations(X_ood)
-
-        # Create dataset for  explanation shift detector
-        S_val["label"] = False
-        S_ood["label"] = True
-
-        S = pd.concat([S_val, S_ood])
-        self.S = S
-
-        self.fit_explanation_shift(S.drop(columns="label"), S["label"])
-
-    def fit_pipeline(self, X, y, X_te, X_ood):
-        """
-        1. Fits the model F to X and y
-        2. Call fit_detector to fit the explanation shift detector
-        """
-        check_X_y(X, y)
-        self.model.fit(X, y)
-        self.fit_detector(X_te, X_ood)
-
-    def fit(self, X_source, y_source, X_ood):
-        """
-        Automatically fits the whole pipeline
-        """
-        self.fit_pipeline(X_source, y_source, X_source, X_ood)
-
-    def predict(self, X):
-        """
-        Returns the predictions (ID,OOD) of the detector on the data X.
-        """
-        return self.detector.predict(self.get_explanations(X))
-
-    def predict_proba(self, X):
-        """
-        Returns the soft predictions (ID,OOD) of the detector on the data X.
-        """
-        return self.detector.predict_proba(self.get_explanations(X))
-
-    def fit_explanation_shift(self, X, y):
-        """
-        Fits the explanation shift detector to the data.
-        """
-        check_X_y(X, y)
-        self.detector.fit(X, y)
-
-    def get_explanations(self, X):
-        """
-        Returns the explanations of the model on the data X.
-        Produces a dataframe with the explanations of the model on the data X.
-        """
-        if self.masker:
-            self.explainer = shap.Explainer(
-                self.model, algorithm=self.algorithm, masker=self.data_masker
+
+def test_supported_models():
+    """
+    Check that models are supported.
+    """
+    for model in [GradientBoostingRegressor(), LogisticRegression()]:
+        for gmodel in [GradientBoostingClassifier(), LogisticRegression()]:
+            assert (
+                type(ExplanationAudit(model=model, gmodel=gmodel)) is ExplanationAudit
             )
-        else:
-            self.explainer = shap.Explainer(self.model, algorithm=self.algorithm)
 
-        shap_values = self.explainer(X)
-        # Name columns
-        if isinstance(X, pd.DataFrame):
-            columns_name = X.columns
-        else:
-            columns_name = ["Shap%d" % (i + 1) for i in range(X.shape[1])]
-
-        exp = pd.DataFrame(
-            data=shap_values.values,
-            columns=columns_name,
-        )
 
-        return exp
+def test_not_supported_models():
+    """
+    Check that models are not supported.
+    """
+
+    from sklearn.neural_network import MLPClassifier
+    import pytest
+
+    with pytest.raises(ValueError):
+        ExplanationAudit(model=MLPClassifier(), gmodel=LogisticRegression())
+    with pytest.raises(ValueError):
+        ExplanationAudit(model=LinearRegression(), gmodel=MLPClassifier())
+
+
+def test_get_model_types():
+    """
+    Check that the model types are returned correctly.
+    """
+    from sklearn.pipeline import Pipeline
+    from sklearn.preprocessing import StandardScaler
+
+    esd = ExplanationAudit(model=LinearRegression(), gmodel=LogisticRegression())
+    assert esd.get_gmodel_type(), esd.get_model_type() == ("linear", "linear")
+    # Case of pipeline
+    esd = ExplanationAudit(
+        model=Pipeline([("scaler", StandardScaler()), ("lr", LinearRegression())]),
+        gmodel=Pipeline([("scaler", StandardScaler()), ("lr", LogisticRegression())]),
+    )
+    assert esd.get_gmodel_type(), esd.get_model_type() == ("linear", "linear")
+
+
+def test_no_nan():
+    """
+    Check that no NaNs are present in the shap values.
+    """
+    esd = ExplanationAudit(model=LinearRegression(), gmodel=LogisticRegression())
+    esd.fit_model(X, y)
+    ex = esd.get_explanations(X)
+    assert not np.any(np.isnan(ex))
+
+
+def test_get_coefs_linear():
+    """
+    Check that the coefficients are returned correctly for the linear regression.
+    """
+    esd = ExplanationAudit(model=LinearRegression(), gmodel=LogisticRegression())
+    esd.fit(X, y, Z="a")
+    coefs = esd.get_linear_coefs()
+    # Assert shape -1 from protected attribute
+    assert len(coefs) == X.shape[1] - 1
+    # Assert that there is non NaNs
+    assert not np.any(np.isnan(coefs))
+    # Check when we call the full methods
+    coefs = esd.get_coefs()
+    # Assert shape -1 from protected attribute
+    assert len(coefs) == X.shape[1] - 1
+    # Assert that there is non NaNs
+    assert not np.any(np.isnan(coefs))
+
+
+def test_get_coefs_pipeline():
+    """
+    Check that the coefficients are returned correctly for the linear regression pipeline.
+    TODO : add a test for the case of a pipeline for F.
+    """
+    from sklearn.pipeline import Pipeline
+    from sklearn.preprocessing import StandardScaler
+
+    esd = ExplanationAudit(
+        model=LinearRegression(),
+        gmodel=Pipeline([("scaler", StandardScaler()), ("lr", LogisticRegression())]),
+    )
+    esd.fit(X, y, Z="a")
+    coefs = esd.get_coefs()
+    # Assert shape -1 from protected attribute
+    assert coefs.shape[1] == X.shape[1] - 1
+    # Assert that there is non NaNs
+    assert not np.any(np.isnan(coefs))
+
+
+def test_predict_drop_prottected():
+    """
+    Check that the protected attribute is dropped when predicting.
+    """
+    audit = ExplanationAudit(
+        model=GradientBoostingRegressor(), gmodel=LogisticRegression()
+    )
+
+    audit.fit(X, y, Z="a")
+    assert np.isnan(audit.predict(X)).sum() == 0
+    assert np.isnan(audit.predict_proba(X)).sum() == 0
+
+
+'''
+def test_doc_examples():
+    """
+    Check that doc examples work.
+    WARNING: this test takes a long time to run. (1-5mins)
+    """
+    from folktables import ACSDataSource, ACSIncome
+
+    data_source = ACSDataSource(survey_year="2014", horizon="1-Year", survey="person")
+    try:
+        acs_data = data_source.get_data(states=["CA"], download=False)
+    except:
+        acs_data = data_source.get_data(states=["CA"], download=True)
+
+    X_, y_, _ = ACSIncome.df_to_numpy(acs_data)
+    X_ = pd.DataFrame(X_, columns=ACSIncome.features)
+
+    # White vs ALL
+    X_["RAC1P"] = np.where(X_["RAC1P"] == 1, 1, 0)
+
+    detector = ExplanationAudit(
+        model=GradientBoostingRegressor(random_state=0), gmodel=LogisticRegression()
+    )
+
+    detector.fit(X_, y_, Z="RAC1P")
+    # Check that the model prediction works
+    assert np.round(detector.get_auc_val(), decimals=1) == 0.7
+    # Check that the coefficients are returned correctly
+    coefs = detector.get_coefs()
+    assert len(coefs) == X_.shape[1] - 1  # -1 for the protected attribute
+    assert np.isnan(coefs).sum() == 0
+    # Hard coded results.
+    # assert np.round(coefs,decimals=0) ==[ 1., -2., -1.,  1., -0., 17.,  2., -0.,  1.]
+'''
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `skshift-0.1.3/tests/test_audit.py` & `skshift-0.1.4/tests/test_explanationshift.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,187 +1,191 @@
-from skshift import ExplanationAudit
+from skshift import ExplanationShiftDetector
 
-from sklearn.ensemble import GradientBoostingClassifier, GradientBoostingRegressor
+
+from xgboost import XGBClassifier, XGBRegressor
 from sklearn.linear_model import LogisticRegression, LinearRegression
 from sklearn.model_selection import train_test_split
 from sklearn.datasets import make_blobs
 import pandas as pd
 import numpy as np
+import pdb
 
 
-X, y = make_blobs(n_samples=1000, centers=2, n_features=5, random_state=0)
-X = pd.DataFrame(X, columns=["a", "b", "c", "d", "e"])
-# Protected att
-X["a"] = np.where(X["a"] > X["a"].mean(), 1, 0)
+X, y = make_blobs(n_samples=2000, centers=2, n_features=5, random_state=0)
 X_tr, X_te, y_tr, y_te = train_test_split(X, y, test_size=0.5, random_state=0)
-
-
-def test_get_splits():
-    detector = ExplanationAudit(
-        model=GradientBoostingRegressor(), gmodel=LogisticRegression()
-    )
-    N = 1000
-    X, y = make_blobs(n_samples=N, centers=2, n_features=5, random_state=0)
-    X = pd.DataFrame(X, columns=["a", "b", "c", "d", "e"])
-    # Binarize
-    X["a"] = np.where(X["a"] > X["a"].mean(), 1, 0)
-
-    detector.get_split_data(X, y, Z="a", n1=0.6, n2=0.5)
-    assert detector.X_tr.shape == (N * 0.4, 5)
-    assert detector.X_val.shape == (N * 0.6 * 0.5, 5)
-    assert detector.X_te.shape == (N * 0.6 * 0.5, 5)
-
-    assert len(set(detector.y_tr)) > 1
-    assert len(set(detector.y_val)) > 1
-    assert len(set(detector.y_te)) > 1
+X_ood, y_ood = make_blobs(n_samples=1000, centers=1, n_features=5, random_state=0)
 
 
 def test_return_shapDF():
     """
     If X is dataframe, return shap values as dataframe.
     """
     XX = pd.DataFrame(X, columns=["a", "b", "c", "d", "e"])
+    XX_ood = pd.DataFrame(X_ood, columns=["a", "b", "c", "d", "e"])
 
-    esd = ExplanationAudit(model=LinearRegression(), gmodel=LogisticRegression())
-    esd.fit_model(XX, y)
+    esd = ExplanationShiftDetector(
+        model=LogisticRegression(), gmodel=LogisticRegression(), masker=True
+    )
+    esd.fit(XX, y, XX_ood)
     ex = esd.get_explanations(XX)
     assert all([a == b for a, b in zip(ex.columns, XX.columns)])
 
 
-def test_supported_models():
-    """
-    Check that models are supported.
-    """
-    for model in [GradientBoostingRegressor(), LogisticRegression()]:
-        for gmodel in [GradientBoostingClassifier(), LogisticRegression()]:
-            assert (
-                type(ExplanationAudit(model=model, gmodel=gmodel)) is ExplanationAudit
-            )
-
-
-def test_not_supported_models():
-    """
-    Check that models are not supported.
-    """
-
-    from sklearn.neural_network import MLPClassifier
-    import pytest
-
-    with pytest.raises(ValueError):
-        ExplanationAudit(model=MLPClassifier(), gmodel=LogisticRegression())
-    with pytest.raises(ValueError):
-        ExplanationAudit(model=LinearRegression(), gmodel=MLPClassifier())
-
-
-def test_get_model_types():
+def test_doc_examples():
     """
-    Check that the model types are returned correctly.
+    Check that doc examples work.
     """
-    from sklearn.pipeline import Pipeline
-    from sklearn.preprocessing import StandardScaler
 
-    esd = ExplanationAudit(model=LinearRegression(), gmodel=LogisticRegression())
-    assert esd.get_gmodel_type(), esd.get_model_type() == ("linear", "linear")
-    # Case of pipeline
-    esd = ExplanationAudit(
-        model=Pipeline([("scaler", StandardScaler()), ("lr", LinearRegression())]),
-        gmodel=Pipeline([("scaler", StandardScaler()), ("lr", LogisticRegression())]),
+    detector = ExplanationShiftDetector(
+        model=XGBRegressor(random_state=0), gmodel=LogisticRegression()
     )
-    assert esd.get_gmodel_type(), esd.get_model_type() == ("linear", "linear")
+    # On OOD
+    detector.fit(X_source=X_tr, y_source=y_tr, X_ood=X_ood)
+    assert np.round(detector.get_auc_val(), decimals=2) == 0.77
+    # On test
+    detector.fit(X_source=X_tr, y_source=y_tr, X_ood=X_te)
+    assert np.round(detector.get_auc_val(), decimals=2) == 0.53
 
 
 def test_no_nan():
     """
     Check that no NaNs are present in the shap values.
     """
-    esd = ExplanationAudit(model=LinearRegression(), gmodel=LogisticRegression())
-    esd.fit_model(X, y)
+    esd = ExplanationShiftDetector(model=XGBClassifier(), gmodel=XGBClassifier())
+    esd.fit(X, y, X_ood)
     ex = esd.get_explanations(X)
     assert not np.any(np.isnan(ex))
 
 
 def test_get_coefs_linear():
     """
     Check that the coefficients are returned correctly for the linear regression.
     """
-    esd = ExplanationAudit(model=LinearRegression(), gmodel=LogisticRegression())
-    esd.fit(X, y, Z="a")
+    esd = ExplanationShiftDetector(
+        model=LinearRegression(), gmodel=LogisticRegression(), masker=True
+    )
+    esd.fit(X, y, X_ood)
     coefs = esd.get_linear_coefs()
-    # Assert shape -1 from protected attribute
-    assert len(coefs) == X.shape[1] - 1
+    # Assert shape
+    assert coefs.shape[1] == X.shape[1]
     # Assert that there is non NaNs
     assert not np.any(np.isnan(coefs))
     # Check when we call the full methods
     coefs = esd.get_coefs()
-    # Assert shape -1 from protected attribute
-    assert len(coefs) == X.shape[1] - 1
+    # Assert shape
+    assert coefs.shape[1] == X.shape[1]
     # Assert that there is non NaNs
     assert not np.any(np.isnan(coefs))
 
 
 def test_get_coefs_pipeline():
     """
     Check that the coefficients are returned correctly for the linear regression pipeline.
     TODO : add a test for the case of a pipeline for F.
     """
     from sklearn.pipeline import Pipeline
     from sklearn.preprocessing import StandardScaler
 
-    esd = ExplanationAudit(
+    esd = ExplanationShiftDetector(
         model=LinearRegression(),
         gmodel=Pipeline([("scaler", StandardScaler()), ("lr", LogisticRegression())]),
+        masker=True,
     )
-    esd.fit(X, y, Z="a")
+    esd.fit(X_tr, y_tr, X_ood)
     coefs = esd.get_coefs()
-    # Assert shape -1 from protected attribute
-    assert coefs.shape[1] == X.shape[1] - 1
+    # Assert shape
+    assert coefs.shape[1] == X.shape[1]
     # Assert that there is non NaNs
     assert not np.any(np.isnan(coefs))
 
 
-def test_predict_drop_prottected():
+def test_get_model_types():
+    """
+    Check that the model types are returned correctly.
+    """
+    from sklearn.pipeline import Pipeline
+    from sklearn.preprocessing import StandardScaler
+
+    esd = ExplanationShiftDetector(
+        model=LinearRegression(), gmodel=LogisticRegression(), masker=X
+    )
+    assert esd.get_gmodel_type(), esd.get_model_type() == ("linear", "linear")
+    # Case of pipeline
+    esd = ExplanationShiftDetector(
+        model=Pipeline([("scaler", StandardScaler()), ("lr", LinearRegression())]),
+        gmodel=Pipeline([("scaler", StandardScaler()), ("lr", LogisticRegression())]),
+    )
+    assert esd.get_gmodel_type(), esd.get_model_type() == ("linear", "linear")
+
+
+def test_spaces():
     """
-    Check that the protected attribute is dropped when predicting.
+    Check that the spaces are returned correctly.
     """
-    audit = ExplanationAudit(
-        model=GradientBoostingRegressor(), gmodel=LogisticRegression()
+
+    esd = ExplanationShiftDetector(
+        model=LinearRegression(),
+        gmodel=LogisticRegression(),
+        space="input",
+        masker=True,
+    )
+    esd.fit(X_tr, y_tr, X_ood)
+    # Check if returns input space
+    # assert esd.get_explanations(X) == X
+    np.testing.assert_array_equal(esd.get_explanations(X), X)
+    # Check if returns output space
+    esd = ExplanationShiftDetector(
+        model=LogisticRegression(),
+        gmodel=LogisticRegression(),
+        space="prediction",
+        masker=True,
+    )
+    esd.fit(X, y, X_ood)
+    np.testing.assert_array_equal(
+        esd.get_explanations(X).shape,
+        pd.DataFrame(data=esd.model.predict(X), columns=["preds"]).shape,
     )
 
-    audit.fit(X, y, Z="a")
-    assert np.isnan(audit.predict(X)).sum() == 0
-    assert np.isnan(audit.predict_proba(X)).sum() == 0
+    # Check if returns exp space
+    esd = ExplanationShiftDetector(
+        model=LinearRegression(),
+        gmodel=LogisticRegression(),
+        space="explanation",
+        masker=True,
+    )
+    esd.fit(X, y, X_ood)
 
+    np.testing.assert_array_equal(esd.get_explanations(X).shape, X.shape)
 
-'''
-def test_doc_examples():
+
+def test_tree_shap():
     """
-    Check that doc examples work.
-    WARNING: this test takes a long time to run. (1-5mins)
+    Check that the shap values are returned correctly for the tree models.
     """
-    from folktables import ACSDataSource, ACSIncome
+    esd = ExplanationShiftDetector(
+        model=XGBRegressor(), gmodel=LogisticRegression(), masker=True
+    )
+    esd.fit(X, y, X_ood)
+    shap_values = esd.get_explanations(X)
+    # Assert shape
+    assert shap_values.shape[1] == X.shape[1]
+    # Assert that there is non NaNs
+    assert not np.any(np.isnan(shap_values))
+
+    esd = ExplanationShiftDetector(model=XGBRegressor(), gmodel=LogisticRegression())
+    esd.fit(X, y, X_ood)
+    shap_values2 = esd.get_explanations(X)
+    # Assert shape
+    assert shap_values2.shape[1] == X.shape[1]
+    # Assert that there is non NaNs
+    assert not np.any(np.isnan(shap_values2))
+    # Assert that the shap values are different depending on the masker
+    assert shap_values2.sum(axis=1).sum(axis=0) != shap_values.sum(axis=1).sum(axis=0)
+
 
-    data_source = ACSDataSource(survey_year="2014", horizon="1-Year", survey="person")
-    try:
-        acs_data = data_source.get_data(states=["CA"], download=False)
-    except:
-        acs_data = data_source.get_data(states=["CA"], download=True)
-
-    X_, y_, _ = ACSIncome.df_to_numpy(acs_data)
-    X_ = pd.DataFrame(X_, columns=ACSIncome.features)
-
-    # White vs ALL
-    X_["RAC1P"] = np.where(X_["RAC1P"] == 1, 1, 0)
-
-    detector = ExplanationAudit(
-        model=GradientBoostingRegressor(random_state=0), gmodel=LogisticRegression()
-    )
-
-    detector.fit(X_, y_, Z="RAC1P")
-    # Check that the model prediction works
-    assert np.round(detector.get_auc_val(), decimals=1) == 0.7
-    # Check that the coefficients are returned correctly
-    coefs = detector.get_coefs()
-    assert len(coefs) == X_.shape[1] - 1  # -1 for the protected attribute
-    assert np.isnan(coefs).sum() == 0
-    # Hard coded results.
-    # assert np.round(coefs,decimals=0) ==[ 1., -2., -1.,  1., -0., 17.,  2., -0.,  1.]
-'''
+def test_explain_detector():
+    for space in ["input", "prediction", "explanation"]:
+        esd = ExplanationShiftDetector(
+            model=XGBClassifier(), gmodel=XGBClassifier(), space=space
+        )
+        esd.fit(X, y, X_ood)
+        esd.explain_detector()
```

### Comparing `skshift-0.1.3/tests/test_explanationShift2.py` & `skshift-0.1.4/tests/test_explanationShift2.py`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/.gitignore` & `skshift-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/LICENSE` & `skshift-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `skshift-0.1.3/pyproject.toml` & `skshift-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "skshift"
-version = "0.01.3"
+version = "0.01.4"
 authors = [
   { name="Carlos Mougan", email="carmougan@gmail.com" },
 ]
 description = "Explanation Shift"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `skshift-0.1.3/PKG-INFO` & `skshift-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skshift
-Version: 0.1.3
+Version: 0.1.4
 Summary: Explanation Shift
 Project-URL: Homepage, https://github.com/cmougan/skshift
 Project-URL: Bug Tracker, https://github.com/cmougan/skshift/issues
 Author-email: Carlos Mougan <carmougan@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carlos Mougan
```

