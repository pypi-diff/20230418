# Comparing `tmp/pixelsort-cli-0.1.4.tar.gz` & `tmp/pixelsort-cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelsort-cli-0.1.4.tar", last modified: Fri Apr  7 19:35:52 2023, max compression
+gzip compressed data, was "pixelsort-cli-0.1.6.tar", last modified: Tue Apr 18 21:10:10 2023, max compression
```

## Comparing `pixelsort-cli-0.1.4.tar` & `pixelsort-cli-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dionysus  (1000) wheel      (998)        0 2023-04-07 19:35:52.647276 pixelsort-cli-0.1.4/
--rw-r--r--   0 dionysus  (1000) wheel      (998)     1072 2023-04-02 00:49:40.000000 pixelsort-cli-0.1.4/LICENSE
--rw-r--r--   0 dionysus  (1000) wheel      (998)     2043 2023-04-07 19:35:52.647276 pixelsort-cli-0.1.4/PKG-INFO
--rw-r--r--   0 dionysus  (1000) wheel      (998)     1490 2023-04-07 18:46:29.000000 pixelsort-cli-0.1.4/README.md
--rw-r--r--   0 dionysus  (1000) wheel      (998)      884 2023-04-07 19:35:30.000000 pixelsort-cli-0.1.4/pyproject.toml
--rw-r--r--   0 dionysus  (1000) wheel      (998)       38 2023-04-07 19:35:52.647276 pixelsort-cli-0.1.4/setup.cfg
--rw-r--r--   0 dionysus  (1000) wheel      (998)       69 2023-04-07 16:41:27.000000 pixelsort-cli-0.1.4/setup.py
-drwxr-xr-x   0 dionysus  (1000) wheel      (998)        0 2023-04-07 19:35:52.647276 pixelsort-cli-0.1.4/src/
-drwxr-xr-x   0 dionysus  (1000) wheel      (998)        0 2023-04-07 19:35:52.647276 pixelsort-cli-0.1.4/src/pixelsort/
--rw-r--r--   0 dionysus  (1000) wheel      (998)      115 2023-04-07 16:35:52.000000 pixelsort-cli-0.1.4/src/pixelsort/__init__.py
--rw-r--r--   0 dionysus  (1000) wheel      (998)     2016 2023-04-07 19:32:19.000000 pixelsort-cli-0.1.4/src/pixelsort/__main__.py
--rw-r--r--   0 dionysus  (1000) wheel      (998)     1470 2023-04-07 16:36:33.000000 pixelsort-cli-0.1.4/src/pixelsort/cli.py
--rw-r--r--   0 dionysus  (1000) wheel      (998)      231 2023-04-07 16:36:51.000000 pixelsort-cli-0.1.4/src/pixelsort/direction.py
--rw-r--r--   0 dionysus  (1000) wheel      (998)     4494 2023-04-07 19:31:41.000000 pixelsort-cli-0.1.4/src/pixelsort/image.py
-drwxr-xr-x   0 dionysus  (1000) wheel      (998)        0 2023-04-07 19:35:52.647276 pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/
--rw-r--r--   0 dionysus  (1000) wheel      (998)     2043 2023-04-07 19:35:52.000000 pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/PKG-INFO
--rw-r--r--   0 dionysus  (1000) wheel      (998)      431 2023-04-07 19:35:52.000000 pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/SOURCES.txt
--rw-r--r--   0 dionysus  (1000) wheel      (998)        1 2023-04-07 19:35:52.000000 pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/dependency_links.txt
--rw-r--r--   0 dionysus  (1000) wheel      (998)       54 2023-04-07 19:35:52.000000 pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/entry_points.txt
--rw-r--r--   0 dionysus  (1000) wheel      (998)       44 2023-04-07 19:35:52.000000 pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/requires.txt
--rw-r--r--   0 dionysus  (1000) wheel      (998)       10 2023-04-07 19:35:52.000000 pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/top_level.txt
-drwxr-xr-x   0 dionysus  (1000) wheel      (998)        0 2023-04-07 19:35:52.647276 pixelsort-cli-0.1.4/test/
--rw-r--r--   0 dionysus  (1000) wheel      (998)      384 2023-04-07 17:01:38.000000 pixelsort-cli-0.1.4/test/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:10.591190 pixelsort-cli-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-18 21:10:10.591190 pixelsort-cli-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:10:10.591190 pixelsort-cli-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:10.587190 pixelsort-cli-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:10.591190 pixelsort-cli-0.1.6/src/pixelsort/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/src/pixelsort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/src/pixelsort/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/src/pixelsort/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/src/pixelsort/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/src/pixelsort/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:10.591190 pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-18 21:10:10.000000 pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-18 21:10:10.000000 pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:10:10.000000 pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-18 21:10:10.000000 pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-18 21:10:10.000000 pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 21:10:10.000000 pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:10.591190 pixelsort-cli-0.1.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-18 21:09:59.000000 pixelsort-cli-0.1.6/test/test_image.py
```

### Comparing `pixelsort-cli-0.1.4/LICENSE` & `pixelsort-cli-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelsort-cli-0.1.4/PKG-INFO` & `pixelsort-cli-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: pixelsort-cli
-Version: 0.1.4
+Version: 0.1.6
 Summary: A Python CLI tool for sorting pixels in images.
 Author-email: Ferdinand Theil <f.p.theil@proton.me>
 Project-URL: Homepage, https://github.com/Blotz/pixelsort-cli
 Project-URL: Bug Tracker, https://github.com/Blotz/pixelsort-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # pixelsort cli
 
+![tests](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-package.yml/badge.svg)
+![package](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-publish.yml/badge.svg)
+
 A simple python command line tool for sort pixels in an image.
 Based on the works of [Kim Asendorf](https://github.com/kimasendorf/ASDFPixelSort).
 
 The script blocks pixels into dark and light areas using a contrast mask.
 Then it sorts the pixels in a given direction via their luminance.
 
 - You can increase/decrease the contrast by setting the threshold.
```

### Comparing `pixelsort-cli-0.1.4/README.md` & `pixelsort-cli-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # pixelsort cli
 
+![tests](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-package.yml/badge.svg)
+![package](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-publish.yml/badge.svg)
+
 A simple python command line tool for sort pixels in an image.
 Based on the works of [Kim Asendorf](https://github.com/kimasendorf/ASDFPixelSort).
 
 The script blocks pixels into dark and light areas using a contrast mask.
 Then it sorts the pixels in a given direction via their luminance.
 
 - You can increase/decrease the contrast by setting the threshold.
```

### Comparing `pixelsort-cli-0.1.4/pyproject.toml` & `pixelsort-cli-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pixelsort-cli"
-version = "0.1.4"
+version = "0.1.6"
 authors = [
     {name = "Ferdinand Theil", email = "f.p.theil@proton.me"},
 ]
 description = "A Python CLI tool for sorting pixels in images."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -35,8 +35,8 @@
 ]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 testpaths = [
     "tests"
-]
+]
```

### Comparing `pixelsort-cli-0.1.4/src/pixelsort/__main__.py` & `pixelsort-cli-0.1.6/src/pixelsort/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     # process image
     image.process_image(image_data, direction, threshold, invert, reversed_direction)
 
     # save image
     if output_path is None:
         # show image if no output path is given
-        image.show_image(image_data)
+        return image.show_image(image_data)
 
     # Parse output path
     output_path = pathlib.Path(output_path)
     if not cli.valid_write_image_path(output_path):
         sys.exit(-1)
 
     cv2.imwrite(str(output_path), image_data)
```

### Comparing `pixelsort-cli-0.1.4/src/pixelsort/cli.py` & `pixelsort-cli-0.1.6/src/pixelsort/cli.py`

 * *Files identical despite different names*

### Comparing `pixelsort-cli-0.1.4/src/pixelsort/image.py` & `pixelsort-cli-0.1.6/src/pixelsort/image.py`

 * *Files identical despite different names*

### Comparing `pixelsort-cli-0.1.4/src/pixelsort_cli.egg-info/PKG-INFO` & `pixelsort-cli-0.1.6/src/pixelsort_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: pixelsort-cli
-Version: 0.1.4
+Version: 0.1.6
 Summary: A Python CLI tool for sorting pixels in images.
 Author-email: Ferdinand Theil <f.p.theil@proton.me>
 Project-URL: Homepage, https://github.com/Blotz/pixelsort-cli
 Project-URL: Bug Tracker, https://github.com/Blotz/pixelsort-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # pixelsort cli
 
+![tests](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-package.yml/badge.svg)
+![package](https://github.com/Blotz/pixelsort-cli/actions/workflows/python-publish.yml/badge.svg)
+
 A simple python command line tool for sort pixels in an image.
 Based on the works of [Kim Asendorf](https://github.com/kimasendorf/ASDFPixelSort).
 
 The script blocks pixels into dark and light areas using a contrast mask.
 Then it sorts the pixels in a given direction via their luminance.
 
 - You can increase/decrease the contrast by setting the threshold.
```

