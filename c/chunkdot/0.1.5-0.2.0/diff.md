# Comparing `tmp/chunkdot-0.1.5.tar.gz` & `tmp/chunkdot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chunkdot-0.1.5.tar", max compression
+gzip compressed data, was "chunkdot-0.2.0.tar", max compression
```

## Comparing `chunkdot-0.1.5.tar` & `chunkdot-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1129 2023-03-31 03:15:29.624003 chunkdot-0.1.5/README.md
--rw-r--r--   0        0        0      131 2023-04-10 13:20:40.268489 chunkdot-0.1.5/chunkdot/__init__.py
--rw-r--r--   0        0        0     3251 2023-03-28 22:49:05.870063 chunkdot-0.1.5/chunkdot/chunkdot.py
--rw-r--r--   0        0        0     3212 2023-03-31 06:43:23.566757 chunkdot-0.1.5/chunkdot/cosine_similarity_top_k.py
--rw-r--r--   0        0        0     4094 2023-03-08 12:19:56.965969 chunkdot-0.1.5/chunkdot/numba_argpartition.py
--rw-r--r--   0        0        0     3964 2023-03-31 03:01:38.405020 chunkdot-0.1.5/chunkdot/utils.py
--rw-r--r--   0        0        0     1002 2023-04-10 13:20:39.585166 chunkdot-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 chunkdot-0.1.5/setup.py
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 chunkdot-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2072 2023-04-18 03:25:54.010872 chunkdot-0.2.0/README.md
+-rw-r--r--   0        0        0      131 2023-04-18 03:26:21.827168 chunkdot-0.2.0/chunkdot/__init__.py
+-rw-r--r--   0        0        0     2364 2023-04-18 03:25:54.012135 chunkdot-0.2.0/chunkdot/chunkdot.py
+-rw-r--r--   0        0        0     7094 2023-04-18 03:25:54.013225 chunkdot-0.2.0/chunkdot/chunkdot_sparse.py
+-rw-r--r--   0        0        0     3693 2023-04-18 03:25:54.014044 chunkdot-0.2.0/chunkdot/cosine_similarity_top_k.py
+-rw-r--r--   0        0        0     4094 2023-03-08 12:19:56.965969 chunkdot-0.2.0/chunkdot/numba_argpartition.py
+-rw-r--r--   0        0        0     4700 2023-04-18 03:25:54.015437 chunkdot-0.2.0/chunkdot/utils.py
+-rw-r--r--   0        0        0     1115 2023-04-18 03:26:20.821419 chunkdot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 chunkdot-0.2.0/PKG-INFO
```

### Comparing `chunkdot-0.1.5/README.md` & `chunkdot-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 ## Usage
 
 ```bash
 pip install -U chunkdot
 ```
 
+### Dense embeddings
+
 Calculate the 50 most similar and dissimilar items for 100K items.
 
 ```python
 import numpy as np
 from chunkdot import cosine_similarity_top_k
 
 embeddings = np.random.randn(100000, 256)
@@ -21,20 +23,52 @@
 cosine_similarity_top_k(embeddings, top_k=-50, max_memory=20E9)
 ```
 ```
 <100000x100000 sparse matrix of type '<class 'numpy.float64'>'
  with 5000000 stored elements in Compressed Sparse Row format>
 ```
 
-## The execution time
-
+Execution time
 ```python
 from timeit import timeit
 import numpy as np
 from chunkdot import cosine_similarity_top_k
 
 embeddings = np.random.randn(100000, 256)
 timeit(lambda: cosine_similarity_top_k(embeddings, top_k=50, max_memory=20E9), number=1)
 ```
 ```
 58.611996899999994
 ```
+
+### Sparse embeddings
+
+Calculate the 50 most similar and dissimilar items for 100K items. Items represented by 10K dimensional vectors and an embeddings matrix of 0.005 density.
+
+```python
+from scipy import sparse
+from chunkdot import cosine_similarity_top_k
+
+embeddings = sparse.rand(100000, 10000, density=0.005)
+# using all you system's memory
+cosine_similarity_top_k(embeddings, top_k=50)
+# most dissimilar items using 20GB
+cosine_similarity_top_k(embeddings, top_k=-50, max_memory=20E9)
+```
+```
+<100000x100000 sparse matrix of type '<class 'numpy.float64'>'
+ with 5000000 stored elements in Compressed Sparse Row format>
+```
+
+Execution time
+
+```python
+from timeit import timeit
+from scipy import sparse
+from chunkdot import cosine_similarity_top_k
+
+embeddings = sparse.rand(100000, 10000, density=0.005)
+timeit(lambda: cosine_similarity_top_k(embeddings, top_k=50, max_memory=20E9), number=1)
+```
+```
+51.87472256699999
+```
```

### Comparing `chunkdot-0.1.5/chunkdot/cosine_similarity_top_k.py` & `chunkdot-0.2.0/chunkdot/cosine_similarity_top_k.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import numpy as np
-from scipy.sparse import issparse
+from scipy import sparse
 from chunkdot.chunkdot import chunkdot
+from chunkdot.chunkdot_sparse import chunkdot_sparse
 from chunkdot.utils import get_chunk_size_per_thread
 
 
 def cosine_similarity_top_k(
     embeddings: np.ndarray,
     top_k: int,
     normalize: bool = True,
     max_memory: int = None,
     force_memory: bool = False,
 ):
     """Calculate cosine similarity and only keep the K most similar items for each item.
 
     Args:
-        embeddings (np.array): 2D array containing the items embeddings. Array of size
-            number of items x embedding dimension.
+        embeddings (np.array or scipy.sparse matrix): 2D object containing the items embeddings,
+            of shape number of items x embedding dimension.
         top_k (int): The amount of similar items per item to return.
         normalize (bool): If to apply L2-norm to each row.
             Default True.
         max_memory (int): Maximum amount of memory to use in bytes. If None it will use the
             available memory to the system according to chunkdot.utils.get_memory_available.
             Default None.
         force_memory (bool): Use max_memory even if it is bigger than the memory
@@ -42,32 +43,41 @@
         3. Parallelize the matrix multiplication using a separate piece in each thread.
         4. Per thread:
             a. Matrix multiplication between the piece and the embeddings matrix transposed.
             b. Extract the values and column indices of the most similar K items per row.
             c. Collect such values and column indices into outer scope arrays.
         5. Create a CSR matrix from all values and indices and return it.
     """
-    if issparse(embeddings):
-        raise TypeError("ChunkDot does not yet support SciPy sparse matrices as input.")
-
     # return type consistent with sklearn.pairwise.cosine_similarity function
     return_type = "float32" if embeddings.dtype == np.float32 else "float64"
+    embeddings = embeddings.astype(return_type)
     if normalize:
-        embeddings = (
-            embeddings
-            / np.sqrt(np.einsum("ij,ij->i", embeddings, embeddings, dtype=return_type))[
-                :, np.newaxis
-            ]
-        )
+        if sparse.issparse(embeddings):
+            norms = sparse.linalg.norm(embeddings, ord=2, axis=1)
+            norms[norms == 0] = np.inf
+            embeddings = sparse.diags(1 / norms) @ embeddings
+        else:
+            norms = np.linalg.norm(embeddings, ord=2, axis=1, keepdims=True)
+            embeddings = np.divide(
+                embeddings,
+                norms,
+                out=np.zeros_like(embeddings, dtype=return_type),
+                where=norms != 0,
+            )
 
-    n_rows = len(embeddings)
+    n_rows = embeddings.shape[0]
     abs_top_k = abs(top_k)
 
     if abs_top_k >= n_rows:
         raise ValueError(
             f"The number of requested similar items (top_k={abs_top_k}) must be less than the "
-            f"total number of items (len(embeddings)={len(embeddings)})"
+            f"total number of items (embeddings.shape[0]={n_rows})"
         )
 
     chunk_size_per_thread = get_chunk_size_per_thread(n_rows, abs_top_k, max_memory, force_memory)
-    similarities = chunkdot(embeddings, embeddings.T, top_k, chunk_size_per_thread, return_type)
+    if sparse.issparse(embeddings):
+        similarities = chunkdot_sparse(
+            embeddings, embeddings.T, top_k, chunk_size_per_thread, return_type
+        )
+    else:
+        similarities = chunkdot(embeddings, embeddings.T, top_k, chunk_size_per_thread, return_type)
     return similarities
```

### Comparing `chunkdot-0.1.5/chunkdot/numba_argpartition.py` & `chunkdot-0.2.0/chunkdot/numba_argpartition.py`

 * *Files identical despite different names*

### Comparing `chunkdot-0.1.5/chunkdot/utils.py` & `chunkdot-0.2.0/chunkdot/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,39 @@
 import logging
 import math
 import warnings
 import psutil
 import numba
+from numba import njit
 import numpy as np
-from chunkdot.chunkdot import chunkdot
-
+from chunkdot import numba_argpartition  # pylint: disable=unused-import
 
 LOGGER = logging.getLogger(__name__)
 
 
+# Noting to parallelize in this function. It will raise an error if setting parallel to True since
+# the calling functions are already being parallelized.
+@njit(parallel=False)
+def to_sparse(matrix, top_k, values, indices):
+    """Get the values and column indices of the biggest K elements per row.
+
+    The function will return the data and indices according with the CSR matrix convention. The
+    indptr values are calculated outside the parallelization of this function.
+    """
+    # This line creates a new array with the same shape as "matrix" effectively doubling the
+    # memory consumption.
+    top_k_j = np.argpartition(matrix, -top_k)
+    if top_k > 0:
+        top_k_j = top_k_j[:, -top_k:]
+    else:
+        top_k_j = top_k_j[:, :-top_k]
+    values[:] = np.take_along_axis(matrix, top_k_j, axis=1).flatten()
+    indices[:] = top_k_j.flatten()
+
+
 def get_memory_available():
     """Get the available memory to the OS.
 
     https://psutil.readthedocs.io/en/latest/#psutil.virtual_memory
 
     The memory that can be given instantly to processes without the system going into swap. This
     is calculated by summing different memory values depending on the platform and it is supposed
@@ -23,20 +43,14 @@
     available memory on that process, as memory could have been used in the Python process
     and released for further use in the same Python process but not back to the OS even if it has
     been garbage collected.
     """
     return psutil.virtual_memory().available
 
 
-def warm_up_chunked_dot():
-    """Make a dummy run of the "chunkdot" function to compile it."""
-    matrix = np.random.randn(10000, 100)
-    chunkdot(matrix, matrix.T, 10, 5000)
-
-
 def get_chunk_size_per_thread(n_items, top_k, max_memory=None, force_memory=False):
     """Calculate the maximum row size of a matrix for a given memory threshold.
 
     This calculation is very specific to the cosine_similarity_top_k algorithm. Given the total
     number of items, the amount of similar items requested, the number of parallel threads to
     execute and the memory threshold to consume, calculate the maximum number of rows to process
     on each thread.
```

### Comparing `chunkdot-0.1.5/pyproject.toml` & `chunkdot-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chunkdot"
-version = "0.1.5"
+version = "0.2.0"
 description = "Multi-threaded matrix multiplication and cosine similarity calculations."
 authors = ["Rodrigo Agundez <rragundez@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/rragundez/chunkdot"
 classifiers = [
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
@@ -31,14 +31,21 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
 
+[tool.pytest.ini_options]
+addopts = "-x --log-cli-level=INFO"
+testpaths = [
+    "tests",
+]
+
 [tool.pylint.messages_control]
 max-line-length = 100
 max-args = 10
 disable = [
   "missing-module-docstring",
   "logging-fstring-interpolation",
+  "too-many-locals",
 ]
```

### Comparing `chunkdot-0.1.5/setup.py` & `chunkdot-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,97 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: chunkdot
+Version: 0.2.0
+Summary: Multi-threaded matrix multiplication and cosine similarity calculations.
+Home-page: https://github.com/rragundez/chunkdot
+Author: Rodrigo Agundez
+Author-email: rragundez@gmail.com
+Requires-Python: >=3.8,<3.11
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development
+Requires-Dist: numba (>=0.56.4,<0.57.0)
+Requires-Dist: numpy (>=1.23,<2.0)
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
+Project-URL: Repository, https://github.com/rragundez/chunkdot
+Description-Content-Type: text/markdown
+
+# ChunkDot
+
+Multi-threaded matrix multiplication and cosine similarity calculations. Appropriate for the calculation of the K most similar items for a large number of items (~1 Million) by partitioning the item matrix representation (embeddings) and using Numba to accelerate the calculations.
+
+## Usage
+
+```bash
+pip install -U chunkdot
+```
+
+### Dense embeddings
+
+Calculate the 50 most similar and dissimilar items for 100K items.
+
+```python
+import numpy as np
+from chunkdot import cosine_similarity_top_k
+
+embeddings = np.random.randn(100000, 256)
+# using all you system's memory
+cosine_similarity_top_k(embeddings, top_k=50)
+# most dissimilar items using 20GB
+cosine_similarity_top_k(embeddings, top_k=-50, max_memory=20E9)
+```
+```
+<100000x100000 sparse matrix of type '<class 'numpy.float64'>'
+ with 5000000 stored elements in Compressed Sparse Row format>
+```
+
+Execution time
+```python
+from timeit import timeit
+import numpy as np
+from chunkdot import cosine_similarity_top_k
+
+embeddings = np.random.randn(100000, 256)
+timeit(lambda: cosine_similarity_top_k(embeddings, top_k=50, max_memory=20E9), number=1)
+```
+```
+58.611996899999994
+```
+
+### Sparse embeddings
+
+Calculate the 50 most similar and dissimilar items for 100K items. Items represented by 10K dimensional vectors and an embeddings matrix of 0.005 density.
+
+```python
+from scipy import sparse
+from chunkdot import cosine_similarity_top_k
+
+embeddings = sparse.rand(100000, 10000, density=0.005)
+# using all you system's memory
+cosine_similarity_top_k(embeddings, top_k=50)
+# most dissimilar items using 20GB
+cosine_similarity_top_k(embeddings, top_k=-50, max_memory=20E9)
+```
+```
+<100000x100000 sparse matrix of type '<class 'numpy.float64'>'
+ with 5000000 stored elements in Compressed Sparse Row format>
+```
+
+Execution time
+
+```python
+from timeit import timeit
+from scipy import sparse
+from chunkdot import cosine_similarity_top_k
+
+embeddings = sparse.rand(100000, 10000, density=0.005)
+timeit(lambda: cosine_similarity_top_k(embeddings, top_k=50, max_memory=20E9), number=1)
+```
+```
+51.87472256699999
+```
 
-packages = \
-['chunkdot']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['numba>=0.56.4,<0.57.0', 'numpy>=1.23,<2.0', 'scipy>=1.10.1,<2.0.0']
-
-setup_kwargs = {
-    'name': 'chunkdot',
-    'version': '0.1.5',
-    'description': 'Multi-threaded matrix multiplication and cosine similarity calculations.',
-    'long_description': "# ChunkDot\n\nMulti-threaded matrix multiplication and cosine similarity calculations. Appropriate for the calculation of the K most similar items for a large number of items (~1 Million) by partitioning the item matrix representation (embeddings) and using Numba to accelerate the calculations.\n\n## Usage\n\n```bash\npip install -U chunkdot\n```\n\nCalculate the 50 most similar and dissimilar items for 100K items.\n\n```python\nimport numpy as np\nfrom chunkdot import cosine_similarity_top_k\n\nembeddings = np.random.randn(100000, 256)\n# using all you system's memory\ncosine_similarity_top_k(embeddings, top_k=50)\n# most dissimilar items using 20GB\ncosine_similarity_top_k(embeddings, top_k=-50, max_memory=20E9)\n```\n```\n<100000x100000 sparse matrix of type '<class 'numpy.float64'>'\n with 5000000 stored elements in Compressed Sparse Row format>\n```\n\n## The execution time\n\n```python\nfrom timeit import timeit\nimport numpy as np\nfrom chunkdot import cosine_similarity_top_k\n\nembeddings = np.random.randn(100000, 256)\ntimeit(lambda: cosine_similarity_top_k(embeddings, top_k=50, max_memory=20E9), number=1)\n```\n```\n58.611996899999994\n```\n",
-    'author': 'Rodrigo Agundez',
-    'author_email': 'rragundez@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/rragundez/chunkdot',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
-
-
-setup(**setup_kwargs)
```

