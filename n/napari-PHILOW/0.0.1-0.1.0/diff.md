# Comparing `tmp/napari-PHILOW-0.0.1.tar.gz` & `tmp/napari-PHILOW-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-PHILOW-0.0.1.tar", last modified: Mon May  2 05:59:56 2022, max compression
+gzip compressed data, was "napari-PHILOW-0.1.0.tar", last modified: Tue Apr 18 02:45:50 2023, max compression
```

## Comparing `napari-PHILOW-0.0.1.tar` & `napari-PHILOW-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,39 @@
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2022-05-02 05:59:56.216220 napari-PHILOW-0.0.1/
--rw-r--r--   0 hiroki     (501) staff       (20)    35148 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/LICENSE
--rw-r--r--   0 hiroki     (501) staff       (20)      121 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/MANIFEST.in
--rw-r--r--   0 hiroki     (501) staff       (20)     8804 2022-05-02 05:59:56.216323 napari-PHILOW-0.0.1/PKG-INFO
--rw-r--r--   0 hiroki     (501) staff       (20)     7915 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/README.md
--rw-r--r--   0 hiroki     (501) staff       (20)      193 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/requirements.txt
--rw-r--r--   0 hiroki     (501) staff       (20)     1121 2022-05-02 05:59:56.217019 napari-PHILOW-0.0.1/setup.cfg
--rw-r--r--   0 hiroki     (501) staff       (20)       84 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/setup.py
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2022-05-02 05:59:56.211037 napari-PHILOW-0.0.1/src/
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2022-05-02 05:59:56.214130 napari-PHILOW-0.0.1/src/napari_PHILOW.egg-info/
--rw-r--r--   0 hiroki     (501) staff       (20)     8804 2022-05-02 05:59:55.000000 napari-PHILOW-0.0.1/src/napari_PHILOW.egg-info/PKG-INFO
--rw-r--r--   0 hiroki     (501) staff       (20)      675 2022-05-02 05:59:56.000000 napari-PHILOW-0.0.1/src/napari_PHILOW.egg-info/SOURCES.txt
--rw-r--r--   0 hiroki     (501) staff       (20)        1 2022-05-02 05:59:55.000000 napari-PHILOW-0.0.1/src/napari_PHILOW.egg-info/dependency_links.txt
--rw-r--r--   0 hiroki     (501) staff       (20)       46 2022-05-02 05:59:55.000000 napari-PHILOW-0.0.1/src/napari_PHILOW.egg-info/entry_points.txt
--rw-r--r--   0 hiroki     (501) staff       (20)      119 2022-05-02 05:59:56.000000 napari-PHILOW-0.0.1/src/napari_PHILOW.egg-info/requires.txt
--rw-r--r--   0 hiroki     (501) staff       (20)       14 2022-05-02 05:59:56.000000 napari-PHILOW-0.0.1/src/napari_PHILOW.egg-info/top_level.txt
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2022-05-02 05:59:56.215745 napari-PHILOW-0.0.1/src/napari_philow/
--rw-r--r--   0 hiroki     (501) staff       (20)      171 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/src/napari_philow/__init__.py
--rw-r--r--   0 hiroki     (501) staff       (20)     8080 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/src/napari_philow/_annotation.py
--rw-r--r--   0 hiroki     (501) staff       (20)     4453 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/src/napari_philow/_data_manager.py
--rw-r--r--   0 hiroki     (501) staff       (20)      328 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/src/napari_philow/_dock_widget.py
--rw-r--r--   0 hiroki     (501) staff       (20)     3797 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/src/napari_philow/_models.py
--rw-r--r--   0 hiroki     (501) staff       (20)     4301 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/src/napari_philow/_predict.py
--rw-r--r--   0 hiroki     (501) staff       (20)     6286 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/src/napari_philow/_prediction.py
-drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2022-05-02 05:59:56.216057 napari-PHILOW-0.0.1/src/napari_philow/_tests/
--rw-r--r--   0 hiroki     (501) staff       (20)        0 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/src/napari_philow/_tests/__init__.py
--rw-r--r--   0 hiroki     (501) staff       (20)      696 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/src/napari_philow/_tests/test_dock_widget.py
--rw-r--r--   0 hiroki     (501) staff       (20)     7643 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/src/napari_philow/_train.py
--rw-r--r--   0 hiroki     (501) staff       (20)    28137 2022-04-25 01:47:53.000000 napari-PHILOW-0.0.1/src/napari_philow/_utils.py
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-18 02:45:50.746918 napari-PHILOW-0.1.0/
+-rw-r--r--   0 hiroki     (501) staff       (20)    35148 2022-04-25 01:47:53.000000 napari-PHILOW-0.1.0/LICENSE
+-rw-r--r--   0 hiroki     (501) staff       (20)       96 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/MANIFEST.in
+-rw-r--r--   0 hiroki     (501) staff       (20)     9297 2023-04-18 02:45:50.747007 napari-PHILOW-0.1.0/PKG-INFO
+-rw-r--r--   0 hiroki     (501) staff       (20)     8024 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/README.md
+-rw-r--r--   0 hiroki     (501) staff       (20)      179 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/pyproject.toml
+-rw-r--r--   0 hiroki     (501) staff       (20)      193 2022-04-25 01:47:53.000000 napari-PHILOW-0.1.0/requirements.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)     1786 2023-04-18 02:45:50.747469 napari-PHILOW-0.1.0/setup.cfg
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-18 02:45:50.741655 napari-PHILOW-0.1.0/src/
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-18 02:45:50.743788 napari-PHILOW-0.1.0/src/napari_PHILOW.egg-info/
+-rw-r--r--   0 hiroki     (501) staff       (20)     9297 2023-04-18 02:45:50.000000 napari-PHILOW-0.1.0/src/napari_PHILOW.egg-info/PKG-INFO
+-rw-r--r--   0 hiroki     (501) staff       (20)     1051 2023-04-18 02:45:50.000000 napari-PHILOW-0.1.0/src/napari_PHILOW.egg-info/SOURCES.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)        1 2023-04-18 02:45:50.000000 napari-PHILOW-0.1.0/src/napari_PHILOW.egg-info/dependency_links.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)       60 2023-04-18 02:45:50.000000 napari-PHILOW-0.1.0/src/napari_PHILOW.egg-info/entry_points.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)      164 2023-04-18 02:45:50.000000 napari-PHILOW-0.1.0/src/napari_PHILOW.egg-info/requires.txt
+-rw-r--r--   0 hiroki     (501) staff       (20)       14 2023-04-18 02:45:50.000000 napari-PHILOW-0.1.0/src/napari_PHILOW.egg-info/top_level.txt
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-18 02:45:50.745407 napari-PHILOW-0.1.0/src/napari_philow/
+-rw-r--r--   0 hiroki     (501) staff       (20)      279 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/__init__.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     7787 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/_annotation.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     4453 2022-04-25 01:47:53.000000 napari-PHILOW-0.1.0/src/napari_philow/_data_manager.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     3975 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/_predict.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     5861 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/_prediction.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     7703 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/_selector.py
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-18 02:45:50.745637 napari-PHILOW-0.1.0/src/napari_philow/_tests/
+-rw-r--r--   0 hiroki     (501) staff       (20)        0 2022-04-25 01:47:53.000000 napari-PHILOW-0.1.0/src/napari_philow/_tests/__init__.py
+-rw-r--r--   0 hiroki     (501) staff       (20)      696 2022-04-25 01:47:53.000000 napari-PHILOW-0.1.0/src/napari_philow/_tests/test_dock_widget.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     7683 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/_train_tf.py
+-rw-r--r--   0 hiroki     (501) staff       (20)    10929 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/_trainer.py
+-rw-r--r--   0 hiroki     (501) staff       (20)    27582 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/_utils.py
+-rw-r--r--   0 hiroki     (501) staff       (20)      799 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/napari.yaml
+drwxr-xr-x   0 hiroki     (501) staff       (20)        0 2023-04-18 02:45:50.746794 napari-PHILOW-0.1.0/src/napari_philow/segmentation/
+-rw-r--r--   0 hiroki     (501) staff       (20)        0 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/segmentation/__init__.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     4526 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/segmentation/data_augmentation.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     2304 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/segmentation/dataset.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     1031 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/segmentation/loss.py
+-rw-r--r--   0 hiroki     (501) staff       (20)      252 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/segmentation/metric.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     2244 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/segmentation/predict.py
+-rw-r--r--   0 hiroki     (501) staff       (20)     5011 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/segmentation/train.py
+-rw-r--r--   0 hiroki     (501) staff       (20)      316 2023-04-18 02:41:23.000000 napari-PHILOW-0.1.0/src/napari_philow/segmentation/utils.py
```

### Comparing `napari-PHILOW-0.0.1/LICENSE` & `napari-PHILOW-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-PHILOW-0.0.1/PKG-INFO` & `napari-PHILOW-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: napari-PHILOW
-Version: 0.0.1
+Version: 0.1.0
 Summary: PHILOW is an interactive deep learning-based platform for 3D datasets
 Home-page: https://github.com/neurobiology-ut/PHILOW
 Author: Hiroki Kawai
 Author-email: h.kawai888@gmail.com
-License: BSD-3-Clause
-Platform: UNKNOWN
+License: GPLv3
+Project-URL: Bug Tracker, https://github.com/neurobiology-ut/PHILOW/issues
+Project-URL: Documentation, https://github.com/neurobiology-ut/PHILOW#README.md
+Project-URL: Source Code, https://github.com/neurobiology-ut/PHILOW
+Project-URL: User Support, https://github.com/neurobiology-ut/PHILOW/issues
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
-Classifier: Topic :: Software Development :: Testing
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 License-File: LICENSE
 
 # napari-PHILOW
 
 [![License](https://img.shields.io/pypi/l/napari-PHILOW.svg?color=green)](https://github.com/neurobiology-ut/PHILOW/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-PHILOW.svg?color=green)](https://pypi.org/project/napari-PHILOW)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-PHILOW.svg?color=green)](https://python.org)
@@ -46,14 +51,17 @@
 
 and review the napari docs for plugin developers:
 https://napari.org/plugins/stable/index.html
 -->
 
 ## Installation
 
+Install napari and Pytorch first.   
+See [napari] and [Pytorch](https://pytorch.org/) for more information.
+
 You can install `napari-PHILOW` via [pip]:
 
     pip install napari-PHILOW
     
 or clone this repository   
 then
 ```angular2
@@ -213,9 +221,7 @@
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
-
```

### Comparing `napari-PHILOW-0.0.1/README.md` & `napari-PHILOW-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 and review the napari docs for plugin developers:
 https://napari.org/plugins/stable/index.html
 -->
 
 ## Installation
 
+Install napari and Pytorch first.   
+See [napari] and [Pytorch](https://pytorch.org/) for more information.
+
 You can install `napari-PHILOW` via [pip]:
 
     pip install napari-PHILOW
     
 or clone this repository   
 then
 ```angular2
```

### Comparing `napari-PHILOW-0.0.1/setup.cfg` & `napari-PHILOW-0.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,70 @@
 [metadata]
 name = napari-PHILOW
-version = 0.0.1
+version = 0.1.0
 author = Hiroki Kawai
 author_email = h.kawai888@gmail.com
 url = https://github.com/neurobiology-ut/PHILOW
-license = BSD-3-Clause
+license = GPLv3
+license_files = LICENSE
 description = PHILOW is an interactive deep learning-based platform for 3D datasets
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
-	Intended Audience :: Developers
 	Framework :: napari
-	Topic :: Software Development :: Testing
+	Intended Audience :: Developers
+	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
-	Operating System :: OS Independent
-	License :: OSI Approved :: BSD License
+	Programming Language :: Python :: 3.10
+	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+	Topic :: Scientific/Engineering :: Image Processing
+project_urls = 
+	Bug Tracker = https://github.com/neurobiology-ut/PHILOW/issues
+	Documentation = https://github.com/neurobiology-ut/PHILOW#README.md
+	Source Code = https://github.com/neurobiology-ut/PHILOW
+	User Support = https://github.com/neurobiology-ut/PHILOW/issues
 
 [options]
 packages = find:
-python_requires = >=3.7
-package_dir = 
-	=src
 install_requires = 
-	napari-plugin-engine>=0.1.4
-	tensorflow
 	numpy
 	scikit-image
 	dask-image
 	opencv-python
 	matplotlib
-	napari-tools-menu
 	pandas
+	torch
+	torchvision
+	segmentation-models-pytorch
+python_requires = >=3.8
+include_package_data = True
+package_dir = 
+	=src
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
-napari.plugin = 
-	napari-PHILOW = napari_philow
+napari.manifest = 
+	napari-PHILOW = napari_philow:napari.yaml
+
+[options.extras_require]
+testing = 
+	tox
+	pytest  # https://docs.pytest.org/en/latest/contents.html
+	pytest-cov  # https://pytest-cov.readthedocs.io/en/latest/
+	pytest-qt  # https://pytest-qt.readthedocs.io/en/latest/
+	napari
+	pyqt5
+
+[options.package_data]
+* = *.yaml
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `napari-PHILOW-0.0.1/src/napari_PHILOW.egg-info/PKG-INFO` & `napari-PHILOW-0.1.0/src/napari_PHILOW.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: napari-PHILOW
-Version: 0.0.1
+Version: 0.1.0
 Summary: PHILOW is an interactive deep learning-based platform for 3D datasets
 Home-page: https://github.com/neurobiology-ut/PHILOW
 Author: Hiroki Kawai
 Author-email: h.kawai888@gmail.com
-License: BSD-3-Clause
-Platform: UNKNOWN
+License: GPLv3
+Project-URL: Bug Tracker, https://github.com/neurobiology-ut/PHILOW/issues
+Project-URL: Documentation, https://github.com/neurobiology-ut/PHILOW#README.md
+Project-URL: Source Code, https://github.com/neurobiology-ut/PHILOW
+Project-URL: User Support, https://github.com/neurobiology-ut/PHILOW/issues
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
-Classifier: Topic :: Software Development :: Testing
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 License-File: LICENSE
 
 # napari-PHILOW
 
 [![License](https://img.shields.io/pypi/l/napari-PHILOW.svg?color=green)](https://github.com/neurobiology-ut/PHILOW/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-PHILOW.svg?color=green)](https://pypi.org/project/napari-PHILOW)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-PHILOW.svg?color=green)](https://python.org)
@@ -46,14 +51,17 @@
 
 and review the napari docs for plugin developers:
 https://napari.org/plugins/stable/index.html
 -->
 
 ## Installation
 
+Install napari and Pytorch first.   
+See [napari] and [Pytorch](https://pytorch.org/) for more information.
+
 You can install `napari-PHILOW` via [pip]:
 
     pip install napari-PHILOW
     
 or clone this repository   
 then
 ```angular2
@@ -213,9 +221,7 @@
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
-
```

### Comparing `napari-PHILOW-0.0.1/src/napari_PHILOW.egg-info/SOURCES.txt` & `napari-PHILOW-0.1.0/src/napari_PHILOW.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.cfg
-setup.py
 src/napari_PHILOW.egg-info/PKG-INFO
 src/napari_PHILOW.egg-info/SOURCES.txt
 src/napari_PHILOW.egg-info/dependency_links.txt
 src/napari_PHILOW.egg-info/entry_points.txt
 src/napari_PHILOW.egg-info/requires.txt
 src/napari_PHILOW.egg-info/top_level.txt
 src/napari_philow/__init__.py
 src/napari_philow/_annotation.py
 src/napari_philow/_data_manager.py
-src/napari_philow/_dock_widget.py
-src/napari_philow/_models.py
 src/napari_philow/_predict.py
 src/napari_philow/_prediction.py
-src/napari_philow/_train.py
+src/napari_philow/_selector.py
+src/napari_philow/_train_tf.py
+src/napari_philow/_trainer.py
 src/napari_philow/_utils.py
+src/napari_philow/napari.yaml
 src/napari_philow/_tests/__init__.py
-src/napari_philow/_tests/test_dock_widget.py
+src/napari_philow/_tests/test_dock_widget.py
+src/napari_philow/segmentation/__init__.py
+src/napari_philow/segmentation/data_augmentation.py
+src/napari_philow/segmentation/dataset.py
+src/napari_philow/segmentation/loss.py
+src/napari_philow/segmentation/metric.py
+src/napari_philow/segmentation/predict.py
+src/napari_philow/segmentation/train.py
+src/napari_philow/segmentation/utils.py
```

### Comparing `napari-PHILOW-0.0.1/src/napari_philow/_annotation.py` & `napari-PHILOW-0.1.0/src/napari_philow/_annotation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import os
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 from magicgui import magicgui
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
+from matplotlib.backends.backend_qtagg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.figure import Figure
 from napari._qt.qthreading import thread_worker
-from napari_tools_menu import register_dock_widget
 from qtpy.QtWidgets import QWidget, QPushButton, QSizePolicy, QLineEdit, QCheckBox, QLabel, QVBoxLayout, QFileDialog
 from scipy import ndimage
 from skimage import io
 
 from napari_philow._data_manager import Datamanager
 from napari_philow._utils import combine_blocks, load_images, load_saved_masks, load_raw_masks, label_ct, \
     label_and_sort, save_masks, crop_img, show_so_layer
 
 
-@register_dock_widget(menu="PHILOW > Annotation mode")
 class AnnotationMode(QWidget):
     def __init__(self, napari_viewer):
         super().__init__()
         self._viewer = napari_viewer
         self.opath = ""
         self.modpath = ""
         self.btn1 = QPushButton('open', self)
@@ -41,14 +39,16 @@
         self.btn4.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
         self.btn4.clicked.connect(self.launch)
         self.lbl = QLabel('original dir', self)
         self.lbl2 = QLabel('mask dir', self)
         self.lbl4 = QLabel('model type (do not use word "train")', self)
         self.build()
 
+        self.filenames = None
+
     def build(self):
         vbox = QVBoxLayout()
         vbox.addWidget(combine_blocks(self.btn1, self.lbl))
         vbox.addWidget(combine_blocks(self.btn2, self.lbl2))
         vbox.addWidget(combine_blocks(self.textbox, self.lbl4))
         vbox.addWidget(self.checkBox)
         vbox.addWidget(self.btn4)
@@ -69,24 +69,25 @@
         if f_name:
             self.modpath = f_name
             self.lbl2.setText(self.modpath)
 
     def launch(self):
         images = load_images(self.opath)
         if self.modpath == "":
-            labels = np.zeros_like(images.compute())
             self.modpath = os.path.join(os.path.dirname(self.opath), self.textbox.text())
             os.makedirs(self.modpath, exist_ok=True)
-            filenames = [fn.name for fn in sorted(list(Path(self.opath).glob('./*png')))]
-            #for i in range(len(labels)):
-            #    io.imsave(os.path.join(self.modpath, str(i).zfill(4) + '.png'), labels[i])
-            for i, filename in enumerate(filenames):
+        else:
+            pass
+        if len(os.listdir(self.modpath)) == 0:
+            labels = np.zeros_like(images.compute())
+            self.filenames = [fn.name for fn in sorted(list(Path(self.opath).glob('./*png')))]
+            for i, filename in enumerate(self.filenames):
                 io.imsave(os.path.join(self.modpath, filename), labels[i])
         else:
-            labels = load_saved_masks(self.modpath)
+            labels, self.filenames = load_saved_masks(self.modpath)
         try:
             labels_raw = load_raw_masks(self.modpath + '_raw')
         except:
             labels_raw = None
         self._viewer.window.remove_dock_widget(self)
         self.launch_anm(images, labels, labels_raw)
 
@@ -115,38 +116,36 @@
 
         @thread_worker(connect={"returned": show_so_layer})
         def create_label(viewer):
             labeled_sorted, nums = label_and_sort(base_label)
             print(nums)
             labeled_c = label_ct(labeled_sorted, nums, 10)
             return labeled_c, labeled_sorted, nums, viewer
+
         if len(np.unique(base_label)) > 1:
             create_label(self._viewer)
 
         layer = self._viewer.layers[0]
         layer1 = self._viewer.layers[1]
 
         @magicgui(dirname={"mode": "d"}, call_button=False)
         def dirpicker(dirname=Path(r_path)):
             """Take a filename and do something with it."""
             print("The filename is:", dirname)
             return dirname
 
-        # gui = dirpicker.Gui(show=True)
         self._viewer.window.add_dock_widget(dirpicker, area='bottom')
 
         @magicgui(call_button="save")
         def saver():
             # out_dir = gui.dirname
             out_dir = dirpicker.dirname.value
             print("The directory is:", out_dir)
-            return save_masks(layer1.data, out_dir)
+            return save_masks(layer1.data, out_dir, self.filenames)
 
-        # gui2 = saver.Gui(show=True)
-        # self._viewer.window.add_dock_widget(gui2, area='bottom')
         self._viewer.window.add_dock_widget(saver, area='bottom')
 
         dmg = Datamanager()
         dmg.prepare(r_path, model_type, checkbox)
         self._viewer.window.add_dock_widget(dmg, area='left')
 
         def update_button(axis_event):
@@ -179,23 +178,21 @@
             zx_axes.scatter(50, 50, s=10, c='red', alpha=0.15)
             zx_axes.set_xlabel('x axis')
             zx_axes.set_ylabel('z axis')
 
             # canvas.figure.tight_layout()
             canvas.figure.subplots_adjust(left=0, bottom=0.1, right=1, top=0.95, wspace=0, hspace=0.4)
 
-        canvas.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Maximum)
-
         self._viewer.window.add_dock_widget(canvas, area='right')
 
         @layer.mouse_drag_callbacks.append
         def update_canvas_canvas(layer, event):
             if 'shift' in event.modifiers:
                 try:
-                    m_point = np.round(layer.position).astype(int)
+                    m_point = np.round(self._viewer.cursor.position).astype(int)
                     print(m_point)
                     crop_big = crop_img([m_point[0], m_point[1], m_point[2]], layer)
                     xy_axes.imshow(crop_big[50], 'gray')
                     yz_axes.imshow(crop_big.transpose(1, 0, 2)[50], 'gray')
                     zx_axes.imshow(crop_big.transpose(2, 0, 1)[50], 'gray')
                     canvas.draw_idle()
                 except Exception as e:
```

### Comparing `napari-PHILOW-0.0.1/src/napari_philow/_data_manager.py` & `napari-PHILOW-0.1.0/src/napari_philow/_data_manager.py`

 * *Files identical despite different names*

### Comparing `napari-PHILOW-0.0.1/src/napari_philow/_prediction.py` & `napari-PHILOW-0.1.0/src/napari_philow/_prediction.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import shutil
 from pathlib import Path
 
 import pandas as pd
-from napari_tools_menu import register_dock_widget
+import torch
 from qtpy.QtWidgets import (QWidget, QVBoxLayout, QPushButton, QSizePolicy, QLabel, QFileDialog,
                             QCheckBox)
+from segmentation_models_pytorch import UnetPlusPlus
+
+from napari_philow._utils import combine_blocks
 
-from napari_philow._models import get_nested_unet
 from napari_philow._predict import predict_3ax, predict_1ax
-from napari_philow._utils import combine_blocks, load_X_gray
 
 
-@register_dock_widget(menu="PHILOW > Prediction mode")
 class Predicter(QWidget):
     def __init__(self):
         super().__init__()
         self.opath = ""
         self.labelpath = ""
         self.modelpath = ""
         self.outpath = ""
@@ -38,20 +38,23 @@
         self.checkBox.toggle()
 
         self.btn5 = QPushButton('predict', self)
         self.btn5.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
         self.btn5.clicked.connect(self.predicter)
         self.lbl = QLabel('original dir', self)
         self.lbl2 = QLabel('label dir', self)
-        self.lbl3 = QLabel('model dir (contains model.hdf5)', self)
+        self.lbl3 = QLabel('model path (.pth)', self)
         self.lbl4 = QLabel('output dir', self)
         self.build()
 
-        self.model = None
+        self.net = None
         self.worker_pred = None
+        self.ori_filenames = None
+        self.device = None
+        self.size = 512
 
     def build(self):
         vbox = QVBoxLayout()
         vbox.addWidget(combine_blocks(self.btn1, self.lbl))
         vbox.addWidget(combine_blocks(self.btn2, self.lbl2))
         vbox.addWidget(combine_blocks(self.btn3, self.lbl3))
         vbox.addWidget(combine_blocks(self.btn4, self.lbl4))
@@ -73,15 +76,15 @@
         f_name = QFileDialog.getExistingDirectory(self, 'Open Directory', default_path)
         if f_name:
             self.labelpath = f_name
             self.lbl2.setText(self.labelpath)
 
     def show_dialog_model(self):
         default_path = max(self.opath, self.labelpath, os.path.expanduser('~'))
-        f_name = QFileDialog.getExistingDirectory(self, 'Open Directory', default_path)
+        f_name, _ = QFileDialog.getOpenFileName(self, 'Select weight file', default_path)
         if f_name:
             self.modelpath = f_name
             self.lbl3.setText(self.modelpath)
 
     def show_dialog_outdir(self):
         default_path = max(self.opath, self.labelpath, os.path.expanduser('~'))
         f_name = QFileDialog.getExistingDirectory(self, 'Open Directory', default_path)
@@ -94,66 +97,59 @@
         try:
             csv = pd.read_csv(str(csvs[-1]), index_col=0)
         except:
             csv = None
         return csv, str(csvs[-1])
 
     def predicter(self):
-        ori_imgs, ori_filenames = load_X_gray(self.opath)
-        print(ori_imgs.shape)
-        input_shape = (512, 512, 1)
-        num_classes = 1
+        self.ori_filenames = sorted(list(Path(self.opath).glob('./*.png')))
 
-        self.model = get_nested_unet(input_shape=input_shape, num_classes=num_classes)
-        self.model.load_weights(os.path.join(self.modelpath, "model.hdf5"))
+        self.net = UnetPlusPlus(encoder_name="efficientnet-b0", encoder_weights="imagenet", in_channels=1, classes=1,
+                                activation='sigmoid')
+        self.device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+        state_dict = torch.load(self.modelpath, map_location=torch.device(self.device))
+        self.net.load_state_dict(state_dict)
+        self.net.to(self.device)
 
         self.btn5.setText('predicting')
 
         if self.checkBox.isChecked() is True:
-            self.predict(ori_imgs, ori_filenames)
+
+            self.predict()
         else:
-            self.predict_single(ori_imgs, ori_filenames)
+            self.predict_single()
 
-    def predict(self, ori_imgs, filenames):
+    def predict(self):
         try:
-            predict_3ax(ori_imgs, self.model, self.outpath, filenames)
+            predict_3ax(self.opath, self.net, self.outpath, self.size, self.device)
         except Exception as e:
             print(e)
         if self.labelpath != "":
-            try:
-                csv, csv_path = self.get_newest_csv()
-                if csv is None:
-                    pass
-                else:
-                    label_names = [node.filename for node in csv.itertuples() if node.train == "Checked"]
-                    for ln in label_names:
-                        shutil.copy(os.path.join(self.labelpath, ln), os.path.join(self.outpath, 'merged_prediction'))
-                    shutil.copy(str(csv_path), os.path.join(self.outpath, 'merged_prediction'))
-            except Exception as e:
-                print(e)
-
+            self.copy_previous_mask()
         self.btn5.setText('predict')
 
-    def predict_single(self, ori_imgs, filenames):
+    def predict_single(self):
         try:
-            predict_1ax(ori_imgs, self.model, self.outpath, filenames)
+            predict_1ax(self.ori_filenames, self.net, self.outpath, self.size, self.device)
         except Exception as e:
             print(e)
         if self.labelpath != "":
-            print('copy previous mask')
-            try:
-                csv, csv_path = self.get_newest_csv()
-                print('find csv', csv_path)
-                if csv is None:
-                    pass
-                else:
-                    label_names = [node.filename for node in csv.itertuples() if node.train == "Checked"]
-                    print(label_names)
-                    for ln in label_names:
-                        print('copy ln')
-                        shutil.copy(os.path.join(self.labelpath, ln), os.path.join(self.outpath, 'merged_prediction'))
-                    shutil.copy(str(csv_path), os.path.join(self.outpath, 'merged_prediction'))
-                    print('csv copied')
-            except Exception as e:
-                print(e)
-
+            self.copy_previous_mask()
         self.btn5.setText('predict')
+
+    def copy_previous_mask(self):
+        print('copy previous mask')
+        try:
+            csv, csv_path = self.get_newest_csv()
+            print('find csv', csv_path)
+            if csv is None:
+                pass
+            else:
+                label_names = [node.filename for node in csv.itertuples() if node.train == "Checked"]
+                print(label_names)
+                for ln in label_names:
+                    print('copy ln')
+                    shutil.copy(os.path.join(self.labelpath, ln), os.path.join(self.outpath, 'merged_prediction'))
+                shutil.copy(str(csv_path), os.path.join(self.outpath, 'merged_prediction'))
+                print('csv copied')
+        except Exception as e:
+            print(e)
```

### Comparing `napari-PHILOW-0.0.1/src/napari_philow/_tests/test_dock_widget.py` & `napari-PHILOW-0.1.0/src/napari_philow/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari-PHILOW-0.0.1/src/napari_philow/_train.py` & `napari-PHILOW-0.1.0/src/napari_philow/_train_tf.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,22 @@
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from PIL import Image
 from napari.qt import thread_worker
-from napari_tools_menu import register_dock_widget
-from qtpy.QtWidgets import QWidget, QPushButton, QSizePolicy, QLabel, QVBoxLayout, QFileDialog
+from qtpy.QtWidgets import QWidget, QPushButton, QSizePolicy, QLabel, QVBoxLayout, QFileDialog, QCheckBox
 from tensorflow.keras.callbacks import CSVLogger, ModelCheckpoint
 from tensorflow.keras.preprocessing.image import ImageDataGenerator
 
 from napari_philow._models import get_nested_unet
 from napari_philow._utils import combine_blocks, load_X_gray, load_Y_gray, select_train_data, divide_imgs
 
 
-@register_dock_widget(menu="PHILOW > Train mode")
 class Trainer(QWidget):
     def __init__(self, napari_viewer):
         super().__init__()
         self._viewer = napari_viewer
         self.opath = ""
         self.labelpath = ""
         self.modelpath = ""
@@ -37,14 +35,16 @@
 
         self.btn4 = QPushButton('start training', self)
         self.btn4.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
         self.btn4.clicked.connect(self.trainer)
         self.lbl = QLabel('original dir', self)
         self.lbl2 = QLabel('label dir', self)
         self.lbl3 = QLabel('model output dir', self)
+        self.checkBox = QCheckBox("resize to 256x256?")
+        self.checkBox.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
         self.build()
 
         self.model = None
         self.worker = None
         self.worker2 = None
 
     def build(self):
```

### Comparing `napari-PHILOW-0.0.1/src/napari_philow/_utils.py` & `napari-PHILOW-0.1.0/src/napari_philow/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 import numpy as np
 from scipy import ndimage
 from skimage import io
 from skimage.filters import gaussian
 import pandas as pd
 from tqdm import tqdm
 
-import tensorflow.keras.backend as K
-from tensorflow.keras.losses import binary_crossentropy
-
 
 def combine_blocks(block1, block2):
     temp_widget = QWidget()
     temp_layout = QHBoxLayout()
     temp_layout.addWidget(block1)
     temp_layout.addWidget(block2)
     temp_widget.setLayout(temp_layout)
@@ -113,15 +110,15 @@
 
 
 def load_saved_masks(mod_mask_dir):
     filename_pattern_label = os.path.join(mod_mask_dir, '*png')
     images_label = dask_image.imread.imread(filename_pattern_label)
     images_label = images_label.compute()
     base_label = images_label
-    return base_label
+    return base_label, [x.name for x in sorted(list(Path(mod_mask_dir).glob('./*png')))]
 
 
 def load_raw_masks(raw_mask_dir):
     filename_pattern_raw = os.path.join(raw_mask_dir, '*png')
     images_raw = dask_image.imread.imread(filename_pattern_raw)
     images_raw = images_raw.compute()
     base_label = np.where((126 < images_raw) & (images_raw < 171), 255, 0)
@@ -133,20 +130,19 @@
     temp_layout = QHBoxLayout()
     temp_layout.addWidget(block1)
     temp_layout.addWidget(block2)
     temp_widget.setLayout(temp_layout)
     return temp_widget
 
 
-def save_masks(labels, out_path):
+def save_masks(labels, out_path, filenames):
     num = labels.shape[0]
-    os.makedirs(out_path, exist_ok=True)
     for i in range(num):
         label = labels[i]
-        io.imsave(os.path.join(out_path, str(i).zfill(4) + '.png'), label)
+        io.imsave(os.path.join(out_path, filenames[i]), label)
 
 
 def label_and_sort(base_label):
     labeled = ndimage.label(base_label, structure=np.ones((3, 3, 3)))[0]
 
     mks, nums = np.unique(labeled, return_counts=True)
 
@@ -276,33 +272,14 @@
         if train_filename in train_img_names:
             train_ori_imgs.append(ori_img)
             train_label_imgs.append(label_img)
     print(ori_filenames)
     return np.array(train_ori_imgs), np.array(train_label_imgs)
 
 
-def dice_coeff(y_true, y_pred):
-    smooth = 1.
-    y_true_f = K.flatten(y_true)
-    y_pred_f = K.flatten(y_pred)
-    intersection = K.sum(y_true_f * y_pred_f)
-    score = (2. * intersection + smooth) / (K.sum(y_true_f) + K.sum(y_pred_f) + smooth)
-    return score
-
-
-def dice_loss(y_true, y_pred):
-    loss = 1 - dice_coeff(y_true, y_pred)
-    return loss
-
-
-def bce_dice_loss(y_true, y_pred):
-    loss = binary_crossentropy(y_true, y_pred) + dice_loss(y_true, y_pred)
-    return loss
-
-
 def divide_imgs(images):
     H = -(-images.shape[1] // 412)
     W = -(-images.shape[2] // 412)
 
     diveded_imgs = np.zeros((images.shape[0] * H * W, 512, 512, 1), np.float32)
     print(H, W)
```

