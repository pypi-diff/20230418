# Comparing `tmp/qctrl_qua-0.3.0.tar.gz` & `tmp/qctrl_qua-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_qua-0.3.0.tar", max compression
+gzip compressed data, was "qctrl_qua-0.3.1.tar", max compression
```

## Comparing `qctrl_qua-0.3.0.tar` & `qctrl_qua-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    36653 2023-03-23 22:31:58.847983 qctrl_qua-0.3.0/LICENSE
--rw-r--r--   0        0        0      122 2023-03-23 22:31:58.847983 qctrl_qua-0.3.0/README.md
--rw-r--r--   0        0        0     2555 2023-03-23 22:32:19.784071 qctrl_qua-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      817 2023-03-23 22:32:19.792071 qctrl_qua-0.3.0/qctrlqua/__init__.py
--rw-r--r--   0        0        0     3907 2023-03-23 22:31:58.847983 qctrl_qua-0.3.0/qctrlqua/qua_config_gen.py
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 qctrl_qua-0.3.0/setup.py
--rw-r--r--   0        0        0     2310 1970-01-01 00:00:00.000000 qctrl_qua-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-04-18 07:49:10.745215 qctrl_qua-0.3.1/LICENSE
+-rw-r--r--   0        0        0      131 2023-04-18 07:49:10.745215 qctrl_qua-0.3.1/README.md
+-rw-r--r--   0        0        0     2736 2023-04-18 07:49:29.630591 qctrl_qua-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      818 2023-04-18 07:49:29.634591 qctrl_qua-0.3.1/qctrlqua/__init__.py
+-rw-r--r--   0        0        0     3978 2023-04-18 07:49:10.745215 qctrl_qua-0.3.1/qctrlqua/qua_config_gen.py
+-rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 qctrl_qua-0.3.1/setup.py
+-rw-r--r--   0        0        0     2327 1970-01-01 00:00:00.000000 qctrl_qua-0.3.1/PKG-INFO
```

### Comparing `qctrl_qua-0.3.0/LICENSE` & `qctrl_qua-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_qua-0.3.0/pyproject.toml` & `qctrl_qua-0.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "qctrl-qua"
-version = "0.3.0"
-description = "Q-CTRL Python QUA"
+version = "0.3.1"
+description = "Q-CTRL Python QUA Adapter"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
 documentation = "https://docs.q-ctrl.com/boulder-opal/references/qctrl-qua/"
@@ -58,25 +58,25 @@
 ]
 packages = [
     { include = "qctrlqua" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
-numpy = "^1.24.0"
+numpy = "^1.23.5"
 
 [tool.poetry.dev-dependencies]
-black = "^23.1.0"
+black = "^23.3.0"
 isort = "^5.12.0"
-mypy = "^1.1.1"
+mypy = "^1.2.0"
 pylint = "^2.17.1"
-pytest = "^7.2.2"
-pre-commit = "^2.9.3"
-qctrl-sphinx-theme = "~0.1.2"
-qualang_tools = "~0.11.2"
+pytest = "^7.3.1"
+pre-commit = "^3.2.2"
+qctrl-sphinx-theme = "~0.1.3"
+qualang_tools = "~0.14.0"
 sphinx = "^5.3.0"
 tomli = "^2.0.1"
 
 [[tool.poetry.source]]
 name = "Q-CTRL PyPI"
 url = "https://pypi.q-ctrl.com/simple"
 secondary = true
@@ -97,10 +97,16 @@
 )
 '''
 
 [tool.isort]
 profile = "black"
 force_grid_wrap = "2"
 
+[tool.pytest.ini_options]
+filterwarnings = [
+    # https://docs.python.org/3/library/warnings.html#describing-warning-filters
+    "error",  # All warnings become errors.
+]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `qctrl_qua-0.3.0/qctrlqua/qua_config_gen.py` & `qctrl_qua-0.3.1/qctrlqua/qua_config_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,16 @@
         config["controllers"] = {}
     if "digital_waveforms" not in config:
         config["digital_waveforms"] = {}
     if "integration_weights" not in config:
         config["integration_weights"] = {}
     if "mixers" not in config:
         config["mixers"] = {}
+    if "oscillators" not in config:
+        config["oscillators"] = {}
     if "waveforms" not in config:
         config["waveforms"] = {}
     if "pulses" not in config:
         config["pulses"] = {}
     if "elements" not in config:
         config["elements"] = {}
     if channel_name not in config["elements"]:
```

### Comparing `qctrl_qua-0.3.0/setup.py` & `qctrl_qua-0.3.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['qctrlqua']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.24.0,<2.0.0']
+['numpy>=1.23.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'qctrl-qua',
-    'version': '0.3.0',
-    'description': 'Q-CTRL Python QUA',
-    'long_description': '# Q-CTRL QUA\n\nThe Q-CTRL QUA Python package allows you to integrate Boulder Opal with the QUA\nquantum computing language.\n',
+    'version': '0.3.1',
+    'description': 'Q-CTRL Python QUA Adapter',
+    'long_description': '# Q-CTRL QUA Adapter\n\nThe Q-CTRL QUA Adapter package allows you to integrate Boulder Opal with the QUA\nquantum computing language.\n',
     'author': 'Q-CTRL',
     'author_email': 'support@q-ctrl.com',
     'maintainer': 'Q-CTRL',
     'maintainer_email': 'support@q-ctrl.com',
     'url': 'https://q-ctrl.com',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `qctrl_qua-0.3.0/PKG-INFO` & `qctrl_qua-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: qctrl-qua
-Version: 0.3.0
-Summary: Q-CTRL Python QUA
+Version: 0.3.1
+Summary: Q-CTRL Python QUA Adapter
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
 Maintainer-email: support@q-ctrl.com
@@ -28,21 +28,21 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
-Requires-Dist: numpy (>=1.24.0,<2.0.0)
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Project-URL: Documentation, https://docs.q-ctrl.com/boulder-opal/references/qctrl-qua/
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Project-URL: YouTube, https://www.youtube.com/qctrl
 Description-Content-Type: text/markdown
 
-# Q-CTRL QUA
+# Q-CTRL QUA Adapter
 
-The Q-CTRL QUA Python package allows you to integrate Boulder Opal with the QUA
+The Q-CTRL QUA Adapter package allows you to integrate Boulder Opal with the QUA
 quantum computing language.
```

