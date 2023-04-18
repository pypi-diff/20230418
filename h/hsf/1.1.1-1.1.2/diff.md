# Comparing `tmp/HSF-1.1.1.tar.gz` & `tmp/hsf-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HSF-1.1.1.tar", max compression
+gzip compressed data, was "hsf-1.1.2.tar", max compression
```

## Comparing `HSF-1.1.1.tar` & `hsf-1.1.2.tar`

### file list

```diff
@@ -1,35 +1,30 @@
--rw-r--r--   0        0        0     1072 2021-11-07 09:51:34.344478 HSF-1.1.1/LICENSE.md
--rw-r--r--   0        0        0    10407 2022-04-27 08:33:34.321503 HSF-1.1.1/README.rst
--rw-r--r--   0        0        0       22 2022-04-27 08:34:50.730502 HSF-1.1.1/hsf/__init__.py
--rw-r--r--   0        0        0     1942 2022-04-26 12:54:30.433764 HSF-1.1.1/hsf/augmentation.py
--rw-r--r--   0        0        0        0 2021-11-07 09:51:34.378478 HSF-1.1.1/hsf/conf/__init__.py
--rw-r--r--   0        0        0      244 2021-11-07 09:51:34.378478 HSF-1.1.1/hsf/conf/augmentation/default.yaml
--rw-r--r--   0        0        0      202 2022-04-26 12:54:30.433764 HSF-1.1.1/hsf/conf/config.yaml
--rw-r--r--   0        0        0       78 2021-12-07 17:05:52.618169 HSF-1.1.1/hsf/conf/files/default.yaml
--rw-r--r--   0        0        0       67 2022-04-26 12:54:30.434764 HSF-1.1.1/hsf/conf/hardware/deepsparse.yaml
--rw-r--r--   0        0        0      126 2022-02-15 14:27:47.261084 HSF-1.1.1/hsf/conf/hardware/onnxruntime.yaml
--rw-r--r--   0        0        0     1514 2022-02-15 14:27:47.261084 HSF-1.1.1/hsf/conf/hydra/help/hsf.yaml
--rw-r--r--   0        0        0       75 2022-04-26 12:54:30.434764 HSF-1.1.1/hsf/conf/multispectrality/default.yaml
--rw-r--r--   0        0        0      139 2021-11-07 09:51:34.378478 HSF-1.1.1/hsf/conf/roiloc/default_corot2.yaml
--rw-r--r--   0        0        0      137 2021-11-07 09:51:34.378478 HSF-1.1.1/hsf/conf/roiloc/default_t2iso.yaml
--rw-r--r--   0        0        0      951 2022-04-26 12:54:30.434764 HSF-1.1.1/hsf/conf/segmentation/bagging_accurate.yaml
--rw-r--r--   0        0        0      955 2022-04-26 12:54:30.434764 HSF-1.1.1/hsf/conf/segmentation/bagging_fast.yaml
--rw-r--r--   0        0        0     1112 2022-04-26 12:54:30.434764 HSF-1.1.1/hsf/conf/segmentation/bagging_sq.yaml
--rw-r--r--   0        0        0      393 2022-04-26 12:54:30.434764 HSF-1.1.1/hsf/conf/segmentation/single_accurate.yaml
--rw-r--r--   0        0        0      398 2022-04-26 12:54:30.435764 HSF-1.1.1/hsf/conf/segmentation/single_fast.yaml
--rw-r--r--   0        0        0      506 2022-04-26 12:54:30.435764 HSF-1.1.1/hsf/conf/segmentation/single_sq.yaml
--rw-r--r--   0        0        0     3832 2022-04-26 12:54:30.435764 HSF-1.1.1/hsf/engines.py
--rw-r--r--   0        0        0     7642 2022-04-26 12:54:30.435764 HSF-1.1.1/hsf/factory.py
--rw-r--r--   0        0        0     1883 2022-04-26 12:54:30.435764 HSF-1.1.1/hsf/fetch_models.py
--rw-r--r--   0        0        0     1481 2022-04-24 18:34:39.427086 HSF-1.1.1/hsf/hsfui.py
--rw-r--r--   0        0        0     3765 2022-04-26 12:54:30.435764 HSF-1.1.1/hsf/multispectrality.py
--rw-r--r--   0        0        0     3373 2022-04-26 12:54:30.435764 HSF-1.1.1/hsf/roiloc_wrapper.py
--rw-r--r--   0        0        0     5743 2022-04-27 08:45:57.270493 HSF-1.1.1/hsf/segment.py
--rw-r--r--   0        0        0        0 2022-04-24 14:14:35.359182 HSF-1.1.1/hsf/tui/__init__.py
--rw-r--r--   0        0        0     2223 2022-04-24 18:23:22.617386 HSF-1.1.1/hsf/tui/main.py
--rw-r--r--   0        0        0     2148 2022-04-24 18:37:19.299538 HSF-1.1.1/hsf/tui/system.py
--rw-r--r--   0        0        0     1017 2021-11-07 09:51:34.380478 HSF-1.1.1/hsf/uncertainty.py
--rw-r--r--   0        0        0     2357 2022-02-15 14:27:47.261084 HSF-1.1.1/hsf/welcome.py
--rw-r--r--   0        0        0     1296 2022-04-27 08:35:51.498501 HSF-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    12041 2022-04-27 08:56:08.026166 HSF-1.1.1/setup.py
--rw-r--r--   0        0        0    11629 2022-04-27 08:56:08.027644 HSF-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-18 07:38:21.317162 hsf-1.1.2/LICENSE.md
+-rw-r--r--   0        0        0    10971 2023-04-18 11:32:34.270968 hsf-1.1.2/README.rst
+-rw-r--r--   0        0        0       22 2023-04-18 09:59:42.848045 hsf-1.1.2/hsf/__init__.py
+-rw-r--r--   0        0        0     1946 2023-04-18 08:46:28.068106 hsf-1.1.2/hsf/augmentation.py
+-rw-r--r--   0        0        0        0 2023-04-18 07:38:21.351163 hsf-1.1.2/hsf/conf/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-18 07:38:21.351163 hsf-1.1.2/hsf/conf/augmentation/default.yaml
+-rw-r--r--   0        0        0      202 2023-04-18 07:38:21.352162 hsf-1.1.2/hsf/conf/config.yaml
+-rw-r--r--   0        0        0       78 2023-04-18 07:38:21.352162 hsf-1.1.2/hsf/conf/files/default.yaml
+-rw-r--r--   0        0        0       67 2023-04-18 07:38:21.352162 hsf-1.1.2/hsf/conf/hardware/deepsparse.yaml
+-rw-r--r--   0        0        0      126 2023-04-18 07:38:21.352162 hsf-1.1.2/hsf/conf/hardware/onnxruntime.yaml
+-rw-r--r--   0        0        0     1514 2023-04-18 07:38:21.352162 hsf-1.1.2/hsf/conf/hydra/help/hsf.yaml
+-rw-r--r--   0        0        0       75 2023-04-18 07:38:21.352162 hsf-1.1.2/hsf/conf/multispectrality/default.yaml
+-rw-r--r--   0        0        0      139 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/roiloc/default_corot2.yaml
+-rw-r--r--   0        0        0      137 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/roiloc/default_t2iso.yaml
+-rw-r--r--   0        0        0      951 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/segmentation/bagging_accurate.yaml
+-rw-r--r--   0        0        0      955 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/segmentation/bagging_fast.yaml
+-rw-r--r--   0        0        0     1112 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/segmentation/bagging_sq.yaml
+-rw-r--r--   0        0        0      393 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/segmentation/single_accurate.yaml
+-rw-r--r--   0        0        0      398 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/segmentation/single_fast.yaml
+-rw-r--r--   0        0        0      506 2023-04-18 07:38:21.353162 hsf-1.1.2/hsf/conf/segmentation/single_sq.yaml
+-rw-r--r--   0        0        0     4322 2023-04-18 10:07:31.648039 hsf-1.1.2/hsf/engines.py
+-rw-r--r--   0        0        0     7646 2023-04-18 08:47:20.656105 hsf-1.1.2/hsf/factory.py
+-rw-r--r--   0        0        0     1887 2023-04-18 08:47:28.240105 hsf-1.1.2/hsf/fetch_models.py
+-rw-r--r--   0        0        0     3769 2023-04-18 08:45:26.889107 hsf-1.1.2/hsf/multispectrality.py
+-rw-r--r--   0        0        0     3377 2023-04-18 08:45:37.718107 hsf-1.1.2/hsf/roiloc_wrapper.py
+-rw-r--r--   0        0        0     5743 2023-04-18 07:38:21.355162 hsf-1.1.2/hsf/segment.py
+-rw-r--r--   0        0        0     1017 2023-04-18 07:38:21.355162 hsf-1.1.2/hsf/uncertainty.py
+-rw-r--r--   0        0        0     2357 2023-04-18 07:38:21.355162 hsf-1.1.2/hsf/welcome.py
+-rw-r--r--   0        0        0     1520 2023-04-18 11:49:31.103954 hsf-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    12381 1970-01-01 00:00:00.000000 hsf-1.1.2/PKG-INFO
```

### Comparing `HSF-1.1.1/LICENSE.md` & `hsf-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `HSF-1.1.1/README.rst` & `hsf-1.1.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,21 @@
 
 To install the package, first setup an environment suitable for your backend (e.g. `ONNX Runtime <https://onnxruntime.ai>`_).
 
 If the environment isn't properly configured, you might be stuck running inference sessions on CPU, which is not optimal unless you use the DeepSparse backend.
 
 Then, simply run:
 
-``pip install hsf``.
+``pip install hsf["your_hardware"]``.
+
+You should always specify the hardware you want to use, as it will install the proper dependencies, supported choices are ``cpu``, ``gpu`` and ``sparse``.
+
+So for example, if you want to use the GPU backend, run:
+
+``pip install hsf["gpu"]``.
 
 
 Quick start
 ===========
 
 Once installed, HSF can be used simply by running the ``hsf`` command.
 
@@ -210,14 +216,21 @@
 
 Changelogs
 ==========
 
 HSF
 ---
 
+**Version 1.1.2**
+
+* ***BREAKING CHANGE***: HSF needs to be installed using extra dependencies depending on the backend you want to use.
+  See the [installation guide](https://hsf.readthedocs.io/en/latest/user-guide/installation/) for more details.
+* Updated dependencies
+* Fixed installation on MacOS
+ 
 **Version 1.1.1**
 
 * Added whole-hippocampus segmentation
 
 **Version 1.1.0**
 
 * New optional multispectral mode de segment from both T1 AND T2 images
```

### Comparing `HSF-1.1.1/hsf/augmentation.py` & `hsf-1.1.2/hsf/augmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from multiprocessing.pool import ThreadPool
 
 import torchio as tio
 from omegaconf.dictconfig import DictConfig
 from rich.logging import RichHandler
 
 FORMAT = "%(message)s"
-logging.basicConfig(level="NOTSET",
+logging.basicConfig(level=logging.INFO,
                     format=FORMAT,
                     datefmt="[%X]",
                     handlers=[RichHandler()])
 
 log = logging.getLogger(__name__)
```

### Comparing `HSF-1.1.1/hsf/conf/hydra/help/hsf.yaml` & `hsf-1.1.2/hsf/conf/hydra/help/hsf.yaml`

 * *Files identical despite different names*

### Comparing `HSF-1.1.1/hsf/conf/segmentation/bagging_accurate.yaml` & `hsf-1.1.2/hsf/conf/segmentation/bagging_accurate.yaml`

 * *Files identical despite different names*

### Comparing `HSF-1.1.1/hsf/conf/segmentation/bagging_fast.yaml` & `hsf-1.1.2/hsf/conf/segmentation/bagging_fast.yaml`

 * *Files identical despite different names*

### Comparing `HSF-1.1.1/hsf/conf/segmentation/bagging_sq.yaml` & `hsf-1.1.2/hsf/conf/segmentation/bagging_sq.yaml`

 * *Files identical despite different names*

### Comparing `HSF-1.1.1/hsf/engines.py` & `hsf-1.1.2/hsf/engines.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 from pathlib import Path, PosixPath
 from typing import Generator
 
-import deepsparse
 import onnxruntime as ort
 from omegaconf.dictconfig import DictConfig
 from omegaconf.listconfig import ListConfig
 
+# If DeepSparse is installed, import it
+try:
+    import deepsparse
+    DEEPSPARSE_AVAILABLE = True
+except ImportError:
+    DEEPSPARSE_AVAILABLE = False
+
 
 def deepsparse_support() -> str:
     """
     Check if the CPU supports DeepSparse's optimizations.
 
     Returns:
         str: Support Status
     """
+    if not DEEPSPARSE_AVAILABLE:
+        return "not installed (you probably installed hsf using `pip install hsf[cpu]` or `hsf[gpu]`)"
+
     avx2 = deepsparse.cpu.cpu_avx2_compatible()
     avx512 = deepsparse.cpu.cpu_avx512_compatible()
     vnni = deepsparse.cpu.cpu_vnni_compatible()
 
     if vnni:
         # Optimal for int8 quantized NN
         return "full"
@@ -50,14 +59,19 @@
         models_path (PosixPath): Path to the models.
         engine_name (str): Name of the engine. Can be "onnxruntime" or "deepsparse".
         engine_settings (DictConfig): Engine settings.
 
     Returns:
         List[InferenceEngine]: Inference Engines.
     """
+    if engine_name == "deepsparse" and not DEEPSPARSE_AVAILABLE:
+        raise ImportError(
+            "DeepSparse is not installed. If you are on Linux, please install it using `pip install hsf[sparse]`."
+        )
+
     p = Path(models_path).expanduser()
     models = list(p.glob("*.onnx"))
 
     for model in models:
         yield InferenceEngine(engine_name=engine_name,
                               engine_settings=engine_settings,
                               model=model)
```

### Comparing `HSF-1.1.1/hsf/factory.py` & `hsf-1.1.2/hsf/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from hsf.roiloc_wrapper import (get_hippocampi, get_mri, load_from_config,
                                 save_hippocampi)
 from hsf.segment import mri_to_subject, save_prediction, segment
 from hsf.uncertainty import voxelwise_uncertainty
 from hsf.welcome import welcome
 
 FORMAT = "%(message)s"
-logging.basicConfig(level="NOTSET",
+logging.basicConfig(level=logging.INFO,
                     format=FORMAT,
                     datefmt="[%X]",
                     handlers=[RichHandler()])
 
 log = logging.getLogger(__name__)
 
 # initialize(config_path="hsf/conf")
```

### Comparing `HSF-1.1.1/hsf/fetch_models.py` & `hsf-1.1.2/hsf/fetch_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import wget
 import xxhash
 from omegaconf import DictConfig
 from rich.logging import RichHandler
 
 FORMAT = "%(message)s"
-logging.basicConfig(level="NOTSET",
+logging.basicConfig(level=logging.INFO,
                     format=FORMAT,
                     datefmt="[%X]",
                     handlers=[RichHandler()])
 
 log = logging.getLogger(__name__)
```

### Comparing `HSF-1.1.1/hsf/multispectrality.py` & `hsf-1.1.2/hsf/multispectrality.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from rich.logging import RichHandler
 from roiloc._cache import handle_cache
 from roiloc.locator import RoiLocator
 
 from hsf.roiloc_wrapper import save_hippocampi
 
 FORMAT = "%(message)s"
-logging.basicConfig(level="NOTSET",
+logging.basicConfig(level=logging.INFO,
                     format=FORMAT,
                     datefmt="[%X]",
                     handlers=[RichHandler()])
 
 log = logging.getLogger(__name__)
```

### Comparing `HSF-1.1.1/hsf/roiloc_wrapper.py` & `hsf-1.1.2/hsf/roiloc_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import ants
 from omegaconf.dictconfig import DictConfig
 from rich.logging import RichHandler
 from roiloc.locator import RoiLocator
 
 FORMAT = "%(message)s"
-logging.basicConfig(level="NOTSET",
+logging.basicConfig(level=logging.INFO,
                     format=FORMAT,
                     datefmt="[%X]",
                     handlers=[RichHandler()])
 
 log = logging.getLogger(__name__)
```

### Comparing `HSF-1.1.1/hsf/segment.py` & `hsf-1.1.2/hsf/segment.py`

 * *Files identical despite different names*

### Comparing `HSF-1.1.1/hsf/uncertainty.py` & `hsf-1.1.2/hsf/uncertainty.py`

 * *Files identical despite different names*

### Comparing `HSF-1.1.1/hsf/welcome.py` & `hsf-1.1.2/hsf/welcome.py`

 * *Files identical despite different names*

### Comparing `HSF-1.1.1/pyproject.toml` & `hsf-1.1.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "HSF"
-version = "1.1.1"
+version = "1.1.2"
 description = "A simple yet exhaustive segmentation tool of the Hippocampal Subfields in T1w and T2w MRIs."
 authors = ["Clément POIRET <poiret.clement@outlook.fr>"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["mri", "brain", "hippocampus", "segmentation", "deep learning"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -16,24 +16,30 @@
 repository = "https://github.com/clementpoiret/HSF"
 
 [tool.poetry.scripts]
 hsf = 'hsf.factory:start'
 deepsparse_support = 'hsf.engines:print_deepsparse_support'
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
+python = ">=3.7.1,<3.11"
 torchio = "^0.18.56"
 roiloc = ">0.2.8"
-onnxruntime = "^1.8.1"
 hydra-core = "^1.1.1"
 wget = "^3.2"
-antspyx = ">0.2.9"
-xxhash = "^2.0.2"
+antspyx = ">0.3.0"
+xxhash = "^3.2.0"
 rich = ">11.0.0"
-deepsparse = ">0.8.0, <1.0.0"
+onnxruntime = {version = "^1.14.0", optional = true}
+onnxruntime-gpu = {version = "^1.14.0", optional = true}
+deepsparse = {version = "^1.4.0", optional = true}
+
+[tool.poetry.extras]
+cpu = ["onnxruntime"]
+gpu = ["onnxruntime-gpu"]
+sparse = ["deepsparse", "onnxruntime"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^6"
 coverage = {version = "^6.0.1", extras = ["toml"]}
 
 [tool.pytest.ini_options]
 filterwarnings = ["ignore::DeprecationWarning"]
```

### Comparing `HSF-1.1.1/setup.py` & `hsf-1.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,352 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: hsf
+Version: 1.1.2
+Summary: A simple yet exhaustive segmentation tool of the Hippocampal Subfields in T1w and T2w MRIs.
+Home-page: https://hippomnesis.dev
+License: MIT
+Keywords: mri,brain,hippocampus,segmentation,deep learning
+Author: Clément POIRET
+Author-email: poiret.clement@outlook.fr
+Requires-Python: >=3.7.1,<3.11
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Provides-Extra: cpu
+Provides-Extra: gpu
+Provides-Extra: sparse
+Requires-Dist: antspyx (>0.3.0)
+Requires-Dist: deepsparse (>=1.4.0,<2.0.0) ; extra == "sparse"
+Requires-Dist: hydra-core (>=1.1.1,<2.0.0)
+Requires-Dist: onnxruntime (>=1.14.0,<2.0.0) ; extra == "cpu" or extra == "sparse"
+Requires-Dist: onnxruntime-gpu (>=1.14.0,<2.0.0) ; extra == "gpu"
+Requires-Dist: rich (>11.0.0)
+Requires-Dist: roiloc (>0.2.8)
+Requires-Dist: torchio (>=0.18.56,<0.19.0)
+Requires-Dist: wget (>=3.2,<4.0)
+Requires-Dist: xxhash (>=3.2.0,<4.0.0)
+Project-URL: Repository, https://github.com/clementpoiret/HSF
+Description-Content-Type: text/x-rst
 
-packages = \
-['hsf', 'hsf.conf', 'hsf.tui']
+======================================
+Hippocampal Segmentation Factory (HSF)
+======================================
 
-package_data = \
-{'': ['*'],
- 'hsf.conf': ['augmentation/*',
-              'files/*',
-              'hardware/*',
-              'hydra/help/*',
-              'multispectrality/*',
-              'roiloc/*',
-              'segmentation/*']}
-
-install_requires = \
-['antspyx>0.2.9',
- 'deepsparse>0.8.0,<1.0.0',
- 'hydra-core>=1.1.1,<2.0.0',
- 'onnxruntime>=1.8.1,<2.0.0',
- 'rich>11.0.0',
- 'roiloc>0.2.8',
- 'torchio>=0.18.56,<0.19.0',
- 'wget>=3.2,<4.0',
- 'xxhash>=2.0.2,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['deepsparse_support = '
-                     'hsf.engines:print_deepsparse_support',
-                     'hsf = hsf.factory:start']}
-
-setup_kwargs = {
-    'name': 'hsf',
-    'version': '1.1.1',
-    'description': 'A simple yet exhaustive segmentation tool of the Hippocampal Subfields in T1w and T2w MRIs.',
-    'long_description': '======================================\nHippocampal Segmentation Factory (HSF)\n======================================\n\nExhaustive documentation available at: `hsf.rtfd.io <https://hsf.rtfd.io/>`_\n\n**Current Models version:** 3.0.0\n\n.. list-table::\n    :header-rows: 1\n\n    * - Python Package\n      - Code Quality\n      - Misc\n    * - .. image:: https://github.com/clementpoiret/HSF/actions/workflows/python-app.yml/badge.svg?branch=master\n        .. image:: https://badge.fury.io/py/hsf.svg\n           :target: https://badge.fury.io/py/hsf\n        .. image:: https://img.shields.io/pypi/dm/hsf\n           :alt: PyPI - Downloads\n      - .. image:: https://app.codacy.com/project/badge/Grade/cf02d1f84739401ba695e24f333c23b7\n           :target: https://www.codacy.com/gh/clementpoiret/HSF/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=clementpoiret/HSF&amp;utm_campaign=Badge_Grade\n        .. image:: https://app.codacy.com/project/badge/Coverage/cf02d1f84739401ba695e24f333c23b7\n           :target: https://www.codacy.com/gh/clementpoiret/HSF/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=clementpoiret/HSF&amp;utm_campaign=Badge_Grade\n        .. image:: https://api.codeclimate.com/v1/badges/e0bf481dcbf3eecebefd/maintainability\n           :target: https://codeclimate.com/github/clementpoiret/HSF/maintainability\n           :alt: Maintainability\n      - .. image:: https://readthedocs.org/projects/hsf/badge/?version=latest\n           :target: https://hsf.readthedocs.io/en/latest/?badge=latest\n           :alt: Documentation Status\n        .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5527122.svg\n           :target: https://doi.org/10.5281/zenodo.5527122\n\n\nThe Hippocampal Segmentation Factory (HSF) is a Python package for\nthe segmentation of the hippocampal subfields in raw MRI volumes.\n\n.. image:: https://raw.githubusercontent.com/clementpoiret/HSF/master/docs/resources/header.svg\n\nThe main idea is to have a one-liner tool that allows the user to\nsegment the hippocampal subfields in a given raw image (T1w or T2w), while keeping\nas much modularity and customization options as possible.\n\nHSF will be able to segment the following subfields:\n\n- Dentate gyrus (DG),\n- Cornu Ammonis (CA1, CA2 & CA3) in a flexible way (e.g. you can ask to combine CA2 and CA3),\n- Subiculum (SUB).\n\nHSF will segment the hippocampus from head to tail: it will produce\nan homogeneous segmentation from the anterior hippocampus (head), to\nthe posterior hippocampus (tail), without assigning a specific head\nor tail class.\n\nHSF results from a collaborative effort:\n\n1. We are continuously working on improving the segmentation of the subfields,\n   mainly by adding new manually segmented MRIs (feel free to send us yours if you can, thanks!)\n2. HSF proposes a "Model Hub", meaning that anyone can distribute their own ONNX segmentation\n   model. Just send us a small `*.yaml` config file, and the end-user will effortlessly be able to\n   use HSF with your model.\n\nPlease note that the tool is still under development and is not yet\nready for production use. It uses multiple expert deep learning models\ntrained on 700+ manually segmented hippocampi which are not yet fully polished.\n\nHSF uses inference sessions provided by `ONNXRuntime <https://onnxruntime.ai>`_,\nwhich means that it can be used *theoretically* on Windows, MacOS and Linux,\nand the following hardware accelerations: CPU, CUDA, DirectML, OneDNN,\nOpenVINO, TensorRT, NUPHAR, Vitis AI, ACL, ArmNN, MIGraphX, and Rockchip NPU.\nPlease be aware that we do not tested all possible configurations, as HSF\nhas been tested only on CPU and CUDA on Linux (Debian-based and Arch-based distros).\n\nSince v1.0.0, HSF also provides a `DeepSparse backend <https://neuralmagic.com/technology/>`_\nwhich can be used in conjunction with pruned and int8 quantized models\nto deliver a much faster CPU inference speed (see [Hardware Acceleration](user-guide/configuration.md)\nsection).\n\n\nTable of Contents...\n====================\n\n.. contents:: ...To guide you in the challenging world of hippocampal subfields segmentation :)\n\n\nInstallation\n============\n\nTo install the package, first setup an environment suitable for your backend (e.g. `ONNX Runtime <https://onnxruntime.ai>`_).\n\nIf the environment isn\'t properly configured, you might be stuck running inference sessions on CPU, which is not optimal unless you use the DeepSparse backend.\n\nThen, simply run:\n\n``pip install hsf``.\n\n\nQuick start\n===========\n\nOnce installed, HSF can be used simply by running the ``hsf`` command.\n\nFor example, to segment a set of T2w MRIs of 0.3*0.3*1.2, run:\n\n``hsf files.path="~/Dataset/MRIs/" files.pattern="*T2w.nii" roiloc.contrast="t2" roiloc.margin=[10,2,10] segmentation=bagging_accurate segmentation.ca_mode="1/2/3"``\n\nNow, let\'s dive into the details.\n\n``files.path`` and ``files.pattern`` are mandatory parameters.\nThey specify the path to the dataset (or MRI) and the pattern to find the files.\n\nAll parameters starting with ``roiloc.`` are directly linked to our home-made ROI location algorithm.\nYou can find more information about it in the `related GitHub repository <https://github.com/clementpoiret/ROILoc>`_.\n\nTo date, we propose 4 different segmentation algorithms (from the fastest to the most accurate):\n\n- ``single_fast``: a segmentation is performed on the whole volume by only one model,\n- ``single_accurate``: a single model segments the same volume that has been augmented 20 times through TTA,\n- ``single_sq``: like ``single_accurate``, but using int8-quantized sparse models for a fast and efficient inference,\n- ``bagging_fast``: a bagging ensemble of 5 models is used to segment the volume without TTA,\n- ``bagging_accurate``: a bagging ensemble of 5 models is used to segment the volume with TTA,\n- ``bagging_sq``: like ``bagging_accurate``, but using int8-quantized sparse models for a fast and efficient inference.\n\nFinally, ``segmentation.ca_mode`` is a parameter that allows to combine CA1, CA2 and CA3 subfields.\nIt is particularly useful when you want to segment low-resolution images where it makes no sense to\ndistinguish between CA\'s subfields.\n\n\nConfiguration\n=============\n\nAs HSF is pretty modular, you can easily configure it to your needs thanks to Hydra.\n\nCompose your configuration from those groups (group=option)\n\n* augmentation: default\n* files: default\n* hardware: deepsparse, onnxruntime\n* multispectrality: default\n* roiloc: default_corot2, default_t2iso\n* segmentation: bagging_accurate, bagging_fast, bagging_sq, single_accurate, single_fast, single_sq\n\nOverride anything in the config (e.g. hsf roiloc.margin=[16,2,16])\n\nYou can also add specific configs absent from the default yaml files\n(e.g. hsf +augmentation.elastic.image_interpolation=sitkBSpline)\n\nFields set with ??? are mandatory.\n\n   files:\n\n   * path: ???\n   * pattern: ???\n   * mask_pattern: ``*mask.nii.gz``\n   * output_dir: hsf_outputs\n\n   roiloc:\n\n   * contrast: t2\n   * roi: hippocampus\n   * bet: false\n   * transform_type: AffineFast\n   * margin: [8, 8, 8]\n   * rightoffset: [0, 0, 0]\n   * leftoffset: [0, 0, 0]\n\n   segmentation:\n\n   * ca_mode: 1/2/3\n   * models_path: ~/.hsf/models\n   * models:\n      *  arunet_bag_0.onnx:\n      *  url: https://zenodo.org/record/5524594/files/arunet_bag0.onnx?download=1\n      *  xxh3_64: d0de65baa81d9382\n      * segmentation:\n         * test_time_augmentation: true\n         * test_time_num_aug: 20\n\n   augmentation:\n\n   * flip:\n      * axes:\n         * LR\n      * flip_probability: 0.5\n      * affine_probability: 0.75\n      * affine:\n         * scales: 0.2\n         * degrees: 15\n         * translation: 3\n         * isotropic: false\n      * elastic_probability: 0.25\n      * elastic:\n         * num_control_points: 4\n         * max_displacement: 4\n         * locked_borders: 0\n\n   multispectrality:\n   \n   * pattern: null\n   * same_space: true\n   * registration:\n     * type_of_transform: Affine\n\n   hardware:\n  \n   * engine: onnxruntime\n   * engine_settings:\n     * execution_providers: ["CUDAExecutionProvider","CPUExecutionProvider"]\n     * batch_size: 1\n\n\nChangelogs\n==========\n\nHSF\n---\n\n**Version 1.1.1**\n\n* Added whole-hippocampus segmentation\n\n**Version 1.1.0**\n\n* New optional multispectral mode de segment from both T1 AND T2 images\n* Bug fixes and optimizations\n\n**Version 1.0.1**\n\n* Fix batch size issue\n\n**Version 1.0.0**\n\n* Added Uncertainty Maps for post-hoc analysis of segmentation results,\n* Support for DeepSparse backend (CPU inference only),\n* Introduced **HSF\'s Model Hub**,\n* Support for batch inference (all backends),\n* Check for updates at startup,\n* Bug fixes and optimizations.\n\n**Version 0.1.2**\n\n* Added build-in support for offsets to recenter the hippocampus in ROILoc,\n* Added support for the customization of Hardware Execution Providers.\n\n**Version 0.1.1**\n\n* Fixed CUDA Execution Provider.\n\n**Version 0.1.0**\n\n* Initial release.\n\n\nModels\n------\n\n**Version 3.0.0**\n\n* More data (coming from the Human Connectome Project),\n* New sparse and int8-quantized models.\n\n**Version 2.1.1**\n\n* Fixed some tails in 3T CoroT2w images (MemoDev)\n\n**Version 2.1.0**\n\n* Corrected incorrect T1w labels used for training,\n* Trained on slightly more data (T1w @1.5T & 3T, T2w; Healthy, Epilepsy & Alzheimer)\n\n**Version 2.0.0**\n\n* Trained with more T1w and T2w MRIs,\n* Trained on more hippocampal sclerosis and Alzheimer\'s disease cases,\n* Updated training pipeline (hyperparameter tuning),\n* `single` models are now independant from bags.\n\n**Version 1.0.0**\n\n* Initial release.\n\n\nDocumentation\n==========================\n\nFor more details about HSF\'s configuration and internal parameters, please refer to\nour `documentation <https://hsf.rtfd.io/>`_.\n\n\nAuthorship, Affiliations and Citations\n======================================\n\nAuthorship:\n\n* C Poiret, UNIACT-NeuroSpin, CEA, Saclay University, France,\n* A Bouyeure, UNIACT-NeuroSpin, CEA, Saclay University, France,\n* S Patil, UNIACT-NeuroSpin, CEA, Saclay University, France,\n* C Boniteau, UNIACT-NeuroSpin, CEA, Saclay University, France,\n* M Noulhiane, UNIACT-NeuroSpin, CEA, Saclay University, France.\n\nIf you use this work, please cite it as follows:\n\n``C. Poiret, et al. (2021). clementpoiret/HSF. Zenodo. https://doi.org/10.5281/zenodo.5527122``\n\nThis work licensed under MIT license was supported in part by the Fondation de France and the IDRIS/GENCI for the HPE Supercomputer Jean Zay.\n',
-    'author': 'Clément POIRET',
-    'author_email': 'poiret.clement@outlook.fr',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://hippomnesis.dev',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<4.0.0',
-}
+Exhaustive documentation available at: `hsf.rtfd.io <https://hsf.rtfd.io/>`_
 
+**Current Models version:** 3.0.0
+
+.. list-table::
+    :header-rows: 1
+
+    * - Python Package
+      - Code Quality
+      - Misc
+    * - .. image:: https://github.com/clementpoiret/HSF/actions/workflows/python-app.yml/badge.svg?branch=master
+        .. image:: https://badge.fury.io/py/hsf.svg
+           :target: https://badge.fury.io/py/hsf
+        .. image:: https://img.shields.io/pypi/dm/hsf
+           :alt: PyPI - Downloads
+      - .. image:: https://app.codacy.com/project/badge/Grade/cf02d1f84739401ba695e24f333c23b7
+           :target: https://www.codacy.com/gh/clementpoiret/HSF/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=clementpoiret/HSF&amp;utm_campaign=Badge_Grade
+        .. image:: https://app.codacy.com/project/badge/Coverage/cf02d1f84739401ba695e24f333c23b7
+           :target: https://www.codacy.com/gh/clementpoiret/HSF/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=clementpoiret/HSF&amp;utm_campaign=Badge_Grade
+        .. image:: https://api.codeclimate.com/v1/badges/e0bf481dcbf3eecebefd/maintainability
+           :target: https://codeclimate.com/github/clementpoiret/HSF/maintainability
+           :alt: Maintainability
+      - .. image:: https://readthedocs.org/projects/hsf/badge/?version=latest
+           :target: https://hsf.readthedocs.io/en/latest/?badge=latest
+           :alt: Documentation Status
+        .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5527122.svg
+           :target: https://doi.org/10.5281/zenodo.5527122
+
+
+The Hippocampal Segmentation Factory (HSF) is a Python package for
+the segmentation of the hippocampal subfields in raw MRI volumes.
+
+.. image:: https://raw.githubusercontent.com/clementpoiret/HSF/master/docs/resources/header.svg
+
+The main idea is to have a one-liner tool that allows the user to
+segment the hippocampal subfields in a given raw image (T1w or T2w), while keeping
+as much modularity and customization options as possible.
+
+HSF will be able to segment the following subfields:
+
+- Dentate gyrus (DG),
+- Cornu Ammonis (CA1, CA2 & CA3) in a flexible way (e.g. you can ask to combine CA2 and CA3),
+- Subiculum (SUB).
+
+HSF will segment the hippocampus from head to tail: it will produce
+an homogeneous segmentation from the anterior hippocampus (head), to
+the posterior hippocampus (tail), without assigning a specific head
+or tail class.
+
+HSF results from a collaborative effort:
+
+1. We are continuously working on improving the segmentation of the subfields,
+   mainly by adding new manually segmented MRIs (feel free to send us yours if you can, thanks!)
+2. HSF proposes a "Model Hub", meaning that anyone can distribute their own ONNX segmentation
+   model. Just send us a small `*.yaml` config file, and the end-user will effortlessly be able to
+   use HSF with your model.
+
+Please note that the tool is still under development and is not yet
+ready for production use. It uses multiple expert deep learning models
+trained on 700+ manually segmented hippocampi which are not yet fully polished.
+
+HSF uses inference sessions provided by `ONNXRuntime <https://onnxruntime.ai>`_,
+which means that it can be used *theoretically* on Windows, MacOS and Linux,
+and the following hardware accelerations: CPU, CUDA, DirectML, OneDNN,
+OpenVINO, TensorRT, NUPHAR, Vitis AI, ACL, ArmNN, MIGraphX, and Rockchip NPU.
+Please be aware that we do not tested all possible configurations, as HSF
+has been tested only on CPU and CUDA on Linux (Debian-based and Arch-based distros).
+
+Since v1.0.0, HSF also provides a `DeepSparse backend <https://neuralmagic.com/technology/>`_
+which can be used in conjunction with pruned and int8 quantized models
+to deliver a much faster CPU inference speed (see [Hardware Acceleration](user-guide/configuration.md)
+section).
+
+
+Table of Contents...
+====================
+
+.. contents:: ...To guide you in the challenging world of hippocampal subfields segmentation :)
+
+
+Installation
+============
+
+To install the package, first setup an environment suitable for your backend (e.g. `ONNX Runtime <https://onnxruntime.ai>`_).
+
+If the environment isn't properly configured, you might be stuck running inference sessions on CPU, which is not optimal unless you use the DeepSparse backend.
+
+Then, simply run:
+
+``pip install hsf["your_hardware"]``.
+
+You should always specify the hardware you want to use, as it will install the proper dependencies, supported choices are ``cpu``, ``gpu`` and ``sparse``.
+
+So for example, if you want to use the GPU backend, run:
+
+``pip install hsf["gpu"]``.
+
+
+Quick start
+===========
+
+Once installed, HSF can be used simply by running the ``hsf`` command.
+
+For example, to segment a set of T2w MRIs of 0.3*0.3*1.2, run:
+
+``hsf files.path="~/Dataset/MRIs/" files.pattern="*T2w.nii" roiloc.contrast="t2" roiloc.margin=[10,2,10] segmentation=bagging_accurate segmentation.ca_mode="1/2/3"``
+
+Now, let's dive into the details.
+
+``files.path`` and ``files.pattern`` are mandatory parameters.
+They specify the path to the dataset (or MRI) and the pattern to find the files.
+
+All parameters starting with ``roiloc.`` are directly linked to our home-made ROI location algorithm.
+You can find more information about it in the `related GitHub repository <https://github.com/clementpoiret/ROILoc>`_.
+
+To date, we propose 4 different segmentation algorithms (from the fastest to the most accurate):
+
+- ``single_fast``: a segmentation is performed on the whole volume by only one model,
+- ``single_accurate``: a single model segments the same volume that has been augmented 20 times through TTA,
+- ``single_sq``: like ``single_accurate``, but using int8-quantized sparse models for a fast and efficient inference,
+- ``bagging_fast``: a bagging ensemble of 5 models is used to segment the volume without TTA,
+- ``bagging_accurate``: a bagging ensemble of 5 models is used to segment the volume with TTA,
+- ``bagging_sq``: like ``bagging_accurate``, but using int8-quantized sparse models for a fast and efficient inference.
+
+Finally, ``segmentation.ca_mode`` is a parameter that allows to combine CA1, CA2 and CA3 subfields.
+It is particularly useful when you want to segment low-resolution images where it makes no sense to
+distinguish between CA's subfields.
+
+
+Configuration
+=============
+
+As HSF is pretty modular, you can easily configure it to your needs thanks to Hydra.
+
+Compose your configuration from those groups (group=option)
+
+* augmentation: default
+* files: default
+* hardware: deepsparse, onnxruntime
+* multispectrality: default
+* roiloc: default_corot2, default_t2iso
+* segmentation: bagging_accurate, bagging_fast, bagging_sq, single_accurate, single_fast, single_sq
+
+Override anything in the config (e.g. hsf roiloc.margin=[16,2,16])
+
+You can also add specific configs absent from the default yaml files
+(e.g. hsf +augmentation.elastic.image_interpolation=sitkBSpline)
+
+Fields set with ??? are mandatory.
+
+   files:
+
+   * path: ???
+   * pattern: ???
+   * mask_pattern: ``*mask.nii.gz``
+   * output_dir: hsf_outputs
+
+   roiloc:
+
+   * contrast: t2
+   * roi: hippocampus
+   * bet: false
+   * transform_type: AffineFast
+   * margin: [8, 8, 8]
+   * rightoffset: [0, 0, 0]
+   * leftoffset: [0, 0, 0]
+
+   segmentation:
+
+   * ca_mode: 1/2/3
+   * models_path: ~/.hsf/models
+   * models:
+      *  arunet_bag_0.onnx:
+      *  url: https://zenodo.org/record/5524594/files/arunet_bag0.onnx?download=1
+      *  xxh3_64: d0de65baa81d9382
+      * segmentation:
+         * test_time_augmentation: true
+         * test_time_num_aug: 20
+
+   augmentation:
+
+   * flip:
+      * axes:
+         * LR
+      * flip_probability: 0.5
+      * affine_probability: 0.75
+      * affine:
+         * scales: 0.2
+         * degrees: 15
+         * translation: 3
+         * isotropic: false
+      * elastic_probability: 0.25
+      * elastic:
+         * num_control_points: 4
+         * max_displacement: 4
+         * locked_borders: 0
+
+   multispectrality:
+   
+   * pattern: null
+   * same_space: true
+   * registration:
+     * type_of_transform: Affine
+
+   hardware:
+  
+   * engine: onnxruntime
+   * engine_settings:
+     * execution_providers: ["CUDAExecutionProvider","CPUExecutionProvider"]
+     * batch_size: 1
+
+
+Changelogs
+==========
+
+HSF
+---
+
+**Version 1.1.2**
+
+* ***BREAKING CHANGE***: HSF needs to be installed using extra dependencies depending on the backend you want to use.
+  See the [installation guide](https://hsf.readthedocs.io/en/latest/user-guide/installation/) for more details.
+* Updated dependencies
+* Fixed installation on MacOS
+ 
+**Version 1.1.1**
+
+* Added whole-hippocampus segmentation
+
+**Version 1.1.0**
+
+* New optional multispectral mode de segment from both T1 AND T2 images
+* Bug fixes and optimizations
+
+**Version 1.0.1**
+
+* Fix batch size issue
+
+**Version 1.0.0**
+
+* Added Uncertainty Maps for post-hoc analysis of segmentation results,
+* Support for DeepSparse backend (CPU inference only),
+* Introduced **HSF's Model Hub**,
+* Support for batch inference (all backends),
+* Check for updates at startup,
+* Bug fixes and optimizations.
+
+**Version 0.1.2**
+
+* Added build-in support for offsets to recenter the hippocampus in ROILoc,
+* Added support for the customization of Hardware Execution Providers.
+
+**Version 0.1.1**
+
+* Fixed CUDA Execution Provider.
+
+**Version 0.1.0**
+
+* Initial release.
+
+
+Models
+------
+
+**Version 3.0.0**
+
+* More data (coming from the Human Connectome Project),
+* New sparse and int8-quantized models.
+
+**Version 2.1.1**
+
+* Fixed some tails in 3T CoroT2w images (MemoDev)
+
+**Version 2.1.0**
+
+* Corrected incorrect T1w labels used for training,
+* Trained on slightly more data (T1w @1.5T & 3T, T2w; Healthy, Epilepsy & Alzheimer)
+
+**Version 2.0.0**
+
+* Trained with more T1w and T2w MRIs,
+* Trained on more hippocampal sclerosis and Alzheimer's disease cases,
+* Updated training pipeline (hyperparameter tuning),
+* `single` models are now independant from bags.
+
+**Version 1.0.0**
+
+* Initial release.
+
+
+Documentation
+==========================
+
+For more details about HSF's configuration and internal parameters, please refer to
+our `documentation <https://hsf.rtfd.io/>`_.
+
+
+Authorship, Affiliations and Citations
+======================================
+
+Authorship:
+
+* C Poiret, UNIACT-NeuroSpin, CEA, Saclay University, France,
+* A Bouyeure, UNIACT-NeuroSpin, CEA, Saclay University, France,
+* S Patil, UNIACT-NeuroSpin, CEA, Saclay University, France,
+* C Boniteau, UNIACT-NeuroSpin, CEA, Saclay University, France,
+* M Noulhiane, UNIACT-NeuroSpin, CEA, Saclay University, France.
+
+If you use this work, please cite it as follows:
+
+``C. Poiret, et al. (2021). clementpoiret/HSF. Zenodo. https://doi.org/10.5281/zenodo.5527122``
+
+This work licensed under MIT license was supported in part by the Fondation de France and the IDRIS/GENCI for the HPE Supercomputer Jean Zay.
 
-setup(**setup_kwargs)
```

