# Comparing `tmp/gaussidan-0.1.4.tar.gz` & `tmp/gaussidan-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaussidan-0.1.4.tar", max compression
+gzip compressed data, was "gaussidan-0.1.5.tar", max compression
```

## Comparing `gaussidan-0.1.4.tar` & `gaussidan-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      165 2022-11-01 19:26:52.461536 gaussidan-0.1.4/gaussidan/__init__.py
--rw-r--r--   0        0        0     1069 2022-11-01 19:23:14.934802 gaussidan-0.1.4/gaussidan/fit_gaussian.py
--rw-r--r--   0        0        0      659 2022-08-31 14:03:00.107879 gaussidan-0.1.4/gaussidan/plot_gaussian.py
--rw-r--r--   0        0        0      442 2023-04-18 19:33:34.454022 gaussidan-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      620 2023-04-18 19:33:40.741807 gaussidan-0.1.4/setup.py
--rw-r--r--   0        0        0      482 2023-04-18 19:33:40.742055 gaussidan-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-04-18 19:35:25.640137 gaussidan-0.1.5/gaussidan/__init__.py
+-rw-r--r--   0        0        0     1076 2023-04-18 19:37:26.831552 gaussidan-0.1.5/gaussidan/fit_gaussian.py
+-rw-r--r--   0        0        0      666 2023-04-18 19:37:50.387418 gaussidan-0.1.5/gaussidan/plot_gaussian.py
+-rw-r--r--   0        0        0      442 2023-04-18 19:39:39.166830 gaussidan-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      620 2023-04-18 19:39:44.836307 gaussidan-0.1.5/setup.py
+-rw-r--r--   0        0        0      482 2023-04-18 19:39:44.836551 gaussidan-0.1.5/PKG-INFO
```

### Comparing `gaussidan-0.1.4/gaussidan/fit_gaussian.py` & `gaussidan-0.1.5/gaussidan/fit_gaussian.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Sequence, Union
+from typing import Sequence, Tuple, Union
 
 import numpy as np
 from lmfit.models import GaussianModel
 
 
 def fit_gaussian(
     data: Union[Sequence[float], np.ndarray],
     bins: Union[int, Union[Sequence[float], np.ndarray]],
     weights: Union[Sequence[float], np.ndarray] = None,
     errors: bool = False,
-) -> tuple[float, float, float]:
+) -> Tuple[float, float, float]:
 
     hist, bin_edges = np.histogram(data, bins=bins, weights=weights)
 
     mask = np.nonzero(hist)
     hist = hist[mask]
     bin_centers = (bin_edges[:-1] + bin_edges[1:]) / 2
     bin_centers = bin_centers[mask]
```

### Comparing `gaussidan-0.1.4/gaussidan/plot_gaussian.py` & `gaussidan-0.1.5/gaussidan/plot_gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Sequence, Union
+from typing import Sequence, Tuple, Union
 
 import numpy as np
 from lmfit.models import GaussianModel
 
 from gaussidan import fit_gaussian
 
 
 def plot_gaussian(
     data: Union[Sequence[float], np.ndarray],
     bins: Union[int, Union[Sequence[float], np.ndarray]],
     weights: Union[Sequence[float], np.ndarray] = None,
-) -> tuple[np.ndarray, np.ndarray]:
+) -> Tuple[np.ndarray, np.ndarray]:
 
     height, mu, sigma = fit_gaussian(data, bins, weights)
     _, bin_edges = np.histogram(data, bins=bins, weights=weights)
     bin_centers = (bin_edges[:-1] + bin_edges[1:]) / 2
 
     model = GaussianModel()
     y = model.eval(x=bin_centers, amplitude=height, center=mu, sigma=sigma)
```

### Comparing `gaussidan-0.1.4/setup.py` & `gaussidan-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['lmfit==1.0.2', 'numpy>=1.19.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'gaussidan',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': '',
     'long_description': None,
     'author': 'Daniel Williams',
     'author_email': 'daniel.mays.williams@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

