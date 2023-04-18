# Comparing `tmp/turbo_broccoli-2.3.8.tar.gz` & `tmp/turbo_broccoli-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_broccoli-2.3.8.tar", last modified: Wed Apr 12 04:11:51 2023, max compression
+gzip compressed data, was "turbo_broccoli-2.4.3.tar", last modified: Tue Apr 18 01:56:44 2023, max compression
```

## Comparing `turbo_broccoli-2.3.8.tar` & `turbo_broccoli-2.4.3.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:11:51.169348 turbo_broccoli-2.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18239 2023-04-12 04:11:51.169348 turbo_broccoli-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 04:11:51.169348 turbo_broccoli-2.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:11:51.165347 turbo_broccoli-2.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25383 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_bokeh.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_nodecode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    52428 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/tests/test_tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:11:51.169348 turbo_broccoli-2.3.8/turbo_broccoli/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/bokeh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/guard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     8770 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/turbo_broccoli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-12 04:11:40.000000 turbo_broccoli-2.3.8/turbo_broccoli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:11:51.169348 turbo_broccoli-2.3.8/turbo_broccoli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18239 2023-04-12 04:11:51.000000 turbo_broccoli-2.3.8/turbo_broccoli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-12 04:11:51.000000 turbo_broccoli-2.3.8/turbo_broccoli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 04:11:51.000000 turbo_broccoli-2.3.8/turbo_broccoli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 04:11:51.000000 turbo_broccoli-2.3.8/turbo_broccoli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:56:44.911273 turbo_broccoli-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18799 2023-04-18 01:56:44.911273 turbo_broccoli-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 01:56:44.911273 turbo_broccoli-2.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:56:44.907273 turbo_broccoli-2.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25383 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_bokeh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_nodecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52467 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/tests/test_tensorflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:56:44.911273 turbo_broccoli-2.4.3/turbo_broccoli/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/bokeh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13828 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8770 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/turbo_broccoli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-18 01:56:31.000000 turbo_broccoli-2.4.3/turbo_broccoli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:56:44.911273 turbo_broccoli-2.4.3/turbo_broccoli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18799 2023-04-18 01:56:44.000000 turbo_broccoli-2.4.3/turbo_broccoli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-18 01:56:44.000000 turbo_broccoli-2.4.3/turbo_broccoli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:56:44.000000 turbo_broccoli-2.4.3/turbo_broccoli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 01:56:44.000000 turbo_broccoli-2.4.3/turbo_broccoli.egg-info/top_level.txt
```

### Comparing `turbo_broccoli-2.3.8/LICENSE` & `turbo_broccoli-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/PKG-INFO` & `turbo_broccoli-2.4.3/turbo_broccoli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: turbo_broccoli
-Version: 2.3.8
+Name: turbo-broccoli
+Version: 2.4.3
 Summary: JSON (de)serialization extensions
 Home-page: https://github.com/altaris/turbo-broccoli
 Author: Cédric Ho Thanh
 Author-email: altaris@users.noreply.github.com
 Project-URL: Issues, https://github.com/altaris/turbo-broccoli/issues
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 ![License](https://img.shields.io/github/license/altaris/turbo-broccoli)
 [![Code
 style](https://img.shields.io/badge/style-black-black)](https://pypi.org/project/black)
 ![hehe](https://img.shields.io/badge/project%20name%20by-github-pink)
 [![Documentation](https://badgen.net/badge/documentation/here/green)](https://https://altaris.github.io/turbo-broccoli/turbo_broccoli.html)
 
 JSON (de)serialization extensions, originally aimed at `numpy` and `tensorflow`
-objects.
+objects, but now supporting a wide range of objects.
 
 # Installation
 
 ```sh
 pip install turbo-broccoli
 ```
 
@@ -80,15 +80,15 @@
 
 ## Supported types
 
 ### Basic types
 
 - [`bytes`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/bytes.html#to_json)
 
-- `dict` with non `str` keys
+- [`dict` with non `str` keys](https://altaris.github.io/turbo-broccoli/turbo_broccoli/dict.html#to_json)
 
 - [Collections](https://altaris.github.io/turbo-broccoli/turbo_broccoli/collections.html#to_json):
   `collections.deque`, `collections.namedtuple`
 
 - [Dataclasses](https://altaris.github.io/turbo-broccoli/turbo_broccoli/dataclass.html#to_json): serialization is straightforward:
   ```py
   @dataclass
@@ -413,15 +413,17 @@
   Comma-separated list of types to not deserialize, for example
   `bytes,numpy.ndarray`. Excludable types are:
 
   - `bokeh`, `bokeh.buffer`, `bokeh.generic`,
 
   - `bytes`,
 
-  - `dict`,
+  - `dict` (this will only disable [Turbo Broccoli's custom
+    serialization](https://altaris.github.io/turbo-broccoli/turbo_broccoli/dict.html#to_json)
+    of `dict`s with non `str` keys),
 
   - `collections`, `collections.deque`, `collections.namedtuple`,
 
   - `dataclass`, `dataclass.<dataclass_name>` (case sensitive),
 
   - `generic`,
 
@@ -457,14 +459,23 @@
 
 This is so cool. Check out
 [`turbo_broccoli.GuardedBlockHandler`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#GuardedBlockHandler),
 [`turbo_broccoli.guarded_call`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#guarded_call),
 and
 [`turbo_broccoli.produces_document`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#produces_document).
 
+## CLI
+
+Turbo Broccoli has a few utilities that can be accessed from the CLI.
+
+- `list-artifacts`: Prints all the artifacts filenames or file paths that are
+  referenced by a given json file.
+
+- `rm`: Removes a json file and all the artifacts it references.
+
 # Contributing
 
 ## Dependencies
 
 - `python3.9` or newer;
 
 - `requirements.txt` for runtime dependencies;
```

### Comparing `turbo_broccoli-2.3.8/README.md` & `turbo_broccoli-2.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ![License](https://img.shields.io/github/license/altaris/turbo-broccoli)
 [![Code
 style](https://img.shields.io/badge/style-black-black)](https://pypi.org/project/black)
 ![hehe](https://img.shields.io/badge/project%20name%20by-github-pink)
 [![Documentation](https://badgen.net/badge/documentation/here/green)](https://https://altaris.github.io/turbo-broccoli/turbo_broccoli.html)
 
 JSON (de)serialization extensions, originally aimed at `numpy` and `tensorflow`
-objects.
+objects, but now supporting a wide range of objects.
 
 # Installation
 
 ```sh
 pip install turbo-broccoli
 ```
 
@@ -62,15 +62,15 @@
 
 ## Supported types
 
 ### Basic types
 
 - [`bytes`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/bytes.html#to_json)
 
-- `dict` with non `str` keys
+- [`dict` with non `str` keys](https://altaris.github.io/turbo-broccoli/turbo_broccoli/dict.html#to_json)
 
 - [Collections](https://altaris.github.io/turbo-broccoli/turbo_broccoli/collections.html#to_json):
   `collections.deque`, `collections.namedtuple`
 
 - [Dataclasses](https://altaris.github.io/turbo-broccoli/turbo_broccoli/dataclass.html#to_json): serialization is straightforward:
   ```py
   @dataclass
@@ -395,15 +395,17 @@
   Comma-separated list of types to not deserialize, for example
   `bytes,numpy.ndarray`. Excludable types are:
 
   - `bokeh`, `bokeh.buffer`, `bokeh.generic`,
 
   - `bytes`,
 
-  - `dict`,
+  - `dict` (this will only disable [Turbo Broccoli's custom
+    serialization](https://altaris.github.io/turbo-broccoli/turbo_broccoli/dict.html#to_json)
+    of `dict`s with non `str` keys),
 
   - `collections`, `collections.deque`, `collections.namedtuple`,
 
   - `dataclass`, `dataclass.<dataclass_name>` (case sensitive),
 
   - `generic`,
 
@@ -439,14 +441,23 @@
 
 This is so cool. Check out
 [`turbo_broccoli.GuardedBlockHandler`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#GuardedBlockHandler),
 [`turbo_broccoli.guarded_call`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#guarded_call),
 and
 [`turbo_broccoli.produces_document`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#produces_document).
 
+## CLI
+
+Turbo Broccoli has a few utilities that can be accessed from the CLI.
+
+- `list-artifacts`: Prints all the artifacts filenames or file paths that are
+  referenced by a given json file.
+
+- `rm`: Removes a json file and all the artifacts it references.
+
 # Contributing
 
 ## Dependencies
 
 - `python3.9` or newer;
 
 - `requirements.txt` for runtime dependencies;
```

### Comparing `turbo_broccoli-2.3.8/setup.py` & `turbo_broccoli-2.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 """Setup script"""
 
 import setuptools
 
 name = "turbo_broccoli"
-version = "2.3.8"
+version = "2.4.3"
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as f:
     requirements = f.read().split()
```

### Comparing `turbo_broccoli-2.3.8/tests/test_bokeh.py` & `turbo_broccoli-2.4.3/tests/test_bokeh.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/tests/test_collections.py` & `turbo_broccoli-2.4.3/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/tests/test_dataclass.py` & `turbo_broccoli-2.4.3/tests/test_dataclass.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # pylint: disable=missing-class-docstring
 # pylint: disable=missing-function-docstring
 """deque (de)serialization test suite"""
 
 from dataclasses import dataclass
 
-from turbo_broccoli.environment import register_dataclass_type
+from common import from_json, to_json  # Must be before turbo_broccoli imports
 
-from common import from_json, to_json
+from turbo_broccoli.environment import register_dataclass_type
 
 
 @dataclass
 class C:
     a_byte_str: bytes
     a_list: list
     a_str: str
```

### Comparing `turbo_broccoli-2.3.8/tests/test_dict.py` & `turbo_broccoli-2.4.3/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/tests/test_generic.py` & `turbo_broccoli-2.4.3/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/tests/test_guard.py` & `turbo_broccoli-2.4.3/tests/test_guard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 # pylint: disable=missing-function-docstring
-"""Test suite for `tdt.produces_document`"""
+"""Test suite for guarded blocks/loops"""
 
 from pathlib import Path
+
+# Must be before turbo_broccoli imports
+# pylint: disable=unused-import
+import common
+
 from turbo_broccoli import (
     GuardedBlockHandler,
     guarded_call,
     produces_document,
     load_json,
 )
 
+TEST_PATH = Path("out") / "test"
+
 
 def test_guarded_bloc_handler_iter():
-    path = Path("out") / "test_guarded_bloc_handler_iter"
+    path = TEST_PATH / "test_guarded_bloc_handler_iter"
     h = GuardedBlockHandler(path)
     l1, l2 = [1, 2, 3], [2, 3, 4]
-    # l1, l2 = list(map(str, l1)), list(map(str, l2))  # Keys should be str
     # First loop
     for x in h.guard(l1):
         # Initialization of results at each iteration
         assert x in h.result
         assert h.result[x] is None
         h.result[x] = int(x)
     # Second loop over same iterable should be skipped
     for x in h.guard(l1):
         assert False
     # Final value
-    assert h.result == {str(i): i for i in l1}
+    assert h.result == {i: i for i in l1}
     # Check output files individually
     for x in l1:
         p = path / f"{x}.json"
         assert p.is_file()
         assert load_json(p) == int(x)
     # Second iteration where some output files already exist
     for x in h.guard(l2):
         if (
             int(x) <= 3
         ):  # Iterations for files that already exist should be skipped
             assert False
         h.result[x] = int(x)
-    assert h.result == {str(i): i for i in l2}
+    assert h.result == {i: i for i in l2}
 
 
 def test_guarded_bloc_handler_no_iter():
-    path = "out/test_guarded_bloc_handler_no_iter.json"
+    path = TEST_PATH / "test_guarded_bloc_handler_no_iter.json"
     h = GuardedBlockHandler(path)
     for _ in h.guard():
         h.result = 41
         h.result = 42
     # Block should be skipped
     for _ in h.guard():
         assert False
@@ -54,41 +60,41 @@
     assert h.result == load_json(path)
 
 
 def test_guarded_call():
     def f(a: int):
         return {"a": a}
 
-    path = "out/test_guarded_call.json"
+    path = TEST_PATH / "test_guarded_call.json"
     x = guarded_call(f, path, 1)
     y = load_json(path)
     assert isinstance(x, dict)
     assert x == y
     assert x != f(2)
     assert x == guarded_call(f, path, 2)  # Intended behavior
 
 
 def test_produces_document():
     def f(a: int):
         return {"a": a}
 
-    path = "out/test_produces_document.json"
+    path = TEST_PATH / "test_produces_document.json"
     _f = produces_document(f, path, check_args=False)
     x = _f(1)
     y = load_json(path)
     assert isinstance(x, dict)
     assert x == y
     assert x != f(2)
     assert x == _f(2)  # Intended behavior
 
 
 def test_produces_document_check_args():
     def f(a: int):
         return {"a": a}
 
-    path = "out/test_produces_document_check_args.json"
+    path = TEST_PATH / "test_produces_document_check_args.json"
     _f = produces_document(f, path, check_args=True)
     assert _f(1) == {"a": 1}
     assert _f(2) == {"a": 2}
     assert _f(1) == {"a": 1}  # Repetition intended
     assert _f(2) == {"a": 2}  # Repetition intended
     assert _f(1) != _f(2)
```

### Comparing `turbo_broccoli-2.3.8/tests/test_keras.py` & `turbo_broccoli-2.4.3/tests/test_keras.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # pylint: disable=missing-function-docstring
 """Keras (de)serialization test suite"""
 
 from tensorflow import keras
 import numpy as np
 from numpy.testing import assert_array_equal
 
-from turbo_broccoli.environment import set_keras_format
+from common import from_json, to_json  # Must be before turbo_broccoli imports
 
-from common import from_json, to_json
+from turbo_broccoli.environment import set_keras_format
 
 
 def _assert_model_equal(a, b):
     assert a.get_config() == b.get_config()
     for i, w in enumerate(a.weights):
         assert_array_equal(w, b.weights[i])
     # Not really necessary but why not
```

### Comparing `turbo_broccoli-2.3.8/tests/test_nodecode.py` & `turbo_broccoli-2.4.3/tests/test_nodecode.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from collections import deque
 from dataclasses import dataclass
 
 import numpy as np
 import pandas as pd
 import tensorflow as tf
-from common import from_json, to_json
+from common import from_json, to_json  # Must be before turbo_broccoli imports
 from test_keras import _build_model
 from test_pandas import _assert_equal as assert_equal_pd
 
 from turbo_broccoli.environment import register_dataclass_type, set_nodecode
 
 
 def _basic_dict() -> dict:
```

### Comparing `turbo_broccoli-2.3.8/tests/test_numpy.py` & `turbo_broccoli-2.4.3/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/tests/test_pandas.py` & `turbo_broccoli-2.4.3/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/tests/test_pytorch.py` & `turbo_broccoli-2.4.3/tests/test_pytorch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # pylint: disable=missing-function-docstring
 """Pytorch (de)serialization test suite"""
 
 import os
 import torch
 
-from turbo_broccoli.environment import register_pytorch_module_type
+from common import from_json, to_json  # Must be before turbo_broccoli imports
 
-from common import from_json, to_json
+from turbo_broccoli.environment import register_pytorch_module_type
 
 
 class _TestModule(torch.nn.Module):
 
     module: torch.nn.Module
 
     def __init__(self):
```

### Comparing `turbo_broccoli-2.3.8/tests/test_scipy.py` & `turbo_broccoli-2.4.3/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/tests/test_secret.py` & `turbo_broccoli-2.4.3/tests/test_secret.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # pylint: disable=missing-function-docstring
 """(de)serialization of secrets"""
 
 import nacl.secret
 import nacl.utils
-from nacl.exceptions import CryptoError
 import pytest
+from common import from_json, to_json  # Must be before turbo_broccoli imports
+from nacl.exceptions import CryptoError
+
 from turbo_broccoli.environment import set_shared_key
 from turbo_broccoli.secret import (
     LockedSecret,
     Secret,
     SecretDict,
     SecretFloat,
     SecretInt,
     SecretList,
     SecretStr,
 )
 
-from common import from_json, to_json
-
 
 def _new_key() -> bytes:
     return nacl.utils.random(nacl.secret.SecretBox.KEY_SIZE)
 
 
 def assert_secret_equal(a: Secret, b: Secret):
     assert type(a) == type(b)  # pylint: disable=unidiomatic-typecheck
```

### Comparing `turbo_broccoli-2.3.8/tests/test_sklearn.py` & `turbo_broccoli-2.4.3/tests/test_sklearn.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from typing import Optional, Tuple
 
 import numpy as np
 from common import from_json, to_json
 from numpy.testing import assert_array_equal
 from scipy import sparse
+from sklearn.base import BaseEstimator
 from sklearn.calibration import *
 from sklearn.cluster import *
 from sklearn.compose import *
 from sklearn.covariance import *
 from sklearn.cross_decomposition import *
 from sklearn.datasets import *
 from sklearn.datasets import load_digits, make_sparse_coded_signal
@@ -29,28 +30,28 @@
 from sklearn.inspection import *
 from sklearn.isotonic import *
 from sklearn.kernel_approximation import *
 from sklearn.kernel_ridge import *
 from sklearn.linear_model import *
 from sklearn.manifold import *
 from sklearn.metrics import *
+from sklearn.metrics.pairwise import pairwise_kernels
 from sklearn.mixture import *
 from sklearn.model_selection import *
 from sklearn.multiclass import *
 from sklearn.multioutput import *
 from sklearn.naive_bayes import *
 from sklearn.neighbors import *
 from sklearn.neural_network import *
 from sklearn.pipeline import *
 from sklearn.preprocessing import *
 from sklearn.random_projection import *
 from sklearn.semi_supervised import *
 from sklearn.svm import *
 from sklearn.tree import *
-from sklearn.metrics.pairwise import pairwise_kernels
 
 
 def _to_json_and_back(obj: BaseEstimator) -> BaseEstimator:
     return from_json(to_json({"e": obj}))["e"]
 
 
 def _fit_labels_test(
```

### Comparing `turbo_broccoli-2.3.8/tests/test_tensorflow.py` & `turbo_broccoli-2.4.3/tests/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/__init__.py` & `turbo_broccoli-2.4.3/turbo_broccoli/__init__.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/bokeh.py` & `turbo_broccoli-2.4.3/turbo_broccoli/bokeh.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,33 +110,33 @@
         }
 
     where the `{...}` dict contains the actual data, and whose structure
     depends on the precise type of `obj`.
 
     - `bokeh.plotting._figure.figure` or `bokeh.models.Model`:
 
-        {
-            "__bokeh__": {
-                "__type__": "generic",
-                "__version__": 1,
-                "content": {...},
-                "buffers": [...],
+            {
+                "__bokeh__": {
+                    "__type__": "generic",
+                    "__version__": 1,
+                    "content": {...},
+                    "buffers": [...],
+                }
             }
-        }
 
     - `bokeh.core.serialization.Buffer`: (for internal use)
 
-        {
-            "__bokeh__": {
-                "__type__": "buffer",
-                "__version__": 1,
-                "id": <str>,
-                "data": <bytes>,
+            {
+                "__bokeh__": {
+                    "__type__": "buffer",
+                    "__version__": 1,
+                    "id": <str>,
+                    "data": <bytes>,
+                }
             }
-        }
 
     """
     ENCODERS: List[Tuple[type, Callable[[Any], dict]]] = [
         (Buffer, _buffer_to_json),
         (Figure, _generic_to_json),
         (Model, _generic_to_json),
     ]
```

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/bytes.py` & `turbo_broccoli-2.4.3/turbo_broccoli/bytes.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/collections.py` & `turbo_broccoli-2.4.3/turbo_broccoli/collections.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/dataclass.py` & `turbo_broccoli-2.4.3/turbo_broccoli/dataclass.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/dict.py` & `turbo_broccoli-2.4.3/turbo_broccoli/dict.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/environment.py` & `turbo_broccoli-2.4.3/turbo_broccoli/environment.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/generic.py` & `turbo_broccoli-2.4.3/turbo_broccoli/generic.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/guard.py` & `turbo_broccoli-2.4.3/turbo_broccoli/guard.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,94 +74,93 @@
     l = [1, 2, 3]  # The elements of l must be stringable
     h = GuardedBlockHandler("out/foo")
     for x in h.guard(l):
         # At the begining of every iteration, h.result is guaranteed to be a
         # dict with key str(x) being None. The result of past iterations are
         # also in h.result
         h.result[x] = {"bar": int(x) + 1}
-    # now, h.result is {"1": {"bar": 2}, "2": {"bar": 3}, ...}
+    # now, h.result is {1: {"bar": 2}, 2: {"bar": 3}, ...}
     ```
 
     creates folder `out/foo` in which there will be files `1.json`, `2.json`,
     `3.json` respectively containing `{"bar": 2}`, `{"bar": 3}`, `{"bar": 4}`.
     Of course, if any of these files existed prior to running the `for` loop
     (e.g. `out/foo/2.json`), then the corresponding iteration (in that case `x
     = 2`) is skipped.
-
-    **Warning**: The `x` in the loop above are actually strings! More generally,
-    `h.guard(l)` actually iterates over `map(str, l)`.
     """
 
     name: Optional[str]
     result: Any = None
     output_path: Path
 
     def __init__(
         self, output_path: Union[str, Path], name: Optional[str] = None
     ) -> None:
         self.output_path = Path(output_path)
         self.name = name
 
-    def _guard_iter(self, iterable: Iterable[Any]) -> Generator:
+    def _guard_iter(
+        self, iterable: Iterable[Any]
+    ) -> Generator[Any, None, None]:
         """
         Internal implementation of a guarded loop. See
         `turbo_broccoli.guard.GuardedBlockHandler`'s documentation.
         """
         self.result = {}
         for x in iterable:
             sx = str(x)
             path = self.output_path / f"{sx}.json"
             if path.is_file():
-                self.result[sx] = load_json(path)
+                self.result[x] = load_json(path)
                 if self.name:
                     logging.debug(
                         f"Skipped guarded iteration '{self.name}'[{sx}]"
                     )
             else:
-                self.result[sx] = None
-                yield sx
-                if self.result[sx] is not None:
+                self.result[x] = None
+                yield x
+                if self.result[x] is not None:
                     path.parent.mkdir(parents=True, exist_ok=True)
-                    save_json(self.result[sx], path)
+                    save_json(self.result[x], path)
                     if self.name is not None:
                         logging.debug(
                             f"Saved guarded iteration '{self.name}'[{sx}] "
                             f"results to '{path}'"
                         )
 
-    def _guard_no_iter(self) -> Generator:
+    def _guard_no_iter(self) -> Generator[Any, None, None]:
         """
         Internal implementation of a guarded block. See
         `turbo_broccoli.guard.GuardedBlockHandler`'s documentation.
         """
         if self.output_path.is_file():
             self.result = load_json(self.output_path)
             if self.name:
                 logging.debug(f"Skipped guarded block '{self.name}'")
         else:
-            try:
-                yield self
-            finally:
-                if self.result is not None:
-                    self.output_path.parent.mkdir(parents=True, exist_ok=True)
-                    save_json(self.result, self.output_path)
-                    if self.name is not None:
-                        logging.debug(
-                            f"Saved guarded block '{self.name}' results to "
-                            f"'{self.output_path}'"
-                        )
+            yield self
+            if self.result is not None:
+                self.output_path.parent.mkdir(parents=True, exist_ok=True)
+                save_json(self.result, self.output_path)
+                if self.name is not None:
+                    logging.debug(
+                        f"Saved guarded block '{self.name}' results to "
+                        f"'{self.output_path}'"
+                    )
 
-    def guard(self, iterable: Optional[Iterable[Any]] = None) -> Generator:
+    def guard(
+        self, iterable: Optional[Iterable[Any]] = None
+    ) -> Generator[Any, None, None]:
         """See `turbo_broccoli.guard.GuardedBlockHandler`'s documentation"""
         self.output_path.parent.mkdir(parents=True, exist_ok=True)
         old_artifact_path = get_artifact_path()
         set_artifact_path(self.output_path.parent)
         if iterable is None:
-            for _ in self._guard_no_iter():
-                yield
+            for x in self._guard_no_iter():
+                yield x
         else:
             for x in self._guard_iter(iterable):
                 yield x
         set_artifact_path(old_artifact_path)
 
 
 def guarded_call(
```

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/keras.py` & `turbo_broccoli-2.4.3/turbo_broccoli/keras.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,14 +222,15 @@
 
 
 def _json_to_model(dct: dict) -> Any:
     """Converts a JSON document to a serializable keras object."""
     DECODERS = {
         1: _json_to_model_v1,
         2: _json_to_model_v2,
+        3: _json_to_model_v3,
     }
     return DECODERS[dct["__version__"]](dct)
 
 
 def _json_to_model_v1(dct: dict) -> Any:
     """
     Converts a JSON document to a keras model object following the v1
@@ -253,14 +254,24 @@
     if "model" in dct:
         return _json_to_model_v1(dct)
     return keras.models.load_model(
         get_artifact_path() / (dct["id"] + "." + dct["format"])
     )
 
 
+def _json_to_model_v3(dct: dict) -> Any:
+    """
+    Converts a JSON document to a keras model object following the v2
+    specification.
+    """
+    if "model" in dct:
+        return _json_to_model_v1(dct)
+    return keras.models.load_model(get_artifact_path() / dct["id"])
+
+
 def _json_to_optimizer(dct: dict) -> Any:
     """Converts a JSON document to a serializable keras object."""
     DECODERS = {
         1: _json_to_optimizer_v1,
     }
     return DECODERS[dct["__version__"]](dct)
 
@@ -295,18 +306,18 @@
             "loss": getattr(model, "loss", None),
             "metrics": getattr(model, "metrics", []),
             "model": keras.utils.serialize_keras_object(model),
             "optimizer": getattr(model, "optimizer", None),
             "weights": model.weights,
         }
     name = str(uuid4())
-    model.save(get_artifact_path() / (name + "." + fmt), save_format=fmt)
+    model.save(get_artifact_path() / name, save_format=fmt)
     return {
         "__type__": "model",
-        "__version__": 2,
+        "__version__": 3,
         "format": fmt,
         "id": name,
     }
 
 
 def from_json(dct: dict) -> Any:
     """
@@ -361,15 +372,15 @@
             }
 
       if `TB_KERAS_FORMAT` is `h5` or `tf`, the document will look like
 
             {
                 "__keras__": {
                     "__type__": "model",
-                    "__version__": 2,
+                    "__version__": 3,
                     "format": <str>,
                     "id": <UUID4 str>
                 }
             }
 
     """
     ENCODERS: List[Tuple[type, Callable[[Any], dict]]] = [
```

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/numpy.py` & `turbo_broccoli-2.4.3/turbo_broccoli/numpy.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/pandas.py` & `turbo_broccoli-2.4.3/turbo_broccoli/pandas.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/pytorch.py` & `turbo_broccoli-2.4.3/turbo_broccoli/pytorch.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/scipy.py` & `turbo_broccoli-2.4.3/turbo_broccoli/scipy.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,25 +78,26 @@
         }
 
     where the `{...}` dict contains the actual data, and whose structure
     depends on the precise type of `obj`.
 
     - [`csr_matrix`](https://docs.scipy.org/doc/scipy/reference/generated/scipy.sparse.csr_matrix.html#scipy.sparse.csr_matrix)
 
-        {
-            "__scipy__": {
-                "__type__": "csr_matrix",
-                "__version__": 1,
-                "data": ...,
-                "dtype": ...,
-                "indices": ...,
-                "indptr": ...,
-                "shape": ...,
+            {
+                "__scipy__": {
+                    "__type__": "csr_matrix",
+                    "__version__": 1,
+                    "data": ...,
+                    "dtype": ...,
+                    "indices": ...,
+                    "indptr": ...,
+                    "shape": ...,
+                }
             }
-        }
+
     """
     ENCODERS: List[Tuple[type, Callable[[Any], dict]]] = [
         (csr_matrix, _csr_matrix_to_json),
     ]
     for t, f in ENCODERS:
         if isinstance(obj, t):
             return {"__scipy__": f(obj)}
```

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/secret.py` & `turbo_broccoli-2.4.3/turbo_broccoli/secret.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,21 +113,20 @@
 
 
 def to_json(obj: Secret) -> dict:
     """
     Encrypts a JSON **string representation** of a secret document into a
     new JSON document with the following structure:
 
-            {
-                "__secret__": {
-                    "__version__": 1,
-                    "data": <encrypted bytes>,
-                }
+        {
+            "__secret__": {
+                "__version__": 1,
+                "data": <encrypted bytes>,
             }
-
+        }
     """
     if not isinstance(obj, Secret):
         raise TypeNotSupported()
     key = get_shared_key()
     if key is None:
         raise RuntimeError(
             "Attempting to serialize a secret type but no shared key is set. "
```

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/sklearn.py` & `turbo_broccoli-2.4.3/turbo_broccoli/sklearn.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/tensorflow.py` & `turbo_broccoli-2.4.3/turbo_broccoli/tensorflow.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli/turbo_broccoli.py` & `turbo_broccoli-2.4.3/turbo_broccoli/turbo_broccoli.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,13 +194,13 @@
     with open(path, mode="r", encoding="utf-8") as fp:
         return json.load(fp, cls=TurboBroccoliDecoder)
 
 
 def save_json(obj: Any, path: Union[str, Path]) -> None:
     """Serializes and saves a JSON-serializable object"""
     with open(path, mode="w", encoding="utf-8") as fp:
-        json.dump(obj, fp, cls=TurboBroccoliEncoder)
+        fp.write(to_json(obj))
 
 
 def to_json(obj: Any) -> str:
     """Converts an object to JSON"""
     return json.dumps(obj, cls=TurboBroccoliEncoder)
```

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli.egg-info/PKG-INFO` & `turbo_broccoli-2.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: turbo-broccoli
-Version: 2.3.8
+Name: turbo_broccoli
+Version: 2.4.3
 Summary: JSON (de)serialization extensions
 Home-page: https://github.com/altaris/turbo-broccoli
 Author: Cédric Ho Thanh
 Author-email: altaris@users.noreply.github.com
 Project-URL: Issues, https://github.com/altaris/turbo-broccoli/issues
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 ![License](https://img.shields.io/github/license/altaris/turbo-broccoli)
 [![Code
 style](https://img.shields.io/badge/style-black-black)](https://pypi.org/project/black)
 ![hehe](https://img.shields.io/badge/project%20name%20by-github-pink)
 [![Documentation](https://badgen.net/badge/documentation/here/green)](https://https://altaris.github.io/turbo-broccoli/turbo_broccoli.html)
 
 JSON (de)serialization extensions, originally aimed at `numpy` and `tensorflow`
-objects.
+objects, but now supporting a wide range of objects.
 
 # Installation
 
 ```sh
 pip install turbo-broccoli
 ```
 
@@ -80,15 +80,15 @@
 
 ## Supported types
 
 ### Basic types
 
 - [`bytes`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/bytes.html#to_json)
 
-- `dict` with non `str` keys
+- [`dict` with non `str` keys](https://altaris.github.io/turbo-broccoli/turbo_broccoli/dict.html#to_json)
 
 - [Collections](https://altaris.github.io/turbo-broccoli/turbo_broccoli/collections.html#to_json):
   `collections.deque`, `collections.namedtuple`
 
 - [Dataclasses](https://altaris.github.io/turbo-broccoli/turbo_broccoli/dataclass.html#to_json): serialization is straightforward:
   ```py
   @dataclass
@@ -413,15 +413,17 @@
   Comma-separated list of types to not deserialize, for example
   `bytes,numpy.ndarray`. Excludable types are:
 
   - `bokeh`, `bokeh.buffer`, `bokeh.generic`,
 
   - `bytes`,
 
-  - `dict`,
+  - `dict` (this will only disable [Turbo Broccoli's custom
+    serialization](https://altaris.github.io/turbo-broccoli/turbo_broccoli/dict.html#to_json)
+    of `dict`s with non `str` keys),
 
   - `collections`, `collections.deque`, `collections.namedtuple`,
 
   - `dataclass`, `dataclass.<dataclass_name>` (case sensitive),
 
   - `generic`,
 
@@ -457,14 +459,23 @@
 
 This is so cool. Check out
 [`turbo_broccoli.GuardedBlockHandler`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#GuardedBlockHandler),
 [`turbo_broccoli.guarded_call`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#guarded_call),
 and
 [`turbo_broccoli.produces_document`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#produces_document).
 
+## CLI
+
+Turbo Broccoli has a few utilities that can be accessed from the CLI.
+
+- `list-artifacts`: Prints all the artifacts filenames or file paths that are
+  referenced by a given json file.
+
+- `rm`: Removes a json file and all the artifacts it references.
+
 # Contributing
 
 ## Dependencies
 
 - `python3.9` or newer;
 
 - `requirements.txt` for runtime dependencies;
```

### Comparing `turbo_broccoli-2.3.8/turbo_broccoli.egg-info/SOURCES.txt` & `turbo_broccoli-2.4.3/turbo_broccoli.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 tests/test_pandas.py
 tests/test_pytorch.py
 tests/test_scipy.py
 tests/test_secret.py
 tests/test_sklearn.py
 tests/test_tensorflow.py
 turbo_broccoli/__init__.py
+turbo_broccoli/__main__.py
 turbo_broccoli/bokeh.py
 turbo_broccoli/bytes.py
 turbo_broccoli/collections.py
 turbo_broccoli/dataclass.py
 turbo_broccoli/dict.py
 turbo_broccoli/environment.py
 turbo_broccoli/generic.py
```

