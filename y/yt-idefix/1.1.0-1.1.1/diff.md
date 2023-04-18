# Comparing `tmp/yt_idefix-1.1.0.tar.gz` & `tmp/yt_idefix-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_idefix-1.1.0.tar", last modified: Sat Mar 18 13:37:16 2023, max compression
+gzip compressed data, was "yt_idefix-1.1.1.tar", last modified: Tue Apr 18 15:42:55 2023, max compression
```

## Comparing `yt_idefix-1.1.0.tar` & `yt_idefix-1.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:16.716275 yt_idefix-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-18 13:37:04.000000 yt_idefix-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-03-18 13:37:16.716275 yt_idefix-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-03-18 13:37:04.000000 yt_idefix-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-03-18 13:37:04.000000 yt_idefix-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-18 13:37:16.716275 yt_idefix-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:16.712275 yt_idefix-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/tests/test_C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/tests/test_dmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/tests/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/tests/test_vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/tests/test_xdmf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:16.712275 yt_idefix-1.1.0/yt_idefix/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:16.716275 yt_idefix-1.1.0/yt_idefix/_io/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/_io/C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/_io/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/_io/dmp_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/_io/h5_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/_io/vtk_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33685 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:05.000000 yt_idefix-1.1.0/yt_idefix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 13:37:16.716275 yt_idefix-1.1.0/yt_idefix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-03-18 13:37:16.000000 yt_idefix-1.1.0/yt_idefix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-18 13:37:16.000000 yt_idefix-1.1.0/yt_idefix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 13:37:16.000000 yt_idefix-1.1.0/yt_idefix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-18 13:37:16.000000 yt_idefix-1.1.0/yt_idefix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-18 13:37:16.000000 yt_idefix-1.1.0/yt_idefix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-18 13:37:16.000000 yt_idefix-1.1.0/yt_idefix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:55.339267 yt_idefix-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 15:42:42.000000 yt_idefix-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-18 15:42:55.339267 yt_idefix-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-18 15:42:42.000000 yt_idefix-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-18 15:42:42.000000 yt_idefix-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:42:55.339267 yt_idefix-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:55.339267 yt_idefix-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/tests/test_C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/tests/test_dmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/tests/test_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/tests/test_xdmf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:55.339267 yt_idefix-1.1.1/yt_idefix/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:55.339267 yt_idefix-1.1.1/yt_idefix/_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_io/C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_io/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_io/dmp_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_io/h5_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_io/vtk_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34032 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:44.000000 yt_idefix-1.1.1/yt_idefix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:42:55.339267 yt_idefix-1.1.1/yt_idefix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-18 15:42:55.000000 yt_idefix-1.1.1/yt_idefix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-18 15:42:55.000000 yt_idefix-1.1.1/yt_idefix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:42:55.000000 yt_idefix-1.1.1/yt_idefix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 15:42:55.000000 yt_idefix-1.1.1/yt_idefix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 15:42:55.000000 yt_idefix-1.1.1/yt_idefix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 15:42:55.000000 yt_idefix-1.1.1/yt_idefix.egg-info/top_level.txt
```

### Comparing `yt_idefix-1.1.0/LICENSE` & `yt_idefix-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.0/PKG-INFO` & `yt_idefix-1.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: yt_idefix
-Version: 1.1.0
+Version: 1.1.1
 Summary: An extension module for yt, adding a frontend for Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
 Keywords: astronomy astrophysics visualization amr adaptivemeshrefinement
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Matplotlib
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: AIX
 Classifier: Operating System :: POSIX :: Linux
@@ -36,15 +36,15 @@
 
 <!--- Tests and style --->
 [![CI](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml/badge.svg)](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/yt_idefix/main.svg)](https://results.pre-commit.ci/latest/github/neutrinoceros/yt_idefix/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
-A maturing yt frontend for Idefix and Pluto (vtk), packaged as an extension for yt.
+A maturing yt frontend for Idefix and Pluto, packaged as an extension for yt.
 
 ## Installation
 
 ```shell
 python -m pip install yt_idefix
 ```
 
@@ -52,17 +52,24 @@
 
 After importing `yt` itself, make sure to activate the extension
 ```python
 import yt
 import yt_idefix
 ```
 
-Now `yt.load` will be able to read Pluto/Idefix `.vtk` output files, as well as
-Idefix `.dmp` dump files.
+Now `yt.load` will be able to read Pluto/Idefix output files.
 
+## Supported formats
+
+| Code   | format | supported since | additional dependencies |
+|--------|:------:|:---------------:|-------------------------|
+| Idefix | `.dmp` | v0.1.0          |                         |
+| Idefix | `.vtk` | v0.3.0          |                         |
+| Pluto  | `.vtk` | v0.9.0          |                         |
+| Pluto  |  XDMF  | v1.1.0          | `h5py`                  |
 
 ## Experimental features
 
 ### Seamless plugin support
 *new in yt 4.2 (unreleased) + yt_idefix 0.16*
 
 `yt>=4.2` supports automatic
```

### Comparing `yt_idefix-1.1.0/README.md` & `yt_idefix-1.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 <!--- Tests and style --->
 [![CI](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml/badge.svg)](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/yt_idefix/main.svg)](https://results.pre-commit.ci/latest/github/neutrinoceros/yt_idefix/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
-A maturing yt frontend for Idefix and Pluto (vtk), packaged as an extension for yt.
+A maturing yt frontend for Idefix and Pluto, packaged as an extension for yt.
 
 ## Installation
 
 ```shell
 python -m pip install yt_idefix
 ```
 
@@ -22,17 +22,24 @@
 
 After importing `yt` itself, make sure to activate the extension
 ```python
 import yt
 import yt_idefix
 ```
 
-Now `yt.load` will be able to read Pluto/Idefix `.vtk` output files, as well as
-Idefix `.dmp` dump files.
+Now `yt.load` will be able to read Pluto/Idefix output files.
 
+## Supported formats
+
+| Code   | format | supported since | additional dependencies |
+|--------|:------:|:---------------:|-------------------------|
+| Idefix | `.dmp` | v0.1.0          |                         |
+| Idefix | `.vtk` | v0.3.0          |                         |
+| Pluto  | `.vtk` | v0.9.0          |                         |
+| Pluto  |  XDMF  | v1.1.0          | `h5py`                  |
 
 ## Experimental features
 
 ### Seamless plugin support
 *new in yt 4.2 (unreleased) + yt_idefix 0.16*
 
 `yt>=4.2` supports automatic
```

### Comparing `yt_idefix-1.1.0/pyproject.toml` & `yt_idefix-1.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 requires = [
     "setuptools>=61.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yt_idefix"
-version = "1.1.0"
+version = "1.1.1"
 description = "An extension module for yt, adding a frontend for Idefix"
 authors = [
     { name = "C.M.T. Robert" },
 ]
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Framework :: Matplotlib",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: AIX",
     "Operating System :: POSIX :: Linux",
```

### Comparing `yt_idefix-1.1.0/tests/test_C_io.py` & `yt_idefix-1.1.1/tests/test_C_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.0/tests/test_dmp.py` & `yt_idefix-1.1.1/tests/test_dmp.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.0/tests/test_loading.py` & `yt_idefix-1.1.1/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.0/tests/test_vtk.py` & `yt_idefix-1.1.1/tests/test_vtk.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.0/tests/test_xdmf.py` & `yt_idefix-1.1.1/tests/test_xdmf.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.0/yt_idefix/_backports.py` & `yt_idefix-1.1.1/yt_idefix/_backports.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.0/yt_idefix/_io/commons.py` & `yt_idefix-1.1.1/yt_idefix/_io/commons.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.0/yt_idefix/_io/dmp_io.py` & `yt_idefix-1.1.1/yt_idefix/_io/dmp_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.0/yt_idefix/_io/h5_io.py` & `yt_idefix-1.1.1/yt_idefix/_io/h5_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.0/yt_idefix/_io/vtk_io.py` & `yt_idefix-1.1.1/yt_idefix/_io/vtk_io.py`

 * *Files 7% similar despite different names*

```diff
@@ -96,25 +96,26 @@
         for _ in range(nfield):
             d = next(fh).decode()
             if d.startswith("GEOMETRY"):
                 geom_flag: int = struct.unpack(">i", fh.read(4))[0]
                 geometry_from_data = KNOWN_GEOMETRIES.get(geom_flag)
                 if geometry_from_data is None:
                     warnings.warn(
-                        f"Unknown geometry enum value {geom_flag}, please report this."
+                        f"Unknown geometry enum value {geom_flag}, please report this.",
+                        stacklevel=2,
                     )
                 metadata["geometry"] = geometry_from_data
             elif d.startswith("TIME"):
                 metadata["time"] = struct.unpack(">f", fh.read(4))[0]
             elif d.startswith("PERIODICITY"):
                 metadata["periodicity"] = tuple(
                     np.fromfile(fh, dtype=">i4", count=3).astype(bool)
                 )
             else:
-                warnings.warn(f"Found unknown field {d!r}")
+                warnings.warn(f"Found unknown field {d!r}", stacklevel=2)
             next(fh)  # skip extra linefeed (empty line)
         parse_shape(next(fh).decode(), metadata)
 
     elif line.startswith("DIMENSIONS"):
         parse_shape(line, metadata)
 
     else:
@@ -126,15 +127,14 @@
 def read_grid_coordinates(
     fh: BinaryIO,
     *,
     geometry: str | None = None,
 ) -> Coordinates:
     # Return cell edges coordinates
 
-    fh.seek(0)
     md = read_metadata(fh)
 
     geometry = md.get("geometry", geometry)
     if geometry not in (valid_geometries := tuple(KNOWN_GEOMETRIES.values())):
         raise ValueError(
             f"Got unknown geometry {geometry!r}, expected one of {valid_geometries}"
         )
@@ -158,20 +158,22 @@
             if point_type == "POINT_DATA":
                 # raw data is cell center coords, extrapolation would be needed here
                 # However it's probably never going to be worth it since this branch
                 # corresponds to Idefix < 0.8 and should never be hit in practice.
                 # Raising a warning should suffice
                 warnings.warn(
                     "point_type=POINT_DATA case is not fully supported. "
-                    "Domain edges will be slightly off."
+                    "Domain edges will be slightly off.",
+                    stacklevel=2,
                 )
             else:
                 warnings.warn(
                     f"Got unexpected value point_type={point_type!r}. "
-                    "Results are not guaranteed."
+                    "Results are not guaranteed.",
+                    stacklevel=2,
                 )
             array_shape = shape
 
     else:
         assert geometry in ("polar", "spherical")
         rshape = Shape(*reversed(shape))
         npoints = int(next(fh).decode().split()[1])  # POINTS NXNYNZ float
@@ -198,29 +200,29 @@
 
         array_shape = shape.to_cell_centered()
         assert data_type == "CELL_DATA"
 
     return Coordinates(coords[0], coords[1], coords[2], array_shape)
 
 
-def read_field_offset_index(fh: BinaryIO, shape: Shape) -> dict[str, int]:
+def read_field_offset_index(
+    fh: BinaryIO, shape: Shape, *, upper_case_varnames: bool
+) -> dict[str, int]:
     # assuming fh is correctly positioned (read_grid_coordinates must be called first)
     retv: dict[str, int] = {}
 
     while True:
         line = fh.readline()
         if len(line) < 2:
             break
         s = line.decode()
         datatype, varname, dtype = s.split()
 
-        # some versions of Pluto define field names in lower case
-        # so we normalize to upper case to avoid duplicating data
-        # in IdefixVtkFieldInfo.known_other_fields
-        varname = varname.upper()
+        if upper_case_varnames:
+            varname = varname.upper()
 
         if datatype == "SCALARS":
             next(fh)
             retv[varname] = fh.tell()
             read_single_field(fh, shape=shape, skip_data=True)
         elif datatype == "VECTORS":
             for axis in "XYZ":
```

### Comparing `yt_idefix-1.1.0/yt_idefix/data_structures.py` & `yt_idefix-1.1.1/yt_idefix/data_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,15 +411,16 @@
         if from_input:
             if from_disk and from_input and from_input != from_disk:
                 warnings.warn(
                     "Geometries from disk and input do not match, got\n"
                     f" - {from_disk!r} (from disk)\n"
                     f" - {from_input!r} (from input)\n"
                     "input prevails to allow working around hypothetical parsing bugs, "
-                    "but it is very likely to result in an error in the general case."
+                    "but it is very likely to result in an error in the general case.",
+                    stacklevel=2,
                 )
             geom_str = from_input
         else:
             assert from_disk
             geom_str = from_disk
 
         def parse_geometry(geom: str):
@@ -486,15 +487,16 @@
         # lines, which is general enough for the data formats we support
         lines = self._read_data_header().splitlines()
         header = "\n".join(lines[: (min(len(lines), 2))])
         regexp = self.__class__._version_regexp
         match = re.search(regexp, header)
         if match is None:
             warnings.warn(
-                f"Could not determine code version from file header {header!r}"
+                f"Could not determine code version from file header {header!r}",
+                stacklevel=2,
             )
             return "unknown"
 
         return match.group()
 
 
 class IdefixDataset(GoodboyDataset, ABC):
@@ -719,19 +721,24 @@
         with open(self.filename, "rb") as fh:
             md = vtk_io.read_metadata(fh)
         self.parameters.update(md)
 
         super()._parse_parameter_file()
         # from here self.geometry is assumed to be set
 
+        # some versions of Pluto define field names in lower case
+        # so we normalize to upper case to avoid duplicating data
+        # in BaseVtkFields.known_other_fields
+        normalize_varnames = self.dataset_type == "pluto-vtk"
+
         # parse the grid
         with open(self.filename, "rb") as fh:
             coords = vtk_io.read_grid_coordinates(fh, geometry=self.geometry)
             self._field_offset_index = vtk_io.read_field_offset_index(
-                fh, coords.array_shape
+                fh, coords.array_shape, upper_case_varnames=normalize_varnames
             )
         self._detected_field_list = list(self._field_offset_index.keys())
 
         self.domain_dimensions = np.array(coords.array_shape)
         self.dimensionality = np.count_nonzero(self.domain_dimensions - 1)
 
         dle = np.array([arr.min() for arr in coords.arrays], dtype="float64")
```

### Comparing `yt_idefix-1.1.0/yt_idefix/definitions.py` & `yt_idefix-1.1.1/yt_idefix/definitions.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.0/yt_idefix/fields.py` & `yt_idefix-1.1.1/yt_idefix/fields.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.0/yt_idefix/io.py` & `yt_idefix-1.1.1/yt_idefix/io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-1.1.0/yt_idefix.egg-info/PKG-INFO` & `yt_idefix-1.1.1/yt_idefix.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: yt-idefix
-Version: 1.1.0
+Version: 1.1.1
 Summary: An extension module for yt, adding a frontend for Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
 Keywords: astronomy astrophysics visualization amr adaptivemeshrefinement
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Matplotlib
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: AIX
 Classifier: Operating System :: POSIX :: Linux
@@ -36,15 +36,15 @@
 
 <!--- Tests and style --->
 [![CI](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml/badge.svg)](https://github.com/neutrinoceros/yt_idefix/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/yt_idefix/main.svg)](https://results.pre-commit.ci/latest/github/neutrinoceros/yt_idefix/main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
-A maturing yt frontend for Idefix and Pluto (vtk), packaged as an extension for yt.
+A maturing yt frontend for Idefix and Pluto, packaged as an extension for yt.
 
 ## Installation
 
 ```shell
 python -m pip install yt_idefix
 ```
 
@@ -52,17 +52,24 @@
 
 After importing `yt` itself, make sure to activate the extension
 ```python
 import yt
 import yt_idefix
 ```
 
-Now `yt.load` will be able to read Pluto/Idefix `.vtk` output files, as well as
-Idefix `.dmp` dump files.
+Now `yt.load` will be able to read Pluto/Idefix output files.
 
+## Supported formats
+
+| Code   | format | supported since | additional dependencies |
+|--------|:------:|:---------------:|-------------------------|
+| Idefix | `.dmp` | v0.1.0          |                         |
+| Idefix | `.vtk` | v0.3.0          |                         |
+| Pluto  | `.vtk` | v0.9.0          |                         |
+| Pluto  |  XDMF  | v1.1.0          | `h5py`                  |
 
 ## Experimental features
 
 ### Seamless plugin support
 *new in yt 4.2 (unreleased) + yt_idefix 0.16*
 
 `yt>=4.2` supports automatic
```

### Comparing `yt_idefix-1.1.0/yt_idefix.egg-info/SOURCES.txt` & `yt_idefix-1.1.1/yt_idefix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

