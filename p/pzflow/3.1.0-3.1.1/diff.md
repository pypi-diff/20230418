# Comparing `tmp/pzflow-3.1.0.tar.gz` & `tmp/pzflow-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pzflow-3.1.0.tar", max compression
+gzip compressed data, was "pzflow-3.1.1.tar", max compression
```

## Comparing `pzflow-3.1.0.tar` & `pzflow-3.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1079 2023-04-06 21:13:39.820423 pzflow-3.1.0/LICENSE
--rw-r--r--   0        0        0     3018 2023-04-06 21:13:39.823423 pzflow-3.1.0/README.md
--rw-r--r--   0        0        0     1293 2023-04-12 19:35:47.784964 pzflow-3.1.0/pyproject.toml
--rw-r--r--   0        0        0      135 2023-04-12 19:35:47.786965 pzflow-3.1.0/pzflow/__init__.py
--rw-r--r--   0        0        0    29958 2023-04-06 21:13:39.927422 pzflow-3.1.0/pzflow/bijectors.py
--rw-r--r--   0        0        0    18084 2023-04-11 18:20:35.939054 pzflow-3.1.0/pzflow/distributions.py
--rw-r--r--   0        0        0   800708 2023-04-06 21:13:39.948422 pzflow-3.1.0/pzflow/example_files/checkerboard-data.pkl
--rw-r--r--   0        0        0  2219977 2023-04-06 21:13:39.991422 pzflow-3.1.0/pzflow/example_files/city-data.pkl
--rw-r--r--   0        0        0  1158452 2023-04-06 21:13:40.016421 pzflow-3.1.0/pzflow/example_files/example-flow.pzflow.pkl
--rw-r--r--   0        0        0  5600784 2023-04-06 21:13:40.135421 pzflow-3.1.0/pzflow/example_files/galaxy-data.pkl
--rw-r--r--   0        0        0  1600708 2023-04-06 21:13:40.169420 pzflow-3.1.0/pzflow/example_files/two-moons-data.pkl
--rw-r--r--   0        0        0     4847 2023-04-06 21:13:40.172420 pzflow-3.1.0/pzflow/examples.py
--rw-r--r--   0        0        0    45183 2023-04-12 19:35:47.793964 pzflow-3.1.0/pzflow/flow.py
--rw-r--r--   0        0        0    25652 2023-04-12 19:35:47.798964 pzflow-3.1.0/pzflow/flowEnsemble.py
--rw-r--r--   0        0        0     8206 2023-04-11 20:07:53.618947 pzflow-3.1.0/pzflow/utils.py
--rw-r--r--   0        0        0     3902 2023-04-13 19:05:29.602088 pzflow-3.1.0/setup.py
--rw-r--r--   0        0        0     3821 2023-04-13 19:05:29.602379 pzflow-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-04-06 21:13:39.820423 pzflow-3.1.1/LICENSE
+-rw-r--r--   0        0        0     3018 2023-04-06 21:13:39.823423 pzflow-3.1.1/README.md
+-rw-r--r--   0        0        0     1293 2023-04-18 21:19:54.807356 pzflow-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-04-18 21:19:54.815357 pzflow-3.1.1/pzflow/__init__.py
+-rw-r--r--   0        0        0    29958 2023-04-06 21:13:39.927422 pzflow-3.1.1/pzflow/bijectors.py
+-rw-r--r--   0        0        0    18084 2023-04-18 21:19:54.821356 pzflow-3.1.1/pzflow/distributions.py
+-rw-r--r--   0        0        0   800708 2023-04-06 21:13:39.948422 pzflow-3.1.1/pzflow/example_files/checkerboard-data.pkl
+-rw-r--r--   0        0        0  2219977 2023-04-06 21:13:39.991422 pzflow-3.1.1/pzflow/example_files/city-data.pkl
+-rw-r--r--   0        0        0  1158452 2023-04-06 21:13:40.016421 pzflow-3.1.1/pzflow/example_files/example-flow.pzflow.pkl
+-rw-r--r--   0        0        0  5600784 2023-04-06 21:13:40.135421 pzflow-3.1.1/pzflow/example_files/galaxy-data.pkl
+-rw-r--r--   0        0        0  1600708 2023-04-06 21:13:40.169420 pzflow-3.1.1/pzflow/example_files/two-moons-data.pkl
+-rw-r--r--   0        0        0     4847 2023-04-06 21:13:40.172420 pzflow-3.1.1/pzflow/examples.py
+-rw-r--r--   0        0        0    45183 2023-04-12 19:35:47.793964 pzflow-3.1.1/pzflow/flow.py
+-rw-r--r--   0        0        0    25652 2023-04-12 19:35:47.798964 pzflow-3.1.1/pzflow/flowEnsemble.py
+-rw-r--r--   0        0        0     8206 2023-04-11 20:07:53.618947 pzflow-3.1.1/pzflow/utils.py
+-rw-r--r--   0        0        0     3902 2023-04-18 21:20:15.258268 pzflow-3.1.1/setup.py
+-rw-r--r--   0        0        0     3821 2023-04-18 21:20:15.259045 pzflow-3.1.1/PKG-INFO
```

### Comparing `pzflow-3.1.0/LICENSE` & `pzflow-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pzflow-3.1.0/README.md` & `pzflow-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pzflow-3.1.0/pyproject.toml` & `pzflow-3.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pzflow"
-version = "3.1.0"
+version = "3.1.1"
 description = "Probabilistic modeling of tabular data with normalizing flows."
 authors = ["John Franklin Crenshaw <jfcrenshaw@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/jfcrenshaw/pzflow"
 readme = "README.md"
```

### Comparing `pzflow-3.1.0/pzflow/bijectors.py` & `pzflow-3.1.1/pzflow/bijectors.py`

 * *Files identical despite different names*

### Comparing `pzflow-3.1.0/pzflow/distributions.py` & `pzflow-3.1.1/pzflow/distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
             The distribution has support (-B, B) along each dimension.
         """
         self.input_dim = input_dim
         self.B = B
 
         # save dist info
         self._params = tuple([(0.0, 0.0) for i in range(input_dim)])
-        self.info = ("CentBeta22", (input_dim, B))
+        self.info = ("CentBeta13", (input_dim, B))
         self.a = 13
         self.b = 13
 
     def log_prob(self, params: Pytree, inputs: jnp.ndarray) -> jnp.ndarray:
         """Calculates log probability density of inputs.
 
         Parameters
```

### Comparing `pzflow-3.1.0/pzflow/example_files/checkerboard-data.pkl` & `pzflow-3.1.1/pzflow/example_files/checkerboard-data.pkl`

 * *Files identical despite different names*

### Comparing `pzflow-3.1.0/pzflow/example_files/city-data.pkl` & `pzflow-3.1.1/pzflow/example_files/city-data.pkl`

 * *Files identical despite different names*

### Comparing `pzflow-3.1.0/pzflow/example_files/example-flow.pzflow.pkl` & `pzflow-3.1.1/pzflow/example_files/example-flow.pzflow.pkl`

 * *Files identical despite different names*

### Comparing `pzflow-3.1.0/pzflow/example_files/galaxy-data.pkl` & `pzflow-3.1.1/pzflow/example_files/galaxy-data.pkl`

 * *Files identical despite different names*

### Comparing `pzflow-3.1.0/pzflow/example_files/two-moons-data.pkl` & `pzflow-3.1.1/pzflow/example_files/two-moons-data.pkl`

 * *Files identical despite different names*

### Comparing `pzflow-3.1.0/pzflow/examples.py` & `pzflow-3.1.1/pzflow/examples.py`

 * *Files identical despite different names*

### Comparing `pzflow-3.1.0/pzflow/flow.py` & `pzflow-3.1.1/pzflow/flow.py`

 * *Files identical despite different names*

### Comparing `pzflow-3.1.0/pzflow/flowEnsemble.py` & `pzflow-3.1.1/pzflow/flowEnsemble.py`

 * *Files identical despite different names*

### Comparing `pzflow-3.1.0/pzflow/utils.py` & `pzflow-3.1.1/pzflow/utils.py`

 * *Files identical despite different names*

### Comparing `pzflow-3.1.0/setup.py` & `pzflow-3.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'jaxlib>=0.4.2,<0.5.0',
  'optax>=0.1.4,<0.2.0',
  'pandas>=1.1',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'pzflow',
-    'version': '3.1.0',
+    'version': '3.1.1',
     'description': 'Probabilistic modeling of tabular data with normalizing flows.',
     'long_description': '![build](https://github.com/jfcrenshaw/pzflow/workflows/build/badge.svg)\n[![codecov](https://codecov.io/gh/jfcrenshaw/pzflow/branch/main/graph/badge.svg?token=qR5cey0swQ)](https://codecov.io/gh/jfcrenshaw/pzflow)\n[![PyPI version](https://badge.fury.io/py/pzflow.svg)](https://badge.fury.io/py/pzflow)\n[![DOI](https://zenodo.org/badge/327498448.svg)](https://zenodo.org/badge/latestdoi/327498448)\n[![Docs](https://img.shields.io/badge/Docs-https%3A%2F%2Fjfcrenshaw.github.io%2Fpzflow%2F-red)](https://jfcrenshaw.github.io/pzflow/)\n\n# PZFlow\n\nPZFlow is a python package for probabilistic modeling of tabular data with normalizing flows.\n\nIf your data consists of continuous variables that can be put into a Pandas DataFrame, pzflow can model the joint probability distribution of your data set.\n\nThe `Flow` class makes building and training a normalizing flow simple.\nIt also allows you to easily sample from the normalizing flow (e.g., for forward modeling or data augmentation), and calculate posteriors over any of your variables.\n\nThere are several tutorial notebooks in the [docs](https://jfcrenshaw.github.io/pzflow/tutorials/).\n\n## Installation\n\nSee the instructions in the [docs](https://jfcrenshaw.github.io/pzflow/install/).\n\n## Citation\n\nWe are preparing a paper on pzflow.\nIf you use this package in your research, please check back here for a citation before publication.\nIn the meantime, please cite the [Zenodo release](https://zenodo.org/badge/latestdoi/327498448).\n\n### Sources\n\nPZFlow was originally designed for forward modeling of photometric redshifts as a part of the Creation Module of the [DESC](https://lsstdesc.org/) [RAIL](https://github.com/LSSTDESC/RAIL) project.\nThe idea to use normalizing flows for photometric redshifts originated with [Bryce Kalmbach](https://github.com/jbkalmbach).\nThe earliest version of the normalizing flow in RAIL was based on a notebook by [Francois Lanusse](https://github.com/eiffl) and included contributions from [Alex Malz](https://github.com/aimalz).\n\nThe functional jax structure of the bijectors was originally based on [`jax-flows`](https://github.com/ChrisWaites/jax-flows) by [Chris Waites](https://github.com/ChrisWaites). The implementation of the Neural Spline Coupling is largely based on the [Tensorflow implementation](https://github.com/tensorflow/probability/blob/master/tensorflow_probability/python/bijectors/rational_quadratic_spline.py), with some inspiration from [`nflows`](https://github.com/bayesiains/nflows/).\n\nNeural Spline Flows are based on the following papers:\n\n  > [NICE: Non-linear Independent Components Estimation](https://arxiv.org/abs/1410.8516)\\\n  > Laurent Dinh, David Krueger, Yoshua Bengio\\\n  > _arXiv:1410.8516_\n\n  > [Density estimation using Real NVP](https://arxiv.org/abs/1605.08803)\\\n  > Laurent Dinh, Jascha Sohl-Dickstein, Samy Bengio\\\n  > _arXiv:1605.08803_\n\n  > [Neural Spline Flows](https://arxiv.org/abs/1906.04032)\\\n  > Conor Durkan, Artur Bekasov, Iain Murray, George Papamakarios\\\n  > _arXiv:1906.04032_\n',
     'author': 'John Franklin Crenshaw',
     'author_email': 'jfcrenshaw@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/jfcrenshaw/pzflow',
```

### Comparing `pzflow-3.1.0/PKG-INFO` & `pzflow-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pzflow
-Version: 3.1.0
+Version: 3.1.1
 Summary: Probabilistic modeling of tabular data with normalizing flows.
 Home-page: https://github.com/jfcrenshaw/pzflow
 License: MIT
 Author: John Franklin Crenshaw
 Author-email: jfcrenshaw@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

