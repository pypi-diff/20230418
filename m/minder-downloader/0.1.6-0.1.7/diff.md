# Comparing `tmp/minder_downloader-0.1.6.tar.gz` & `tmp/minder_downloader-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minder_downloader-0.1.6.tar", max compression
+gzip compressed data, was "minder_downloader-0.1.7.tar", max compression
```

## Comparing `minder_downloader-0.1.6.tar` & `minder_downloader-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2296 2023-03-13 06:58:21.238849 minder_downloader-0.1.6/README.md
--rw-r--r--   0        0        0      140 2023-04-04 19:54:51.041491 minder_downloader-0.1.6/minder_downloader/__init__.py
--rw-r--r--   0        0        0      154 2023-04-14 12:14:07.094370 minder_downloader-0.1.6/minder_downloader/__version__.py
--rw-r--r--   0        0        0     1482 2023-04-14 04:55:03.024070 minder_downloader-0.1.6/minder_downloader/config.py
--rw-r--r--   0        0        0     9556 2023-04-14 12:07:46.275779 minder_downloader-0.1.6/minder_downloader/download.py
--rw-r--r--   0        0        0     2279 2023-04-14 07:08:52.609588 minder_downloader-0.1.6/minder_downloader/info.py
--rw-r--r--   0        0        0      419 2023-03-13 11:49:39.589041 minder_downloader-0.1.6/minder_downloader/update.py
--rw-r--r--   0        0        0     1081 2023-04-08 03:48:59.591442 minder_downloader-0.1.6/minder_downloader/upload.py
--rw-r--r--   0        0        0     5586 2023-04-08 03:49:16.155397 minder_downloader-0.1.6/minder_downloader/utils.py
--rw-r--r--   0        0        0      548 2023-04-14 12:14:18.975793 minder_downloader-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 minder_downloader-0.1.6/setup.py
--rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 minder_downloader-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2296 2023-03-13 06:58:21.238849 minder_downloader-0.1.7/README.md
+-rw-r--r--   0        0        0      140 2023-04-04 19:54:51.041491 minder_downloader-0.1.7/minder_downloader/__init__.py
+-rw-r--r--   0        0        0      154 2023-04-18 06:43:58.210176 minder_downloader-0.1.7/minder_downloader/__version__.py
+-rw-r--r--   0        0        0     2176 2023-04-18 06:41:56.332419 minder_downloader-0.1.7/minder_downloader/config.py
+-rw-r--r--   0        0        0     9556 2023-04-14 12:07:46.275779 minder_downloader-0.1.7/minder_downloader/download.py
+-rw-r--r--   0        0        0     2279 2023-04-14 07:08:52.609588 minder_downloader-0.1.7/minder_downloader/info.py
+-rw-r--r--   0        0        0      419 2023-03-13 11:49:39.589041 minder_downloader-0.1.7/minder_downloader/update.py
+-rw-r--r--   0        0        0     1081 2023-04-08 03:48:59.591442 minder_downloader-0.1.7/minder_downloader/upload.py
+-rw-r--r--   0        0        0     5586 2023-04-08 03:49:16.155397 minder_downloader-0.1.7/minder_downloader/utils.py
+-rw-r--r--   0        0        0      548 2023-04-18 06:44:01.232789 minder_downloader-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 minder_downloader-0.1.7/setup.py
+-rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 minder_downloader-0.1.7/PKG-INFO
```

### Comparing `minder_downloader-0.1.6/README.md` & `minder_downloader-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `minder_downloader-0.1.6/minder_downloader/download.py` & `minder_downloader-0.1.7/minder_downloader/download.py`

 * *Files identical despite different names*

### Comparing `minder_downloader-0.1.6/minder_downloader/info.py` & `minder_downloader-0.1.7/minder_downloader/info.py`

 * *Files identical despite different names*

### Comparing `minder_downloader-0.1.6/minder_downloader/upload.py` & `minder_downloader-0.1.7/minder_downloader/upload.py`

 * *Files identical despite different names*

### Comparing `minder_downloader-0.1.6/minder_downloader/utils.py` & `minder_downloader-0.1.7/minder_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `minder_downloader-0.1.6/pyproject.toml` & `minder_downloader-0.1.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "minder-downloader"
-version = "0.1.06"
+version = "0.1.07"
 description = "The minder-downloader module provides a simple interface for downloading datasets and uploading reports using the Minder research portal."
 authors = ["Dr Eyal Soreq <eyal.soreq@ukdri.ac.uk>"]
 readme = "README.md"
 packages = [{include = "minder_downloader"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `minder_downloader-0.1.6/setup.py` & `minder_downloader-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'pandas>=1.5,<2.0',
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.65.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'minder-downloader',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'The minder-downloader module provides a simple interface for downloading datasets and uploading reports using the Minder research portal.',
     'long_description': "# Minder Downloader\nThe minder-downloader module is a Python package that provides a user-friendly interface for interacting with the Minder research portal. This package enables users to easily download datasets from the Minder research portal, as well as upload reports to the platform.\n\nThe downloading functionality of the package is straightforward to use. The module handles the authentication and request/response handling, so the user doesn't need to worry about the details of these processes. Once authenticated, users can specify the date range and datasets to download, and the module will return the data as a Pandas DataFrame. This makes it easy to work with the data using Python's powerful data analysis tools.\n\nIn addition to downloading data, the minder-downloader module also provides a simple way to upload reports to the Minder research portal. This can be done by providing the path to a file and the HTML address to upload the file to. The module takes care of the uploading process, making it easy to share reports with collaborators or the wider research community.\n\nOverall, the minder-downloader package provides a convenient and streamlined way to interact with the Minder research portal, whether you need to download data or upload reports.\n\n## Installation\nYou can install minder-downloader using pip:\n\n```bash\npip install minder-downloader\n```\n\n## Usage\nHere is a simple example of how to use minder-downloader to download data from the Minder research portal:\n\n```python\nfrom datetime import datetime, timedelta\nfrom minder_downloader import MinderDatasetDownload\n\n# Define date range and datasets to download\nsince = datetime.now() - timedelta(days=7)\nuntil = datetime.now()\ndatasets = ['example_dataset_1', 'example_dataset_2']\n\n# Create downloader object and download data\ndownloader = MinderDatasetDownload(since, until, datasets)\ndata = downloader.download_data()\n\n# Print downloaded data\nprint(data.head())\n```\n\nThis will download the specified datasets for the past week and print the first few rows of the resulting DataFrame.\n\n## License\nminder-downloader is licensed under the MIT License. See the LICENSE file for details.\n\n## Acknowledgements\nThis module was created by Dr Eyal Soreq. If you find it useful, please consider citing it in your research.",
     'author': 'Dr Eyal Soreq',
     'author_email': 'eyal.soreq@ukdri.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `minder_downloader-0.1.6/PKG-INFO` & `minder_downloader-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minder-downloader
-Version: 0.1.6
+Version: 0.1.7
 Summary: The minder-downloader module provides a simple interface for downloading datasets and uploading reports using the Minder research portal.
 Author: Dr Eyal Soreq
 Author-email: eyal.soreq@ukdri.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

