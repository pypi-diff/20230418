# Comparing `tmp/yolov7x-0.1.0.tar.gz` & `tmp/yolov7x-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolov7x-0.1.0.tar", max compression
+gzip compressed data, was "yolov7x-0.1.1.tar", max compression
```

## Comparing `yolov7x-0.1.0.tar` & `yolov7x-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,29 @@
--rw-r--r--   0        0        0        0 2023-04-18 04:56:28.989634 yolov7x-0.1.0/README.md
--rw-r--r--   0        0        0      666 2023-04-18 04:53:36.663188 yolov7x-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        6 2023-04-18 04:45:56.468662 yolov7x-0.1.0/yolov7x/__init__.py
--rw-r--r--   0        0        0    84388 2023-04-18 04:45:56.468662 yolov7x-0.1.0/yolov7x/common.py
--rw-r--r--   0        0        0    10898 2023-04-18 04:45:56.468662 yolov7x-0.1.0/yolov7x/experimental.py
--rw-r--r--   0        0        0    40024 2023-04-18 04:45:56.468662 yolov7x-0.1.0/yolov7x/yolo.py
--rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 yolov7x-0.1.0/setup.py
--rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 yolov7x-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-18 04:56:28.989634 yolov7x-0.1.1/README.md
+-rw-r--r--   0        0        0      697 2023-04-18 05:31:24.430271 yolov7x-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-04-18 04:45:56.468662 yolov7x-0.1.1/src/models/__init__.py
+-rw-r--r--   0        0        0    84388 2023-04-18 04:45:56.468662 yolov7x-0.1.1/src/models/common.py
+-rw-r--r--   0        0        0    10898 2023-04-18 04:45:56.468662 yolov7x-0.1.1/src/models/experimental.py
+-rw-r--r--   0        0        0    40024 2023-04-18 04:45:56.468662 yolov7x-0.1.1/src/models/yolo.py
+-rw-r--r--   0        0        0        6 2023-04-18 05:23:52.001499 yolov7x-0.1.1/src/utils/__init__.py
+-rw-r--r--   0        0        0     2248 2023-04-18 05:23:52.001499 yolov7x-0.1.1/src/utils/activations.py
+-rw-r--r--   0        0        0     5616 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/add_nms.py
+-rw-r--r--   0        0        0     7147 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/autoanchor.py
+-rw-r--r--   0        0        0        5 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/aws/__init__.py
+-rw-r--r--   0        0        0      780 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/aws/mime.sh
+-rw-r--r--   0        0        0     1113 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/aws/resume.py
+-rw-r--r--   0        0        0     1250 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/aws/userdata.sh
+-rw-r--r--   0        0        0    56225 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/datasets.py
+-rw-r--r--   0        0        0    36876 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/general.py
+-rw-r--r--   0        0        0      821 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/google_app_engine/Dockerfile
+-rw-r--r--   0        0        0      105 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/google_app_engine/additional_requirements.txt
+-rw-r--r--   0        0        0      172 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/google_app_engine/app.yaml
+-rw-r--r--   0        0        0     4873 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/google_utils.py
+-rw-r--r--   0        0        0    75030 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/loss.py
+-rw-r--r--   0        0        0     9310 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/metrics.py
+-rw-r--r--   0        0        0    20921 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/plots.py
+-rw-r--r--   0        0        0    15467 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/torch_utils.py
+-rw-r--r--   0        0        0        6 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/wandb_logging/__init__.py
+-rw-r--r--   0        0        0      815 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/wandb_logging/log_dataset.py
+-rw-r--r--   0        0        0    16265 2023-04-18 05:23:52.005499 yolov7x-0.1.1/src/utils/wandb_logging/wandb_utils.py
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 yolov7x-0.1.1/setup.py
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 yolov7x-0.1.1/PKG-INFO
```

### Comparing `yolov7x-0.1.0/pyproject.toml` & `yolov7x-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "yolov7x"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
-authors = ["Your Name <you@example.com>"]
+authors = ["Doohoon Kim <me@doohoon.kim>"]
 readme = "README.md"
+packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.6"
 matplotlib = ">=3.2.2"
 numpy = ">=1.18.5,<1.24.0"
 opencv-python = ">=4.1.1"
 pillow = ">=7.1.2"
 pyyaml = ">=5.3.1"
 requests = ">=2.23.0"
 scipy = ">=1.4.1"
```

### Comparing `yolov7x-0.1.0/yolov7x/common.py` & `yolov7x-0.1.1/src/models/common.py`

 * *Files identical despite different names*

### Comparing `yolov7x-0.1.0/yolov7x/experimental.py` & `yolov7x-0.1.1/src/models/experimental.py`

 * *Files identical despite different names*

### Comparing `yolov7x-0.1.0/yolov7x/yolo.py` & `yolov7x-0.1.1/src/models/yolo.py`

 * *Files identical despite different names*

### Comparing `yolov7x-0.1.0/setup.py` & `yolov7x-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['yolov7x']
+['src', 'src.models', 'src.utils', 'src.utils.aws', 'src.utils.wandb_logging']
 
 package_data = \
-{'': ['*']}
+{'': ['*'], 'src.utils': ['google_app_engine/*']}
 
 install_requires = \
 ['ipython>=8.12.0,<9.0.0',
  'matplotlib>=3.2.2',
  'numpy>=1.18.5,<1.24.0',
  'opencv-python>=4.1.1',
  'pandas>=1.1.4',
@@ -24,23 +24,23 @@
  'thop>=0.1.1.post2209072238,<0.2.0',
  'torch>=1.7.0,!=1.12.0',
  'torchvision>=0.8.1,!=0.13.0',
  'tqdm>=4.41.0']
 
 setup_kwargs = {
     'name': 'yolov7x',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '',
-    'author': 'Your Name',
-    'author_email': 'you@example.com',
+    'author': 'Doohoon Kim',
+    'author_email': 'me@doohoon.kim',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.6,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `yolov7x-0.1.0/PKG-INFO` & `yolov7x-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: yolov7x
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
-Author: Your Name
-Author-email: you@example.com
-Requires-Python: >=3.10,<4.0
+Author: Doohoon Kim
+Author-email: me@doohoon.kim
+Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipython (>=8.12.0,<9.0.0)
 Requires-Dist: matplotlib (>=3.2.2)
 Requires-Dist: numpy (>=1.18.5,<1.24.0)
 Requires-Dist: opencv-python (>=4.1.1)
 Requires-Dist: pandas (>=1.1.4)
```

