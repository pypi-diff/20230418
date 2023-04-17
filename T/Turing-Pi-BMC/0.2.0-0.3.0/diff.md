# Comparing `tmp/Turing Pi BMC-0.2.0.tar.gz` & `tmp/Turing Pi BMC-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Turing Pi BMC-0.2.0.tar", last modified: Mon Apr 17 22:18:43 2023, max compression
+gzip compressed data, was "Turing Pi BMC-0.3.0.tar", last modified: Mon Apr 17 22:30:26 2023, max compression
```

## Comparing `Turing Pi BMC-0.2.0.tar` & `Turing Pi BMC-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:18:43.740735 Turing Pi BMC-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-17 22:18:43.740735 Turing Pi BMC-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:18:43.740735 Turing Pi BMC-0.2.0/Turing_Pi_BMC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-17 22:18:43.000000 Turing Pi BMC-0.2.0/Turing_Pi_BMC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-17 22:18:43.000000 Turing Pi BMC-0.2.0/Turing_Pi_BMC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:18:43.000000 Turing Pi BMC-0.2.0/Turing_Pi_BMC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 22:18:43.000000 Turing Pi BMC-0.2.0/Turing_Pi_BMC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 22:18:43.000000 Turing Pi BMC-0.2.0/Turing_Pi_BMC.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:18:43.740735 Turing Pi BMC-0.2.0/bmc/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/cluster_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/sdcard.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/turing_pi_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/bmc/usb_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 22:18:32.000000 Turing Pi BMC-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-17 22:18:43.740735 Turing Pi BMC-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:26.195318 Turing Pi BMC-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-17 22:30:13.000000 Turing Pi BMC-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-17 22:30:26.195318 Turing Pi BMC-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 22:30:13.000000 Turing Pi BMC-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:26.195318 Turing Pi BMC-0.3.0/Turing_Pi_BMC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-17 22:30:26.000000 Turing Pi BMC-0.3.0/Turing_Pi_BMC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-17 22:30:26.000000 Turing Pi BMC-0.3.0/Turing_Pi_BMC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:30:26.000000 Turing Pi BMC-0.3.0/Turing_Pi_BMC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 22:30:26.000000 Turing Pi BMC-0.3.0/Turing_Pi_BMC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 22:30:26.000000 Turing Pi BMC-0.3.0/Turing_Pi_BMC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:30:26.195318 Turing Pi BMC-0.3.0/bmc/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 22:30:13.000000 Turing Pi BMC-0.3.0/bmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-17 22:30:13.000000 Turing Pi BMC-0.3.0/bmc/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-17 22:30:13.000000 Turing Pi BMC-0.3.0/bmc/cluster_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-17 22:30:13.000000 Turing Pi BMC-0.3.0/bmc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-17 22:30:13.000000 Turing Pi BMC-0.3.0/bmc/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-17 22:30:13.000000 Turing Pi BMC-0.3.0/bmc/sdcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-17 22:30:13.000000 Turing Pi BMC-0.3.0/bmc/turing_pi_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-17 22:30:13.000000 Turing Pi BMC-0.3.0/bmc/usb_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 22:30:13.000000 Turing Pi BMC-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-17 22:30:26.195318 Turing Pi BMC-0.3.0/setup.cfg
```

### Comparing `Turing Pi BMC-0.2.0/LICENSE` & `Turing Pi BMC-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Turing Pi BMC-0.2.0/PKG-INFO` & `Turing Pi BMC-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Turing Pi BMC
-Version: 0.2.0
+Version: 0.3.0
 Summary: Package to manage a Turing Pi 2 cluster using the BMC API
 Home-page: https://github.com/petermcd/bmc
 Author: Peter McDonald
 Author-email: git@petermcdonald.co.uk
 Project-URL: Bug Tracker, https://github.com/petermcd/turing-pi-bmc/issues
 Project-URL: Source, https://github.com/petermcd/turing-pi-bmc
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Turing Pi BMC-0.2.0/Turing_Pi_BMC.egg-info/PKG-INFO` & `Turing Pi BMC-0.3.0/Turing_Pi_BMC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Turing-Pi-BMC
-Version: 0.2.0
+Version: 0.3.0
 Summary: Package to manage a Turing Pi 2 cluster using the BMC API
 Home-page: https://github.com/petermcd/bmc
 Author: Peter McDonald
 Author-email: git@petermcdonald.co.uk
 Project-URL: Bug Tracker, https://github.com/petermcd/turing-pi-bmc/issues
 Project-URL: Source, https://github.com/petermcd/turing-pi-bmc
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Turing Pi BMC-0.2.0/bmc/cluster.py` & `Turing Pi BMC-0.3.0/bmc/cluster.py`

 * *Files identical despite different names*

### Comparing `Turing Pi BMC-0.2.0/bmc/cluster_request.py` & `Turing Pi BMC-0.3.0/bmc/cluster_request.py`

 * *Files identical despite different names*

### Comparing `Turing Pi BMC-0.2.0/bmc/node.py` & `Turing Pi BMC-0.3.0/bmc/node.py`

 * *Files identical despite different names*

### Comparing `Turing Pi BMC-0.2.0/setup.cfg` & `Turing Pi BMC-0.3.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Turing Pi BMC
-version = 0.2.0
+version = 0.3.0
 author = Peter McDonald
 author_email = git@petermcdonald.co.uk
 description = Package to manage a Turing Pi 2 cluster using the BMC API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/petermcd/bmc
 project_urls = 
@@ -17,17 +17,18 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Intended Audience :: Developers
 
 [options]
 packages = find:
 python_requires = >=3.9
+install_requires = requests; semver
 
 [options.extras_require]
-test = flake8; isort; mypy;
+test = pre-commit;
 build = wheel; build;
 
 [flake8]
 max_line_length = 120
 
 [egg_info]
 tag_build =
```

