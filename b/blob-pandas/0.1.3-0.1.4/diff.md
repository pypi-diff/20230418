# Comparing `tmp/blob_pandas-0.1.3.tar.gz` & `tmp/blob_pandas-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blob_pandas-0.1.3.tar", max compression
+gzip compressed data, was "blob_pandas-0.1.4.tar", max compression
```

## Comparing `blob_pandas-0.1.3.tar` & `blob_pandas-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      900 2023-04-18 09:29:54.707218 blob_pandas-0.1.3/LICENSE
--rw-r--r--   0        0        0      209 2023-04-18 09:29:54.707218 blob_pandas-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-18 09:29:54.707218 blob_pandas-0.1.3/blobpandas/__init__.py
--rw-r--r--   0        0        0       22 2023-04-18 09:29:54.707218 blob_pandas-0.1.3/blobpandas/__version__.py
--rw-r--r--   0        0        0     3379 2023-04-18 09:29:54.707218 blob_pandas-0.1.3/blobpandas/blob_io.py
--rw-r--r--   0        0        0     2082 2023-04-18 09:29:54.708218 blob_pandas-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 blob_pandas-0.1.3/setup.py
--rw-r--r--   0        0        0     1039 1970-01-01 00:00:00.000000 blob_pandas-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      900 2023-04-18 09:34:07.447672 blob_pandas-0.1.4/LICENSE
+-rw-r--r--   0        0        0      209 2023-04-18 09:34:07.448673 blob_pandas-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 09:34:07.448673 blob_pandas-0.1.4/blob_pandas/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-18 09:34:07.448673 blob_pandas-0.1.4/blob_pandas/__version__.py
+-rw-r--r--   0        0        0     3379 2023-04-18 09:34:07.448673 blob_pandas-0.1.4/blob_pandas/blob_io.py
+-rw-r--r--   0        0        0     2084 2023-04-18 09:34:07.449673 blob_pandas-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 blob_pandas-0.1.4/setup.py
+-rw-r--r--   0        0        0     1039 1970-01-01 00:00:00.000000 blob_pandas-0.1.4/PKG-INFO
```

### Comparing `blob_pandas-0.1.3/LICENSE` & `blob_pandas-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `blob_pandas-0.1.3/blobpandas/blob_io.py` & `blob_pandas-0.1.4/blob_pandas/blob_io.py`

 * *Files identical despite different names*

### Comparing `blob_pandas-0.1.3/pyproject.toml` & `blob_pandas-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "blob-pandas"
-version = "0.1.3"
+version = "0.1.4"
 description = "Classes and utils to communicate with Azure Blob Storage through pandas DataFrames"
 authors = ["Mattia Tantardini <mattia.tantardini@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/tantardini/blob-pandas"
 keywords = ["utils", "azure-blob-storage"]
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
 ]
-packages = [{include = "blobpandas"}]
+packages = [{include = "blob_pandas"}]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -59,15 +59,15 @@
     ["disabled", "fg:#858585 italic"]
 ]
 
 # --- Semantic release --- #
 [tool.semantic_release]
 # Reference: https://python-semantic-release.readthedocs.io/en/latest/index.html
 version_variable = [
-    "blobpandas/__version__.py:__version__",
+    "blob_pandas/__version__.py:__version__",
     "pyproject.toml:version"
 ]
 branch = "main"
 hvcs = "gitlab"
 tag_format = "v{version}"
 build_command = ""
 upload_to_pypi = false
```

### Comparing `blob_pandas-0.1.3/setup.py` & `blob_pandas-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['blobpandas']
+['blob_pandas']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['azure-storage-blob>=12.16.0,<13.0.0', 'pandas>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'blob-pandas',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Classes and utils to communicate with Azure Blob Storage through pandas DataFrames',
     'long_description': '# blob-pandas\nClasses and utils to communicate with Azure Blob Storage through pandas DataFrames.\n\n## Installation\n```\npip install blob-pandas\n```\n\n## Usage\nDescribe how to launch and use blob-pandas project.\n',
     'author': 'Mattia Tantardini',
     'author_email': 'mattia.tantardini@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/tantardini/blob-pandas',
```

### Comparing `blob_pandas-0.1.3/PKG-INFO` & `blob_pandas-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blob-pandas
-Version: 0.1.3
+Version: 0.1.4
 Summary: Classes and utils to communicate with Azure Blob Storage through pandas DataFrames
 Home-page: https://gitlab.com/tantardini/blob-pandas
 Keywords: utils,azure-blob-storage
 Author: Mattia Tantardini
 Author-email: mattia.tantardini@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
```

