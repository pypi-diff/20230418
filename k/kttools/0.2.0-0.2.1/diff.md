# Comparing `tmp/kttools-0.2.0.tar.gz` & `tmp/kttools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kttools-0.2.0.tar", max compression
+gzip compressed data, was "kttools-0.2.1.tar", max compression
```

## Comparing `kttools-0.2.0.tar` & `kttools-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-12 06:12:13.687609 kttools-0.2.0/LICENSE
--rw-r--r--   0        0        0     1538 2023-04-12 06:12:13.687609 kttools-0.2.0/README.rst
--rw-r--r--   0        0        0     1084 2023-04-12 06:12:13.687609 kttools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      457 2023-04-12 06:12:13.687609 kttools-0.2.0/tools/__init__.py
--rw-r--r--   0        0        0      366 2023-04-12 06:12:13.687609 kttools-0.2.0/tools/sc/__init__.py
--rw-r--r--   0        0        0    12358 2023-04-12 06:12:13.687609 kttools-0.2.0/tools/sc/_sc.py
--rw-r--r--   0        0        0      429 2023-04-12 06:12:13.687609 kttools-0.2.0/tools/tools/__init__.py
--rw-r--r--   0        0        0     8879 2023-04-12 06:12:13.687609 kttools-0.2.0/tools/tools/_tools.py
--rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 kttools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-18 05:39:37.706567 kttools-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1538 2023-04-18 05:39:37.706567 kttools-0.2.1/README.rst
+-rw-r--r--   0        0        0     1090 2023-04-18 05:39:37.706567 kttools-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      457 2023-04-18 05:39:37.706567 kttools-0.2.1/tools/__init__.py
+-rw-r--r--   0        0        0      366 2023-04-18 05:39:37.706567 kttools-0.2.1/tools/sc/__init__.py
+-rw-r--r--   0        0        0    12358 2023-04-18 05:39:37.710567 kttools-0.2.1/tools/sc/_sc.py
+-rw-r--r--   0        0        0      429 2023-04-18 05:39:37.710567 kttools-0.2.1/tools/tools/__init__.py
+-rw-r--r--   0        0        0     8879 2023-04-18 05:39:37.710567 kttools-0.2.1/tools/tools/_tools.py
+-rw-r--r--   0        0        0     2611 1970-01-01 00:00:00.000000 kttools-0.2.1/PKG-INFO
```

### Comparing `kttools-0.2.0/LICENSE` & `kttools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kttools-0.2.0/README.rst` & `kttools-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `kttools-0.2.0/pyproject.toml` & `kttools-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "kttools"
-version = "0.2.0"
+version = "0.2.1"
 description = "Kelvin's miscellaneous tools for python"
 authors = ["Zewen Kelvin Tuong <z.tuong@uq.edu.au>"]
 license = "MIT"
 readme = "README.rst"
 classifiers = [
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Programming Language :: Python :: 3',
 ]
 packages = [{ include = "tools" }]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-pandas = "^1.2.4"
-numpy = "^1.21.6"
-matplotlib = "^3.5.2"
-scanpy = "^1.7.1"
-anndata = "^0.7.6"
+python = ">=3.8"
+pandas = ">=1.2.4"
+numpy = ">=1.21.6"
+matplotlib = ">=3.5.2"
+scanpy = ">=1.7.1"
+anndata = ">=0.7.6"
 sphinx-autodoc-typehints = { optional = true, version = "*" }
 sphinx_rtd_theme = { optional = true, version = "*" }
 readthedocs-sphinx-ext = { optional = true, version = "*" }
 recommonmark = { optional = true, version = "*" }
 
 [tool.poetry.extras]
 docs = [
```

### Comparing `kttools-0.2.0/tools/sc/_sc.py` & `kttools-0.2.1/tools/sc/_sc.py`

 * *Files identical despite different names*

### Comparing `kttools-0.2.0/tools/tools/_tools.py` & `kttools-0.2.1/tools/tools/_tools.py`

 * *Files identical despite different names*

### Comparing `kttools-0.2.0/PKG-INFO` & `kttools-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: kttools
-Version: 0.2.0
+Version: 0.2.1
 Summary: Kelvin's miscellaneous tools for python
 License: MIT
 Author: Zewen Kelvin Tuong
 Author-email: z.tuong@uq.edu.au
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: docs
-Requires-Dist: anndata (>=0.7.6,<0.8.0)
-Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
-Requires-Dist: numpy (>=1.21.6,<2.0.0)
-Requires-Dist: pandas (>=1.2.4,<2.0.0)
+Requires-Dist: anndata (>=0.7.6)
+Requires-Dist: matplotlib (>=3.5.2)
+Requires-Dist: numpy (>=1.21.6)
+Requires-Dist: pandas (>=1.2.4)
 Requires-Dist: readthedocs-sphinx-ext ; extra == "docs"
 Requires-Dist: recommonmark ; extra == "docs"
-Requires-Dist: scanpy (>=1.7.1,<2.0.0)
+Requires-Dist: scanpy (>=1.7.1)
 Requires-Dist: sphinx-autodoc-typehints ; extra == "docs"
 Requires-Dist: sphinx_rtd_theme ; extra == "docs"
 Description-Content-Type: text/x-rst
 
 |Docs| |PyPI|
 
 kttools
```

