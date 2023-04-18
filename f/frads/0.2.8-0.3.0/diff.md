# Comparing `tmp/frads-0.2.8.tar.gz` & `tmp/frads-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frads-0.2.8.tar", last modified: Thu Oct 27 19:48:50 2022, max compression
+gzip compressed data, was "frads-0.3.0.tar", last modified: Tue Apr 18 20:38:14 2023, max compression
```

## Comparing `frads-0.2.8.tar` & `frads-0.3.0.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:48:50.121840 frads-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-10-27 19:48:40.000000 frads-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8941 2022-10-27 19:48:50.121840 frads-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6196 2022-10-27 19:48:40.000000 frads-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:48:50.117840 frads-0.2.8/frads/
--rwxr-xr-x   0 runner    (1001) docker     (121)     4156 2022-10-27 19:48:40.000000 frads-0.2.8/frads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33347 2022-10-27 19:48:40.000000 frads-0.2.8/frads/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     6722 2022-10-27 19:48:40.000000 frads-0.2.8/frads/color.py
--rw-r--r--   0 runner    (1001) docker     (121)    60540 2022-10-27 19:48:40.000000 frads-0.2.8/frads/color_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:48:50.117840 frads-0.2.8/frads/data/
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-10-27 19:48:40.000000 frads-0.2.8/frads/data/WC.DAT
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-10-27 19:48:40.000000 frads-0.2.8/frads/data/mrad_default.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)    21391 2022-10-27 19:48:40.000000 frads-0.2.8/frads/epjson2rad.py
--rw-r--r--   0 runner    (1001) docker     (121)    19402 2022-10-27 19:48:40.000000 frads-0.2.8/frads/gencolorsky.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15936 2022-10-27 19:48:40.000000 frads-0.2.8/frads/geom.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12083 2022-10-27 19:48:40.000000 frads-0.2.8/frads/matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    36345 2022-10-27 19:48:40.000000 frads-0.2.8/frads/methods.py
--rw-r--r--   0 runner    (1001) docker     (121)     8799 2022-10-27 19:48:40.000000 frads-0.2.8/frads/mtxmult.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17474 2022-10-27 19:48:40.000000 frads-0.2.8/frads/ncp.py
--rw-r--r--   0 runner    (1001) docker     (121)    18997 2022-10-27 19:48:40.000000 frads-0.2.8/frads/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     7098 2022-10-27 19:48:40.000000 frads-0.2.8/frads/raycall.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7473 2022-10-27 19:48:40.000000 frads-0.2.8/frads/room.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15429 2022-10-27 19:48:40.000000 frads-0.2.8/frads/sky.py
--rw-r--r--   0 runner    (1001) docker     (121)    16402 2022-10-27 19:48:40.000000 frads-0.2.8/frads/types.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    22593 2022-10-27 19:48:40.000000 frads-0.2.8/frads/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:48:50.117840 frads-0.2.8/frads.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8941 2022-10-27 19:48:50.000000 frads-0.2.8/frads.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-10-27 19:48:50.000000 frads-0.2.8/frads.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 19:48:50.000000 frads-0.2.8/frads.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-10-27 19:48:50.000000 frads-0.2.8/frads.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 19:48:49.000000 frads-0.2.8/frads.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-27 19:48:50.000000 frads-0.2.8/frads.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-27 19:48:40.000000 frads-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-10-27 19:48:50.125841 frads-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:48:50.121840 frads-0.2.8/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 19:48:50.121840 frads-0.2.8/test/Resources/
--rw-r--r--   0 runner    (1001) docker     (121)  1640229 2022-10-27 19:48:40.000000 frads-0.2.8/test/Resources/USA_CA_Oakland.Intl.AP.724930_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (121)   449366 2022-10-27 19:48:40.000000 frads-0.2.8/test/Resources/blinds30.xml
--rw-r--r--   0 runner    (1001) docker     (121)   846532 2022-10-27 19:48:40.000000 frads-0.2.8/test/Resources/klems_aniso_high.xml
--rw-r--r--   0 runner    (1001) docker     (121)   150134 2022-10-27 19:48:40.000000 frads-0.2.8/test/Resources/oak.wea
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-10-27 19:48:40.000000 frads-0.2.8/test/Resources/test.wea
--rw-r--r--   0 runner    (1001) docker     (121)     2868 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_color.py
--rw-r--r--   0 runner    (1001) docker     (121)     1820 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_epjson2rad.py
--rw-r--r--   0 runner    (1001) docker     (121)     1652 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (121)     2478 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_mtxmult.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_ncp.py
--rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_raycall.py
--rw-r--r--   0 runner    (1001) docker     (121)     4137 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_sky.py
--rw-r--r--   0 runner    (1001) docker     (121)     4841 2022-10-27 19:48:40.000000 frads-0.2.8/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:38:14.585332 frads-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-18 20:38:01.000000 frads-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-04-18 20:38:14.585332 frads-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-18 20:38:01.000000 frads-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:38:14.577332 frads-0.3.0/frads/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4088 2023-04-18 20:38:01.000000 frads-0.3.0/frads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33367 2023-04-18 20:38:01.000000 frads-0.3.0/frads/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-18 20:38:01.000000 frads-0.3.0/frads/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60540 2023-04-18 20:38:01.000000 frads-0.3.0/frads/color_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:38:14.577332 frads-0.3.0/frads/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-18 20:38:01.000000 frads-0.3.0/frads/data/WC.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-18 20:38:01.000000 frads-0.3.0/frads/data/mrad_default.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23025 2023-04-18 20:38:01.000000 frads-0.3.0/frads/epjson2rad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20889 2023-04-18 20:38:01.000000 frads-0.3.0/frads/eprad.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15845 2023-04-18 20:38:01.000000 frads-0.3.0/frads/geom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14588 2023-04-18 20:38:01.000000 frads-0.3.0/frads/matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37712 2023-04-18 20:38:01.000000 frads-0.3.0/frads/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-04-18 20:38:01.000000 frads-0.3.0/frads/mtxmult.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17474 2023-04-18 20:38:01.000000 frads-0.3.0/frads/ncp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-04-18 20:38:01.000000 frads-0.3.0/frads/parsers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7473 2023-04-18 20:38:01.000000 frads-0.3.0/frads/room.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20846 2023-04-18 20:38:01.000000 frads-0.3.0/frads/sky.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-04-18 20:38:01.000000 frads-0.3.0/frads/types.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19079 2023-04-18 20:38:01.000000 frads-0.3.0/frads/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-04-18 20:38:01.000000 frads-0.3.0/frads/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:38:14.577332 frads-0.3.0/frads.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-04-18 20:38:14.000000 frads-0.3.0/frads.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-18 20:38:14.000000 frads-0.3.0/frads.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:38:14.000000 frads-0.3.0/frads.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-18 20:38:14.000000 frads-0.3.0/frads.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:38:14.000000 frads-0.3.0/frads.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-18 20:38:14.000000 frads-0.3.0/frads.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 20:38:14.000000 frads-0.3.0/frads.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-18 20:38:01.000000 frads-0.3.0/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-18 20:38:01.000000 frads-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-18 20:38:14.585332 frads-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:38:14.581332 frads-0.3.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:38:14.585332 frads-0.3.0/test/Resources/
+-rw-r--r--   0 runner    (1001) docker     (123)  1640229 2023-04-18 20:38:01.000000 frads-0.3.0/test/Resources/USA_CA_Oakland.Intl.AP.724930_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)   449366 2023-04-18 20:38:01.000000 frads-0.3.0/test/Resources/blinds30.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   846532 2023-04-18 20:38:01.000000 frads-0.3.0/test/Resources/klems_aniso_high.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   150134 2023-04-18 20:38:01.000000 frads-0.3.0/test/Resources/oak.wea
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-18 20:38:01.000000 frads-0.3.0/test/Resources/test.wea
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_epjson2rad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_mtxmult.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_ncp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_sky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-18 20:38:01.000000 frads-0.3.0/test/test_window.py
```

### Comparing `frads-0.2.8/PKG-INFO` & `frads-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: frads
-Version: 0.2.8
-Summary: Wrapper for Radiance simulation control
+Version: 0.3.0
+Summary: Wrapper for Radiance related simulation workflows
 License: BSD 3-Clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 
 ![Install + Test](https://github.com/LBNL-ETA/frads/actions/workflows/main.yml/badge.svg)
-![CodeQL](https://github.com/LBNL-ETA/frads/actions/workflows/codeql-analysis.yml/badge.svg)
 [![Upload Python Package](https://github.com/LBNL-ETA/frads/actions/workflows/python-publish.yml/badge.svg)](https://github.com/LBNL-ETA/frads/actions/workflows/python-publish.yml)
+![Downloads](https://img.shields.io/pypi/dm/frads.svg)
 # _frads_: Framework for Radiance simulation control
 
 This is the repository for _frads_ development. Radiance is a free and open-source, raytracing-based lighting engine that is used extensively by engineering firms for innovative solar control, lighting, and daylighting design to improve the energy efficiency of buildings. With matrix algebraic methods, climate-based annual simulations can now be conducted in less than two minutes. _frads_ automates setup of these simulations by providing end users with an open-source, high-level abstraction of the Radiance command-line workflow (Unix toolbox model), helping to reduce the steep learning curve and associated user errors. _frads_ also provides the necessary infrastructure needed for seamless integration of Radiance and other modeling tools, such as EnergyPlus.
 
 [Documentation](https://lbnl-eta.github.io/frads/)
 
 ## Contact/ Support
@@ -43,29 +43,14 @@
 
 	$ python
 	Python 3.X.X
 	[GCC 4.x] on linux
 	Type "help", "copyright", "credits" or "license" for more information.
 	>>>
 
-### Install Radiance
-
-If you haven't already, you will need to install Radiance. `frads` will check your Radiance
-installation, so make sure you install it first.
-
-To install Radiance, visit Radiance Github [repo](https://github.com/LBNL-ETA/Radiance/releases)
- to download the latest release for your operating system.
-
-You can verify that Radiance is installed properly by typing in the command-line:
-
-```
-$ rtrace -version
-RADIANCE 5.4a ...
-```
-
 ### Install frads
 
 After you have Python installed, you should have `pip` command available in your shell environment as well. You can then use `pip` to install `frads`:
 
 	$ python -m pip install frads
 
 Alternatively, more recent version of `frads` can be installed directly from github as well. Watch for the passing/failed tag on github to check if the current version passed the tests.:
```

### Comparing `frads-0.2.8/README.md` & `frads-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![Install + Test](https://github.com/LBNL-ETA/frads/actions/workflows/main.yml/badge.svg)
-![CodeQL](https://github.com/LBNL-ETA/frads/actions/workflows/codeql-analysis.yml/badge.svg)
 [![Upload Python Package](https://github.com/LBNL-ETA/frads/actions/workflows/python-publish.yml/badge.svg)](https://github.com/LBNL-ETA/frads/actions/workflows/python-publish.yml)
+![Downloads](https://img.shields.io/pypi/dm/frads.svg)
 # _frads_: Framework for Radiance simulation control
 
 This is the repository for _frads_ development. Radiance is a free and open-source, raytracing-based lighting engine that is used extensively by engineering firms for innovative solar control, lighting, and daylighting design to improve the energy efficiency of buildings. With matrix algebraic methods, climate-based annual simulations can now be conducted in less than two minutes. _frads_ automates setup of these simulations by providing end users with an open-source, high-level abstraction of the Radiance command-line workflow (Unix toolbox model), helping to reduce the steep learning curve and associated user errors. _frads_ also provides the necessary infrastructure needed for seamless integration of Radiance and other modeling tools, such as EnergyPlus.
 
 [Documentation](https://lbnl-eta.github.io/frads/)
 
 ## Contact/ Support
@@ -34,29 +34,14 @@
 
 	$ python
 	Python 3.X.X
 	[GCC 4.x] on linux
 	Type "help", "copyright", "credits" or "license" for more information.
 	>>>
 
-### Install Radiance
-
-If you haven't already, you will need to install Radiance. `frads` will check your Radiance
-installation, so make sure you install it first.
-
-To install Radiance, visit Radiance Github [repo](https://github.com/LBNL-ETA/Radiance/releases)
- to download the latest release for your operating system.
-
-You can verify that Radiance is installed properly by typing in the command-line:
-
-```
-$ rtrace -version
-RADIANCE 5.4a ...
-```
-
 ### Install frads
 
 After you have Python installed, you should have `pip` command available in your shell environment as well. You can then use `pip` to install `frads`:
 
 	$ python -m pip install frads
 
 Alternatively, more recent version of `frads` can be installed directly from github as well. Watch for the passing/failed tag on github to check if the current version passed the tests.:
```

### Comparing `frads-0.2.8/frads/__init__.py` & `frads-0.3.0/frads/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,47 +46,59 @@
 manual- and automatically-controlled shading and daylighting systems
 or other site and building features that can change parametrically
 or on a time-step basis.
 """
 
 import logging
 import shutil
-import subprocess as sp
+
+from .epjson2rad import epjson2rad
+
+from .eprad import load_epmodel, EnergyPlusSetup, ep_datetime_parser
 
 from .matrix import (
+    load_matrix,
+    multiply_rgb,
     rfluxmtx,
     surface_as_sender,
     points_as_sender,
     view_as_sender,
     surface_as_receiver,
     sun_as_receiver,
     sky_as_receiver,
 )
 
 from .parsers import (
-    parse_primitive,
     parse_epw,
     parse_wea,
     parse_polygon,
+    parse_mrad_config,
 )
 
-from .raycall import oconv, rtrace, render
+from .methods import assemble_model, three_phase
 
-from .sky import basis_glow, gen_perez_sky
+from .sky import (
+    basis_glow,
+    gen_perez_sky,
+    genskymtx,
+    WeaData,
+    WeaMetaData,
+)
 
 from .types import (
     Primitive,
     View,
-    WeaData,
-    WeaMetaData,
 )
 
+
 from .utils import gen_grid, unpack_primitives
 
-__version__ = "0.2.8"
+from .window import GlazingSystem, AIR, ARGON, KRYPTON, XENON
+
+__version__ = "0.3.0"
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 # Check if Radiance is installed more or less
 rad_progs = [
     "rfluxmtx",
     "total",
@@ -99,48 +111,43 @@
 ]
 
 for prog in rad_progs:
     ppath = shutil.which(prog)
     if ppath is None:
         logger.info("%s not found; check Radiance installation", prog)
 
-try:
-    # Check Radiance version, need to be at least 5.X
-    version_check: str = sp.run(
-        ["rtrace", "-version"],
-        check=True,
-        stdout=sp.PIPE,
-        encoding="ascii",
-    ).stdout
-    try:
-        rad_version = float(version_check.split()[1][:3])
-        if rad_version < 5.3:
-            logger.critical("Please upgrade to Radiance version 5.3 or later")
-    except ValueError:
-        logger.critical(version_check)
-except FileNotFoundError as err:
-    logger.critical(err)
 
 __all__ = [
+    "AIR",
+    "ARGON",
+    "assemble_model",
     "basis_glow",
+    "EnergyPlusSetup",
+    "ep_datetime_parser",
+    "epjson2rad",
+    "GlazingSystem",
     "gen_perez_sky",
     "gen_grid",
-    "parse_primitive",
+    "genskymtx",
+    "KRYPTON",
+    "load_epmodel",
+    "load_matrix",
+    "multiply_rgb",
     "parse_epw",
+    "parse_mrad_config",
     "parse_wea",
     "parse_polygon",
     "Primitive",
-    "oconv",
     "points_as_sender",
     "rfluxmtx",
-    "rtrace",
     "sky_as_receiver",
     "surface_as_receiver",
     "sun_as_receiver",
     "surface_as_sender",
-    "render",
+    "three_phase",
     "unpack_primitives",
     "View",
     "view_as_sender",
     "WeaData",
     "WeaMetaData",
+    "XENON",
 ]
```

### Comparing `frads-0.2.8/frads/cli.py` & `frads-0.3.0/frads/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from frads import mtxmult
 from frads import ncp
 from frads import parsers
 from frads import room
 from frads import utils
 from frads.types import NcpModel
 from frads.types import PaneRGB
-from frads.types import Receiver
+from frads.matrix import Receiver
 
 
 logger: logging.Logger = logging.getLogger("frads")
 
 
 def mrad_init(args: argparse.Namespace) -> None:
     """Initiate mrad operation.
@@ -227,17 +227,18 @@
             try:
                 with open(item, "r", encoding="utf-8") as rdr:
                     json_obj = json.load(rdr)
             except FileNotFoundError as fnfe:
                 raise fnfe
             panes.append(parsers.parse_igsdb_json(json_obj))
     pane_rgb = []
-    coeffs = color.get_conversion_matrix(args.cspace)
+    coeffs = color_data.XYZ2RGB_RAD
+    # coeffs = color.get_conversion_matrix(args.cspace)
     for pane in panes:
-        wvls = sorted(set(color_data.CIE_XYZ_2).intersections(pane.wavelength))
+        wvls = sorted(set(color_data.CIE_XYZ_2).intersection(pane.wavelength))
         wvl_range = wvls[-1] - wvls[0]
         cie_xyz = color.get_interpolated_cie_xyz(wvls, args.observer)
         trans = [pane.transmittance[pane.wavelength.index(wvl)] for wvl in wvls]
         reflf = [pane.reflectance_front[pane.wavelength.index(wvl)] for wvl in wvls]
         reflb = [pane.reflectance_back[pane.wavelength.index(wvl)] for wvl in wvls]
         tf_x, tf_y, tf_z = color.spec2xyz(cie_xyz, trans, wvl_range)
         rf_x, rf_y, rf_z = color.spec2xyz(cie_xyz, reflf, wvl_range)
@@ -302,17 +303,17 @@
     del args.pts, args.basis, args.sys, args.verbose
     matrix.rfluxmtx(sender, receiver, sys_paths, utils.opt2list(vars(args)))
 
 
 def genmtx_vu_sky(args) -> None:
     """Generate a view to sky matrix."""
     with open(args.vu, "r", encoding="ascii") as rdr:
-        vudict = parsers.parse_vu(rdr.readlines()[-1])  # use the last view
+        view = parsers.parse_vu(rdr.readlines()[-1])  # use the last view
     sender = matrix.view_as_sender(
-        vu_dict=vudict,
+        view,
         ray_cnt=1,
         xres=args.resolu[0],
         yres=args.resolu[1],
     )
     out = Path(f"{args.vu.stem}_{args.basis}sky")
     out.mkdir()
     receiver = matrix.sky_as_receiver(args.basis, out / "%04d.hdr")
@@ -352,53 +353,54 @@
         ]
         if _receiver != []:
             outpath = Path(f"{args.pts.stem}_{args.srf.stem}.mtx")
             receiver += matrix.surface_as_receiver(
                 prim_list=_receiver,
                 basis=args.basis,
                 offset=args.offset,
-                left=None,
+                left=False,
                 source="glow",
                 out=outpath,
             )
     del args.pts, args.srf, args.sys, args.basis, args.offset, args.verbose
     matrix.rfluxmtx(sender, receiver, sys_paths, utils.opt2list(vars(args)))
 
 
 def genmtx_vu_srf(args) -> None:
     """Generate a view to surface matrix."""
     with open(args.vu, "r", encoding="ascii") as rdr:
-        sender = matrix.view_as_sender(
-            vu_dict=parsers.parse_vu(rdr.readlines()[-1]),
-            ray_cnt=1,
-            xres=args.resolu[0],
-            yres=args.resolu[1],
-        )
+        view = parsers.parse_vu(rdr.readlines()[-1])
+    sender = matrix.view_as_sender(
+        view,
+        ray_cnt=1,
+        xres=args.resolu[0],
+        yres=args.resolu[1],
+    )
     rprims = utils.unpack_primitives(args.srf)
     modifiers = {prim.modifier for prim in rprims if prim.ptype in ("polygon", "ring")}
     receiver = Receiver(receiver="", basis=args.basis, modifier="")
     sys_paths = args.sys
     for mod in modifiers:
         _receiver = [
             prim
             for prim in rprims
             if prim.modifier == mod and prim.ptype in ("polygon", "ring")
         ]
         if _receiver != []:
-            outpath = Path(f"{args.pts.name}_{args.srf.name}")
+            outpath = Path(f"{args.vu.stem}_{args.srf.stem}")
             outpath.mkdir()
             receiver += matrix.surface_as_receiver(
                 prim_list=_receiver,
                 basis=args.basis,
                 offset=args.offset,
-                left=None,
+                left=False,
                 source="glow",
                 out=outpath / "%04d.hdr",
             )
-    del args.pts, args.srf, args.sys, args.basis, args.offset, args.resolu, args.verbose
+    del args.vu, args.srf, args.sys, args.basis, args.offset, args.resolu, args.verbose
     matrix.rfluxmtx(sender, receiver, sys_paths, utils.opt2list(vars(args)))
 
 
 def genmtx_srf_srf(args) -> None:
     """Generate a surface to surface matrix."""
     sender = matrix.surface_as_sender(
         prim_list=utils.unpack_primitives(args.ssrf),
@@ -442,30 +444,31 @@
         window_normals=None,
         full_mod=full_modifier,
     )
     outpath = Path(f"{args.pts.stem}_sun.mtx")
     sun_oct = f"sun_{utils.id_generator()}"
     sys_paths = args.sys
     matrix.rcvr_oct(receiver, sys_paths, sun_oct)
-    del args.pts, args.basis, args.sys_paths, args.verbose
+    del args.pts, args.basis, args.sys, args.verbose
     matrix.rcontrib(
         sender=sender,
         modifier=receiver.modifier,
         octree=sun_oct,
         out=outpath,
         opt=utils.opt2list(vars(args)),
     )
     os.remove(sun_oct)
 
 
 def genmtx_vu_sun(args) -> None:
     """Generate a view to sun matrix."""
     with open(args.vu, "r", encoding="ascii") as rdr:
+        view = parsers.parse_vu(rdr.readlines()[-1])
         sender = matrix.view_as_sender(
-            vu_dict=parsers.parse_vu(rdr.readlines()[-1]),
+            view,
             ray_cnt=1,
             xres=args.resolu[0],
             yres=args.resolu[1],
         )
     wnormals = None
     if args.window is not None:
         wnormals = utils.primitive_normal(args.window)
```

### Comparing `frads-0.2.8/frads/color.py` & `frads-0.3.0/frads/color.py`

 * *Files identical despite different names*

### Comparing `frads-0.2.8/frads/color_data.py` & `frads-0.3.0/frads/color_data.py`

 * *Files identical despite different names*

### Comparing `frads-0.2.8/frads/data/WC.DAT` & `frads-0.3.0/frads/data/WC.DAT`

 * *Files identical despite different names*

### Comparing `frads-0.2.8/frads/epjson2rad.py` & `frads-0.3.0/frads/epjson2rad.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,48 @@
 """Convert an EnergyPlus epJSON file into Radiance model[s]."""
 
 from configparser import ConfigParser
-import json
 import logging
+import math
+import json
 import os
 from pathlib import Path
+import sys
 import subprocess as sp
-from typing import Any, Mapping, Dict
-from typing import List
+from typing import Dict, List
+
+import pyradiance as pr
+
+from frads import geom, utils
+from frads.types import (
+    EPlusWindowGas,
+    EPlusOpaqueMaterial,
+    EPlusWindowMaterial,
+    EPlusWindowMaterialComplexShade,
+    EPlusConstruction,
+    EPlusOpaqueSurface,
+    EPlusFenestration,
+    EPlusZone,
+    Primitive,
+)
 
-from frads import geom
-from frads import utils
-from frads.types import Primitive
-from frads.types import BSDFData
-from frads.types import RadMatrix
-from frads.types import EPlusWindowGas
-from frads.types import EPlusOpaqueMaterial
-from frads.types import EPlusWindowMaterial
-from frads.types import EPlusConstruction
-from frads.types import EPlusOpaqueSurface
-from frads.types import EPlusFenestration
-from frads.types import EPlusZone
 
 logger: logging.Logger = logging.getLogger("frads.epjson2rad")
 
 
+def tmit2tmis(tmit: float) -> float:
+    """Convert from transmittance to transmissivity."""
+    a = 0.0072522239
+    b = 0.8402528435
+    c = 0.9166530661
+    d = 0.0036261119
+    tmis = ((math.sqrt(a * tmit**2 + b) - c) / d) / tmit
+    return max(0, min(tmis, 1))
+
+
 def thicken(
     surface: geom.Polygon, windows: List[geom.Polygon], thickness: float
 ) -> list:
     """Thicken window-wall."""
     direction = surface.normal.scale(thickness)
     facade = surface.extrude(direction)[:2]
     for window in windows:
@@ -49,18 +63,17 @@
     for layer in construction.layers:
         layer_thickness.append(materials[layer.lower()].thickness)
     return sum(layer_thickness)
 
 
 def check_outward(polygon: geom.Polygon, zone_center: geom.Vector) -> bool:
     """Check whether a surface is facing outside."""
-    pi = 3.14159265358579
     outward = True
     angle2center = polygon.normal.angle_from(zone_center - polygon.centroid)
-    if angle2center < pi / 4:
+    if angle2center < math.pi / 4:
         outward = False
     return outward
 
 
 def eplus_surface2primitive(
     surfaces: dict, constructions, zone_center, materials
 ) -> dict:
@@ -190,14 +203,34 @@
         solar_absorptance,
         visible_absorptance,
         visible_reflectance,
         primitive,
     )
 
 
+def parse_windowmaterial_complexshade(
+    name: str, material: dict
+) -> EPlusWindowMaterialComplexShade:
+    """Parse EP WindowMaterial:ComplexShade."""
+    return EPlusWindowMaterialComplexShade(
+        name.replace(" ", "_"),
+        material.get("layer_type", ""),
+        material.get("thickness", 0.002),
+        material.get("conductivity", 1.0),
+        material.get("ir_transmittance", 0.0),
+        material.get("front_emissivity", 0.84),
+        material.get("back_emissivity", 0.84),
+        material.get("top_opening_multiplier", 0.0),
+        material.get("bottom_opening_multiplier", 0.0),
+        material.get("left_side_opening_multiplier", 0.0),
+        material.get("right_side_opening_multiplier", 0.0),
+        material.get("front_opening_multiplier", 0.0),
+    )
+
+
 def parse_windowmaterial_gap(name: str, material: dict) -> EPlusWindowGas:
     """Parse EP WindowMaterial:Gap"""
     name = name.replace(" ", "_")
     thickness = material["thickness"]
     gas = material["gas_or_gas_mixture_"]
     return EPlusWindowGas(name, thickness, gas, [1])
 
@@ -223,38 +256,38 @@
 def parse_windowmaterial_simpleglazingsystem(
     name: str, material: dict
 ) -> EPlusWindowMaterial:
     """Parse EP WindowMaterial:SimpleGlazingSystem"""
     identifier = name.replace(" ", "_")
     shgc = material["solar_heat_gain_coefficient"]
     tmit = material.get("visible_transmittance", shgc)
-    tmis = utils.tmit2tmis(tmit)
+    tmis = tmit2tmis(tmit)
     primitive = Primitive("void", "glass", identifier, ["0"], [3, tmis, tmis, tmis])
     return EPlusWindowMaterial(identifier, tmit, primitive)
 
 
 def parse_windowmaterial_simpleglazing(
     name: str, material: dict
 ) -> EPlusWindowMaterial:
     """Parse EP WindowMaterial:Simpleglazing"""
     identifier = name.replace(" ", "_")
     tmit = material["visible_transmittance"]
-    tmis = utils.tmit2tmis(tmit)
+    tmis = tmit2tmis(tmit)
     primitive = Primitive("void", "glass", identifier, ["0"], [3, tmis, tmis, tmis])
     return EPlusWindowMaterial(identifier, tmit, primitive)
 
 
 def parse_windowmaterial_glazing(name: str, material: dict) -> EPlusWindowMaterial:
     """Parse EP WindowMaterial:Glazing"""
     identifier = name.replace(" ", "_")
     if material["optical_data_type"].lower() == "bsdf":
         tmit = 1
     else:
         tmit = material["visible_transmittance_at_normal_incidence"]
-    tmis = utils.tmit2tmis(tmit)
+    tmis = tmit2tmis(tmit)
     primitive = Primitive("void", "glass", identifier, ["0"], [3, tmis, tmis, tmis])
     return EPlusWindowMaterial(identifier, tmit, primitive)
 
 
 def parse_windowmaterial_blind(inp: dict) -> dict:
     """Parse EP WindowMaterial:Blind"""
     blind_prims = {}
@@ -294,26 +327,32 @@
 def parse_construction_complexfenestrationstate(epjs):
     """Parser EP Construction:ComplexFenestrationState."""
     construction = epjs.get("Construction:ComplexFenestrationState", {})
     cfs = {}
     matrices = {}
     for key, val in construction.items():
         val["ctype"] = "cfs"
-        tf_name = val["visible_optical_complex_front_transmittance_matrix_name"]
-        tb_name = val["visible_optical_complex_back_transmittance_matrix_name"]
-        tf_list = epjs["Matrix:TwoDimension"][tf_name]["values"]
-        tb_list = epjs["Matrix:TwoDimension"][tb_name]["values"]
-        ncolumn = epjs["Matrix:TwoDimension"][tf_name]["number_of_columns"]
-        # if ncolumn < 145:
-        # raise ValueError("BSDF resolution too low to take advantage of Radiance")
-        tf_bsdf = [v["value"] for v in tf_list]
-        tb_bsdf = [v["value"] for v in tb_list]
-        tf = utils.bsdf2sdata(BSDFData(tf_bsdf, ncolumn, ncolumn))
-        tb = utils.bsdf2sdata(BSDFData(tb_bsdf, ncolumn, ncolumn))
-        matrices[key] = RadMatrix(tf, tb)
+        names = {
+            "tvf": val["visible_optical_complex_front_transmittance_matrix_name"],
+            "tvb": val["visible_optical_complex_back_transmittance_matrix_name"],
+            # "rvf": val["visible_optical_complex_front_reflectance_matrix_name"],
+            # "rvb": val["visible_optical_complex_back_reflectance_matrix_name"],
+            "tsf": val["solar_optical_complex_front_transmittance_matrix_name"],
+            # "tsb": val["solar_optical_complex_back_transmittance_matrix_name"],
+            # "rsf": val["solar_optical_complex_front_reflectance_matrix_name"],
+            "rsb": val["solar_optical_complex_back_reflectance_matrix_name"],
+        }
+        bsdf = {key: [v["value"] for v in epjs["Matrix:TwoDimension"][name]['values']]
+                for key, name in names.items()}
+        ncs = {key: epjs["Matrix:TwoDimension"][name]["number_of_columns"]
+                for key, name in names.items()}
+        nrs = {key: epjs["Matrix:TwoDimension"][name]["number_of_rows"]
+                for key, name in names.items()}
+        matrices[key] = {key: {"ncolumns": ncs[key], "nrows": nrs[key], "values": bsdf[key]} 
+                         for key in names}
         cfs[key] = EPlusConstruction(key, "cfs", [])
     return cfs, matrices
 
 
 def parse_construction(construction: dict) -> dict:
     """Parse EP Construction"""
     constructions = {}
@@ -374,15 +413,20 @@
     """
     Convert EnergyPlus JSON objects into Radiance primitives.
     """
     # get site information
     site = list(epjs["Site:Location"].values())[0]
 
     # parse each fenestration
-    fenestrations = parse_epjson_fenestration(epjs["FenestrationSurface:Detailed"])
+    fenes = epjs.get("FenestrationSurface:Detailed")
+    if fenes is not None:
+        fenestrations = parse_epjson_fenestration(fenes)
+    else:
+        logger.warning("No fenestration found in the model.")
+        sys.exit(1)
 
     # Get all the fenestration hosting surfaces
     fene_hosts = {val.host for val in fenestrations.values()}
 
     # parse each opaque surface
     opaque_surfaces = parse_opaque_surface(
         epjs["BuildingSurface:Detailed"], fenestrations
@@ -421,64 +465,68 @@
             n: val
             for n, val in fenestrations.items()
             if opaque_surfaces[val.host].zone == zname
         }
         for name, surface in opaque_surfaces.items():
             if surface.zone == zname:
                 surface_map[surface.type][name] = surface
-        zones[zname] = EPlusZone(zone_name, *surface_map.values(), windows)
+        zones[zname] = EPlusZone(
+            zone_name,
+            surface_map["Wall"],
+            surface_map["Ceiling"],
+            surface_map["Roof"],
+            surface_map["Floor"],
+            windows,
+        )
     return site, zones, constructions, materials, matrices
 
 
-def write_config(config: Mapping[str, Mapping[str, Any]]) -> None:
-    """Write config."""
-    cfg = ConfigParser(allow_no_value=True)
-    # templ_config = config.to_dict()
-    cfg.read_dict(config)
-    with open(f"{config.name}.cfg", "w", encoding="utf-8") as rdr:
-        cfg.write(rdr)
-
-
-def epjson2rad(epjs: dict) -> None:
+def epjson2rad(epjs: dict, epw=None) -> None:
     """Command-line program to convert a energyplus model into a Radiance model."""
     # Setup file structure
-    Path("Objects").mkdir(exist_ok=True)
-    Path("Resources").mkdir(exist_ok=True)
-    Path("Matrices").mkdir(exist_ok=True)
+    objdir = Path("Objects")
+    objdir.mkdir(exist_ok=True)
+    mtxdir = Path("Matrices")
+    mtxdir.mkdir(exist_ok=True)
 
     site, zones, constructions, materials, matrices = parse_epjson(epjs)
-    building_name = epjs["Building"].popitem()[0].replace(" ", "_")
+    # building_name = epjs["Building"].popitem()[0].replace(" ", "_")
+    building_name = list(epjs["Building"].keys())[0].replace(" ", "_")
+
+    if len(matrices) > 0:
+        rsodir = Path("Resources")
+        rsodir.mkdir(exist_ok=True)
+        # Write matrix files to xml, if any
+        xml_paths = {}
+        for key, val in matrices.items():
+            opath = rsodir / (key + ".xml")
+            _vis = pr.WrapBSDFInput("Visible")
+            _sol = pr.WrapBSDFInput("Solar")
+            for _key, _val in val.items():
+                _mtxpath = rsodir / f"{key}_{key}.mtx"
+                with open(_mtxpath, "w") as fp:
+                    fp.write(" ".join(str(v) for v in _val["values"]))
+                if _key[1] == "v":
+                    _vis.__setattr__(_key[0]+_key[-1], _mtxpath)
+                elif _key[1] == "s":
+                    _sol.__setattr__(_key[0]+_key[-1], _mtxpath)
+            basis = [i.name for i in pr.ABASELIST if i.nangles == val['tvf']['ncolumns']].pop()
+            abr_basis = "".join(i[0].lower() for i in basis.decode().lstrip("LBNL/").split())
+            with open(opath, "wb") as wtr:
+                wtr.write(
+                    pr.wrapbsdf(basis=abr_basis, inp=[_vis, _sol], unlink=True, n=key)
+                )
+            xml_paths[key] = str(opath)
 
     # Write material file
     material_path = os.path.join("Objects", f"materials{building_name}.mat")
     with open(material_path, "w", encoding="ascii") as wtr:
         for material in materials.values():
             wtr.write(str(material.primitive))
 
-    # Write matrix files to xml, if any
-    xml_paths = {}
-    for key, val in matrices.items():
-        opath = os.path.join("Resources", key + ".xml")
-        tf_path = os.path.join("Resources", key + "_tf.mtx")
-        tb_path = os.path.join("Resources", key + "_tb.mtx")
-        with open(tf_path, "w", encoding="ascii") as wtr:
-            wtr.write(repr(val.tf))
-        with open(tb_path, "w", encoding="ascii") as wtr:
-            wtr.write(repr(val.tb))
-        # basis = ''.join([word[0] for word in val.tf.basis.split()])
-        basis = "".join(
-            [word[0].lower() for word in utils.BASIS_DICT[str(val.tf.ncolumn)].split()]
-        )
-        cmd = ["wrapBSDF", "-f", "n=" + key, "-a", basis]
-        cmd += ["-tf", tf_path, "-tb", tb_path, "-U"]
-        wb_process = sp.run(cmd, check=True, stdout=sp.PIPE, stderr=sp.PIPE)
-        with open(opath, "wb") as wtr:
-            wtr.write(wb_process.stdout)
-        xml_paths[key] = opath
-
     # For each zone write primitves to files and create a config file
     for name, zone in zones.items():
         mrad_config = ConfigParser(allow_no_value=False)
         mrad_config["SimControl"] = {
             "vmx_basis": "kf",
             "vmx_opt": "-ab 5 -ad 65536 -lw 1e-5",
             "fmx_basis": "kf",
@@ -490,22 +538,21 @@
             "ray_count": "1",
             "nprocess": "1",
             "separate_direct": "False",
             "overwrite": "False",
             "method": "",
         }
         mrad_config["Site"] = {
-            "wea_path": "",
-            "zipcode": "",
+            "epw_path": epw,
             "latitude": site["latitude"],
             "longitude": site["longitude"],
-            "start_hour": "",
-            "end_hour": "",
             "daylight_hours_only": "True",
         }
+        if epw is not None:
+            mrad_config["Site"]["epw_path"] = epw
         primitives = epluszone2rad(zone, constructions, materials)
         scene = []
         windows = []
         window_xmls = []
         floors = []
         for primitive in primitives:
             write_primitives(primitive, "Objects")
@@ -521,24 +568,24 @@
         # Get floors
         for primitive in primitives[-1]:
             floors.append(os.path.join("Objects", primitive + ".rad"))
 
         mrad_config["Model"] = {
             "material": material_path,
             "scene": "\n".join(scene),
-            "window_paths": " ".join(windows),
+            "windows": " ".join(windows),
             "window_xml": " ".join(window_xmls),
             "ncp_shade": "",
         }
         mrad_config["RaySender"] = {
             "grid_surface": " ".join(floors),
             "grid_spacing": "1",
             "grid_height": "0.75",
         }
-        with open(f"{name.replace(' ', '_')}.cfg", "w", encoding="utf-8") as wtr:
+        with open(f"{name}.cfg", "w", encoding="utf-8") as wtr:
             mrad_config.write(wtr)
 
 
 def read_ep_input(fpath: Path) -> dict:
     """Load and parse input file into a JSON object.
     If the input file is in .idf fomart, use command-line
     energyplus program to convert it to epJSON format
@@ -552,10 +599,12 @@
         cmd = ["energyplus", "--convert-only", str(fpath)]
         sp.run(cmd, check=True)
         epjson_path = Path(fpath.with_suffix(".epJSON").name)
         if not epjson_path.is_file():
             raise FileNotFoundError(f"Converted {str(epjson_path)} not found.")
     elif fpath.suffix == ".epJSON":
         epjson_path = fpath
+    else:
+        raise Exception(f"Unknown file type {fpath}")
     with open(epjson_path) as rdr:
         epjs = json.load(rdr)
     return epjs
```

### Comparing `frads-0.2.8/frads/geom.py` & `frads-0.3.0/frads/geom.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 and other geometry related routines.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 import math
-from typing import Union
-from typing import List
-from typing import Tuple
-from typing import Sequence
+from typing import Union, List, Tuple, Sequence
 
 
 @dataclass(frozen=True)
 class Vector:
     """3D vector class.
 
     Attributes:
@@ -179,15 +176,15 @@
 class Polygon:
     """3D polygon class
 
     Attributes:
         vertices(List[Vector]): list of vertices of the polygon.
     """
 
-    vertices: Tuple[Vector]
+    vertices: List[Vector]
 
     def __post_init__(self) -> None:
         """."""
         if len(self.vertices) < 3:
             raise ValueError("Need more than 2 vertices to make a polygon.")
 
     def __eq__(self, other: object) -> bool:
@@ -233,15 +230,15 @@
             results.extend(new_other_vert)
             results.append(other.vertices[idx_min])
         else:
             results.append(new_other_vert[0])
             results.extend(reversed(new_other_vert[1:]))
             results.append(new_other_vert[0])
         results.extend(self.vertices)
-        return Polygon(tuple(results))
+        return Polygon(results)
 
     @property
     def normal(self) -> Vector:
         """Calculate the polygon normal."""
         normal = Vector(0, 0, 0)
         for idx in range(len(self.vertices) - 2):
             normal += (self.vertices[idx + 1] - self.vertices[idx]).cross(
@@ -289,15 +286,15 @@
         """
         new_vertices = []
         for vert in self.vertices:
             sx = center.x + (vert.x - center.x) * scale_vect.x
             sy = center.y + (vert.y - center.y) * scale_vect.y
             sz = center.z + (vert.z - center.z) * scale_vect.z
             new_vertices.append(Vector(sx, sy, sz))
-        return Polygon(tuple(new_vertices))
+        return Polygon(new_vertices)
 
     def extrude(self, vector: Vector) -> list:
         """Extrude the polygon.
 
         Args:
             vector (Vector): extrude along the vector;
 
@@ -307,30 +304,30 @@
         """
         polygons = [self]
         polygon2 = Polygon(([i + vector for i in self.vertices]))
         polygons.append(polygon2)
         for i in range(len(self.vertices) - 1):
             polygons.append(
                 Polygon(
-                    (
+                    [
                         self.vertices[i],
                         polygon2.vertices[i],
                         polygon2.vertices[i + 1],
                         self.vertices[i + 1],
-                    )
+                    ]
                 )
             )
         polygons.append(
             Polygon(
-                (
+                [
                     self.vertices[-1],
                     polygon2.vertices[-1],
                     polygon2.vertices[0],
                     self.vertices[0],
-                )
+                ]
             )
         )
         return polygons
 
     def shared_pts(self, other) -> Tuple[int, List[int]]:
         """Return the total number of share points between two polygons."""
         cnt = 0
@@ -353,15 +350,15 @@
 
     def to_list(self):
         """Return a list of tuples."""
         return [p.to_tuple() for p in self.vertices]
 
     def to_real(self) -> Union[List[float], List[int]]:
         """Convert the vertices to real arg string format."""
-        real_arg = [3 * len(self.vertices)]
+        real_arg = []
         for vert in self.vertices:
             real_arg.append(vert.x)
             real_arg.append(vert.y)
             real_arg.append(vert.z)
         return real_arg
 
     @classmethod
```

### Comparing `frads-0.2.8/frads/matrix.py` & `frads-0.3.0/frads/matrix.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,88 @@
 """
 This module contains routines to generate sender and receiver objects, generate
 matrices by calling either rfluxmtx or rcontrib.
 """
 
 from __future__ import annotations
+from dataclasses import dataclass
 import logging
 import os
 from pathlib import Path
 import subprocess as sp
 import tempfile as tf
-from typing import Iterable
-from typing import List
-from typing import Optional
-from typing import Sequence
-from typing import Union
-
-from frads import sky
-from frads import geom
-from frads import parsers
-from frads import raycall
-from frads import utils
-from frads.types import Primitive
-from frads.types import Receiver
-from frads.types import Sender
-from frads.geom import Vector
+from typing import List, Optional, Union, Sequence
+
+from frads import geom, parsers, sky, utils
+import numpy as np
+import pyradiance as pr
 
 
 logger: logging.Logger = logging.getLogger("frads.matrix")
 
 
+@dataclass(frozen=True)
+class Sender:
+    """Sender object for matrix generation.
+
+    Attributes:
+        form: types of sender, {surface(s)|view(v)|points(p)}
+        sender: the sender string
+        xres: sender x dimension
+        yres: sender y dimension
+    """
+
+    form: str
+    sender: bytes
+    xres: Optional[int]
+    yres: Optional[int]
+
+
+@dataclass
+class Receiver:
+    """Receiver object for matrix generation.
+
+    Attributes:
+        receiver: receiver string which can be appended to one another
+        basis: receiver basis, usually kf, r4, r6;
+        modifier: modifiers to the receiver objects;
+    """
+
+    receiver: str
+    basis: str
+    modifier: str = ""
+
+    def __add__(self, other) -> "Receiver":
+        return Receiver(
+            self.receiver + "\n" + other.receiver, self.basis, self.modifier
+        )
+
+
 def surface_as_sender(prim_list: list, basis: str, offset=None, left=None) -> Sender:
     """
     Construct a sender from a surface.
 
     Args:
-        prim_list(list): a list of primitives
-        basis(str): sender sampling basis
-        offset(float): move the sender surface in its normal direction
-        left(bool): Use left-hand rule instead for matrix generation
+        prim_list: a list of primitives
+        basis: sender sampling basis
+        offset: move the sender surface in its normal direction
+        left: Use left-hand rule instead for matrix generation
 
     Returns:
         A sender object (Sender)
 
     """
     prim_str = prepare_surface(
         prims=prim_list, basis=basis, offset=offset, left=left, source=None, out=None
     )
     logger.debug("Surface sender:\n%s", prim_str)
     return Sender("s", prim_str.encode(), None, None)
 
 
-def view_as_sender(view: View, ray_cnt: int, xres: int, yres: int) -> Sender:
+def view_as_sender(view, ray_cnt: int, xres: int, yres: int) -> Sender:
     """
     Construct a sender from a view.
 
     Args:
         view: a view object;
         ray_cnt: ray count;
         xres, yres: image resolution
@@ -62,49 +90,107 @@
 
     Returns:
         A sender object
 
     """
     if (xres is None) or (yres is None):
         raise ValueError("Need to specify resolution")
-    res_cmd = [
-        "vwrays",
-        *view.args(),
-        "-x",
-        str(xres),
-        "-y",
-        str(yres),
-        "-d",
-    ]
-    logger.info("Check real image resolution: \n%s", " ".join(res_cmd))
-    res_proc = sp.run(res_cmd, check=True, stdout=sp.PIPE, encoding="ascii")
-    res_eval = res_proc.stdout.split()
+    res_eval = pr.vwrays(
+        view=view.args(), xres=xres, yres=yres, dimensions=True
+    ).split()
     new_xres, new_yres = int(res_eval[1]), int(res_eval[3])
     if (new_xres != xres) and (new_yres != yres):
         logger.info("Changed resolution to %s %s", new_xres, new_yres)
-    vwrays_cmd = ["vwrays", "-ff", "-x", str(new_xres), "-y", str(new_yres)]
+    # vwrays_cmd = ["vwrays", "-ff", "-x", str(new_xres), "-y", str(new_yres)]
+    vwrays_cmd = ["vwrays", "-ff"]
     if ray_cnt > 1:
         vwrays_cmd.extend(["-c", str(ray_cnt), "-pj", "0.7"])
     logger.debug("Ray count is %s", ray_cnt)
     vwrays_cmd += view.args()
+    vwrays_cmd += ["-x", str(new_xres), "-y", str(new_yres)]
     logger.info("Generate view rays with: \n%s", " ".join(vwrays_cmd))
     vwrays_proc = sp.run(vwrays_cmd, check=True, stdout=sp.PIPE)
+    vwrays_proc = pr.vwrays(
+        view=view.args(),
+        outform="f",
+        xres=new_xres,
+        yres=new_yres,
+        ray_count=ray_cnt,
+        pixel_jitter=0.7,
+    )
     if view.vtype == "a":
-        flush_cmd = utils.get_flush_corner_rays_command(ray_cnt, xres)
+        flush_cmd = [
+            "rcalc",
+            "-if6",
+            "-of",
+            "-e",
+            f"DIM:{xres};CNT:{ray_cnt}",
+            "-e",
+            "pn=(recno-1)/CNT+.5",
+            "-e",
+            "frac(x):x-floor(x)",
+            "-e",
+            "xpos=frac(pn/DIM);ypos=pn/(DIM*DIM)",
+            "-e",
+            "incir=if(.25-(xpos-.5)*(xpos-.5)-(ypos-.5)*(ypos-.5),1,0)",
+            "-e",
+            "$1=$1;$2=$2;$3=$3;$4=$4*incir;$5=$5*incir;$6=$6*incir",
+        ]
         logger.info("Flushing -vta corner rays: \n%s", " ".join(flush_cmd))
-        flush_proc = sp.run(
-            flush_cmd, check=True, input=vwrays_proc.stdout, stdout=sp.PIPE
-        )
+        flush_proc = sp.run(flush_cmd, check=True, input=vwrays_proc, stdout=sp.PIPE)
         vrays = flush_proc.stdout
     else:
-        vrays = vwrays_proc.stdout
+        vrays = vwrays_proc
     logger.debug("View sender:\n%s", vrays)
     return Sender("v", vrays, xres, yres)
 
 
+def load_matrix(file: Union[bytes, str, Path], dtype: str = "float"):
+    """
+    Load a Radiance matrix file into numpy array.
+
+    Args:
+        file: a file path
+
+    Returns:
+        A numpy array
+    """
+    npdtype = np.double if dtype.startswith("d") else np.single
+    mtx = pr.rmtxop(file, outform=dtype[0].lower())
+    nrows, ncols, ncomp, _ = parsers.parse_rad_header(pr.getinfo(mtx).decode())
+    return np.frombuffer(pr.getinfo(mtx, strip_header=True), dtype=npdtype).reshape(
+        nrows, ncols, ncomp
+    )
+
+
+def load_image_matrix(file, outform="d") -> np.ndarray:
+    """
+    Load a Radiance HDR image into numpy array.
+    Args:
+        file: a file path
+    Returns:
+        A numpy array
+    """
+    xres, yres = pr.get_image_dimensions(file)
+    pix = pr.pvalue(file, outform=outform)
+    return np.frombuffer(pix, np.double).reshape(xres, yres, 3)
+
+
+def multiply_rgb(*mtx: np.ndarray, weights=None):
+    """Multiply matrices as numpy ndarray."""
+    resr = np.linalg.multi_dot([m[:, :, 0] for m in mtx])
+    resg = np.linalg.multi_dot([m[:, :, 1] for m in mtx])
+    resb = np.linalg.multi_dot([m[:, :, 2] for m in mtx])
+    if weights:
+        if len(weights) != 3:
+            raise ValueError("Weights should have 3 values")
+        return resr * weights[0] + resg * weights[1] + resb * weights[2]
+    return np.array((resr, resg, resb))
+
+
 def points_as_sender(pts_list: list, ray_cnt: Optional[int] = None) -> Sender:
     """
     Construct a sender from a list of points.
 
     Args:
         pts_list(list): a list of list of float
         ray_cnt(int): sender ray count
@@ -122,15 +208,15 @@
     logger.debug("Point sender:\n%s", grid_str)
     return Sender("p", grid_str.encode(), None, len(pts_list))
 
 
 def sun_as_receiver(
     basis,
     smx_path: Path,
-    window_normals: Optional[List[Vector]],
+    window_normals: Optional[List[geom.Vector]],
     full_mod: bool = False,
 ) -> Receiver:
     """
     Instantiate a sun receiver object.
 
     Args:
         basis: receiver sampling basis {kf | r1 | sc25...}
@@ -170,15 +256,15 @@
     sky_str = f'#@rfluxmtx o="{str(out)}"\n'
     sky_str += sky.basis_glow(basis)
     logger.debug("Sky receiver:\n%s", sky_str)
     return Receiver(sky_str, basis)
 
 
 def surface_as_receiver(
-    prim_list: Sequence[Primitive],
+    prim_list: List[pr.Primitive],
     basis: str,
     out: Union[None, str, Path],
     offset=None,
     left: bool = False,
     source: str = "glow",
 ) -> Receiver:
     """
@@ -227,45 +313,45 @@
     if len(modifier_set) != 1:
         logger.warning("Primitives don't share modifier")
     src_mod = f"rflx{prims[0].modifier}{utils.id_generator()}"
     header = f"#@rfluxmtx h={basis} u={upvector_str}\n"
     if out is not None:
         header += f'#@rfluxmtx o="{out}"\n\n'
     if source == "glow":
-        source_prim = Primitive("void", source, src_mod, ("0"), (4, 1, 1, 1, 0))
+        source_prim = pr.Primitive("void", source, src_mod, ("0"), (1, 1, 1, 0))
         header += str(source_prim)
     elif source == "light":
-        source_prim = Primitive("void", source, src_mod, ("0"), (3, 1, 1, 1))
+        source_prim = pr.Primitive("void", source, src_mod, ("0"), (1, 1, 1))
         header += str(source_prim)
     modifiers = [p.modifier for p in prims]
     content = ""
     for prim in prims:
         if prim.identifier in modifiers:
             _identifier = "discarded"
         else:
             _identifier = prim.identifier
         _modifier = src_mod
         if offset is not None:
-            poly = parsers.parse_polygon(prim.real_arg)
+            poly = parsers.parse_polygon(prim.fargs)
             offset_vec = poly.normal.scale(offset)
             moved_pts = [pt + offset_vec for pt in poly.vertices]
             _real_args = geom.Polygon(moved_pts).to_real()
         else:
-            _real_args = prim.real_arg
-        new_prim = Primitive(
-            _modifier, prim.ptype, _identifier, prim.str_arg, _real_args
+            _real_args = prim.fargs
+        new_prim = pr.Primitive(
+            _modifier, prim.ptype, _identifier, prim.sargs, _real_args
         )
         content += str(new_prim) + "\n"
     return header + content
 
 
 def rfluxmtx(
     sender: Sender,
     receiver: Receiver,
-    env: Iterable[Path],
+    env: Sequence[Path],
     opt: Optional[List[str]] = None,
 ) -> None:
     """
     Calling rfluxmtx to generate the matrices.
 
     Args:
         sender: Sender object
@@ -276,37 +362,32 @@
 
     Returns:
         return the stdout of the rfluxmtx run.
     """
     if None in (sender, receiver):
         raise ValueError("Sender/Receiver object is None")
     opt = [] if opt is None else opt
-    _sender = None
-    stdin: Optional[bytes] = sender.sender
+    rays = None
+    surface = None
     with tf.TemporaryDirectory() as tempd:
         receiver_path = Path(tempd, "receiver")
         with open(receiver_path, "w", encoding="ascii") as wtr:
             wtr.write(receiver.receiver)
         if sender.form == "s":
             sender_path = Path(tempd, "sender")
             with open(sender_path, "wb") as wtr:
                 wtr.write(sender.sender)
-            _sender = sender_path
-            stdin = None
+            surface = sender_path
         elif sender.form == "p":
             opt.extend(["-I+", "-faa", "-y", str(sender.yres)])
+            rays = sender.sender
         elif sender.form == "v":
             opt.extend(["-ffc", "-x", str(sender.xres), "-y", str(sender.yres), "-ld-"])
-        cmd = raycall.get_rfluxmtx_command(
-            receiver_path, option=opt, sender=_sender, sys_paths=env
-        )
-        logger.info("Running rfluxmtx with:\n%s", " ".join(cmd))
-        proc = sp.run(cmd, check=True, input=stdin, stderr=sp.PIPE)
-        if proc.stderr != b"":
-            logger.warning(proc.stderr.decode())
+            rays = sender.sender
+        pr.rfluxmtx(receiver_path, surface=surface, rays=rays, params=opt, scene=env)
 
 
 def rcvr_oct(receiver, env, oct_path: Union[str, Path]) -> None:
     """
     Generate an octree of the environment and the receiver.
 
     Args:
@@ -345,23 +426,42 @@
         out: output path
 
     Returns:
         None
 
     """
     opt.append("-fo+")
+    xres = None
+    yres = None
+    inform = None
+    outform = None
     with tf.TemporaryDirectory() as tempd:
         modifier_path = os.path.join(tempd, "modifier")
         with open(modifier_path, "w", encoding="utf-8") as wtr:
             wtr.write(modifier)
-        cmd = ["rcontrib", *opt]
-        stdin = sender.sender
         if sender.form == "p":
-            cmd += ["-I+", "-faf", "-y", str(sender.yres)]
+            opt += ["-I+"]
+            inform = "a"
+            outform = "f"
+            yres = sender.yres
         elif sender.form == "v":
             out = Path(out)
             out.mkdir(exist_ok=True)
             out = out / "%04d.hdr"
-            cmd += ["-ffc", "-x", str(sender.xres), "-y", str(sender.yres)]
-        cmd += ["-o", str(out), "-M", modifier_path, str(octree)]
-        logger.info("Running rcontrib with:\n%s", " ".join(cmd))
-        sp.run(cmd, check=True, input=stdin)
+            inform = "f"
+            outform = "c"
+            xres = sender.xres
+            yres = sender.yres
+            # cmd += ["-ffc", "-x", str(sender.xres), "-y", str(sender.yres)]
+        mod = pr.RcModifier()
+        mod.modifier_path = modifier_path
+        mod.xres = xres
+        mod.yres = yres
+        mod.output = str(out)
+        pr.rcontrib(
+            sender.sender,
+            str(octree),
+            [mod],
+            inform=inform,
+            outform=outform,
+            params=opt,
+        )
```

### Comparing `frads-0.2.8/frads/methods.py` & `frads-0.3.0/frads/methods.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,135 +1,125 @@
 """Typical Radiance matrix-based simulation workflows
 """
 
 from configparser import ConfigParser
 from contextlib import contextmanager
 import logging
+import math
 import os
 from pathlib import Path
 import shutil
 import subprocess as sp
 import tempfile as tf
-from typing import List
-from typing import Dict
-from typing import Generator
-from typing import Sequence
-from typing import Tuple
-
-from frads import geom
-from frads import sky
-from frads import matrix
-
-from frads import mtxmult
-from frads import parsers
-from frads import raycall
-from frads import utils
-from frads.types import Options
-from frads.types import Primitive
-from frads.types import Receiver
-from frads.types import Sender
-from frads.types import MradModel
-from frads.types import MradPath
-from frads.types import WeaMetaData
-from frads.types import WeaData
+from typing import Dict, List, Generator, Sequence, Tuple
+
+from frads import geom, sky, matrix
+from frads import mtxmult, parsers, utils
+from frads.matrix import Sender, Receiver
+from frads.types import MradModel, MradPath, View
+from frads.sky import WeaMetaData, WeaData
+
+import pyradiance as pr
 
 
 logger: logging.Logger = logging.getLogger("frads.methods")
 
 
-def get_window_group(wpaths: List[Path], orientation=None) -> Tuple[dict, list]:
+def get_window_group(wpaths: List[Path]) -> Tuple[dict, list]:
     """Parse window groups from config.
 
     Args:
         wpaths(str): window file paths
     Return:
         window_groups(dict): window group name and primitives
         window_normals(list): a list of normal for each window group.
     """
     window_groups = {}
     window_normals: List[geom.Vector] = []
     for wpath in wpaths:
         prims = utils.unpack_primitives(wpath)
         window_groups[wpath.stem] = prims
         # Taking normal from the first polygon
-        _normal = parsers.parse_polygon(prims[0].real_arg).normal
+        _normal = parsers.parse_polygon(prims[0].fargs).normal
         if _normal not in window_normals:
             window_normals.append(_normal)
-    final_window_normals = window_normals
-    if (orientation is not None) and (float(orientation) != 0):
-        rorient = float(orientation) * 180 / 3.14159265358579
-        final_window_normals = [n.rotate_3d(geom.Vector(0, 0, 1), rorient)
-                                for n in window_normals]
-    return window_groups, final_window_normals
+    return window_groups, window_normals
 
 
 def get_ncp_shades(npaths: List[Path]) -> dict:
     """Parse ncp shade groups from config."""
     ncp_shades = {}
     for npath in npaths:
         prims = utils.unpack_primitives(npath)
         ncp_shades[npath.stem] = prims
     return ncp_shades
 
 
 def get_wea_data(config: ConfigParser) -> Tuple[WeaMetaData, List[WeaData], str]:
     """Get wea data and parse into appropriate data types."""
+
     if wea_path := config["Site"].getpath("wea_path"):
         logger.info("Using user specified %s file.", wea_path)
         name = wea_path.stem
         with open(wea_path, "r", encoding="utf-8") as rdr:
             wea_metadata, wea_data = parsers.parse_wea(rdr.read())
+
     elif epw_path := config["Site"].getpath("epw_path"):
         logger.info("Converting %s to a .wea file", epw_path)
         name = epw_path.stem
         with open(epw_path, "r", encoding="utf-8") as rdr:
             wea_metadata, wea_data = parsers.parse_epw(rdr.read())
     else:
         raise ValueError("Need either a .wea or a .epw file")
     return wea_metadata, wea_data, name
 
 
 def get_sender_grid(config: ConfigParser) -> Dict[str, Sender]:
     """Get point grid as ray senders."""
     sender_grid: Dict[str, Sender] = {}
-    if (grid_paths := config["RaySender"].getpaths("grid_surface")) is None:
-        return sender_grid
-    for gpath in grid_paths:
-        name: str = gpath.stem
-        # Take the first polygon primitive
-        gprimitives = utils.unpack_primitives(gpath)
-        surface_polygon = None
-        for prim in gprimitives:
-            if prim.ptype == "polygon":
-                surface_polygon = parsers.parse_polygon(prim.real_arg)
-        if surface_polygon is None:
-            raise ValueError(f"No polygon found in {gpath}")
-        sensor_pts = utils.gen_grid(
-            surface_polygon,
-            config["RaySender"].getfloat("grid_height"),
-            config["RaySender"].getfloat("grid_spacing"),
-        )
-        sender_grid[name] = matrix.points_as_sender(
-            pts_list=sensor_pts, ray_cnt=config["SimControl"].getint("ray_count")
-        )
+    if (grid_files := config["RaySender"].getpaths("grid_points")) is not None:
+        for gfile in grid_files:
+            name = gfile.stem
+            with open(gfile) as f:
+                sensor_pts = [[float(v) for v in l.split()] for l in f.readlines()]
+            sender_grid[name] = matrix.points_as_sender(
+                pts_list=sensor_pts, ray_cnt=config["SimControl"].getint("ray_count")
+            )
+    elif (grid_paths := config["RaySender"].getpaths("grid_surface")) is not None:
+        for gpath in grid_paths:
+            name: str = gpath.stem
+            # Take the first polygon primitive
+            gprimitives = utils.unpack_primitives(gpath)
+            surface_polygon = None
+            for prim in gprimitives:
+                if prim.ptype == "polygon":
+                    surface_polygon = parsers.parse_polygon(prim.fargs)
+                    break
+            if surface_polygon is None:
+                raise ValueError(f"No polygon found in {gpath}")
+            sensor_pts = utils.gen_grid(
+                surface_polygon,
+                config["RaySender"].getfloat("grid_height"),
+                config["RaySender"].getfloat("grid_spacing"),
+            )
+            sender_grid[name] = matrix.points_as_sender(
+                pts_list=sensor_pts, ray_cnt=config["SimControl"].getint("ray_count")
+            )
     return sender_grid
 
 
 def get_sender_view(config: ConfigParser) -> Tuple[dict, dict]:
     """Get a single view as a sender.
     Args:
         config: MradConfig object"""
     sender_view: Dict[str, matrix.Sender] = {}
     view_dicts: Dict[str, View] = {}
     if (view := config["RaySender"].getview("view")) is None:
         return sender_view, view_dicts
     view_name = "view_00"
-    # if "vf" in vdict:
-    # with open(vdict["vf"], "r", encoding="ascii") as rdr:
-    # vdict.update(parsers.parse_vu(rdr.read()))
     view_dicts[view_name] = view
     sender_view[view_name] = matrix.view_as_sender(
         view=view,
         ray_cnt=int(config["SimControl"]["ray_count"]),
         xres=view.xres,
         yres=view.yres,
     )
@@ -147,28 +137,26 @@
         raise ValueError("Need to at least specify a grid or a view")
     # Get materials
     material_primitives = []
     for path in config["Model"].getpaths("material"):
         for prim in utils.unpack_primitives(path):
             material_primitives.append(prim)
     material_primitives.append(
-        Primitive("void", "plastic", "black", ["0"], [5, 0, 0, 0, 0, 0])
+        pr.Primitive("void", "plastic", "black", ["0"], [0, 0, 0, 0, 0])
     )
     material_primitives.append(
-        Primitive("void", "glow", "glowing", ["0"], [4, 1, 1, 1, 0])
+        pr.Primitive("void", "glow", "glowing", ["0"], [1, 1, 1, 0])
     )
     material_path = Path(f"all_material_{utils.id_generator()}.rad")
     with open(material_path, "w", encoding="ascii") as wtr:
         for primitive in material_primitives:
             wtr.write(str(primitive) + "\n")
-    # Orientation
-    orientation = config["Site"].get("orientation")
     # Get window groups
     window_groups, window_normals = get_window_group(
-        config["Model"].getpaths("windows", []), orientation=orientation
+        config["Model"].getpaths("windows", []),
     )
     # Get BSDFs
     bsdf_mat = {
         wname: Path(path)
         for wname, path in zip(
             window_groups, config["Model"].getpaths("window_xmls", [])
         )
@@ -271,15 +259,15 @@
             else:
                 mpath.pvmx[_name] = Path("Matrices", f"pvmx_{model.name}_{_name}.mtx")
                 out = mpath.pvmx[_name]
             receiver_windows += matrix.surface_as_receiver(
                 prim_list=window_prim,
                 basis=config["SimControl"]["vmx_basis"],
                 offset=None,
-                left=None,
+                left=False,
                 source="glow",
                 out=out,
             )
         if direct:
             files_exist = all(f.is_file() for f in mpath.pvmxd.values())
         else:
             files_exist = all(f.is_file() for f in mpath.pvmx.values())
@@ -374,52 +362,70 @@
     bwindow_path = f"blackened_window_{utils.id_generator()}.rad"
     gwindow_path = f"glowing_window_{utils.id_generator()}.rad"
     blackened_window = []
     glowing_window = []
     for _, windows in model.window_groups.items():
         for window in windows:
             blackened_window.append(
-                Primitive(
+                pr.Primitive(
                     "black",
                     window.ptype,
                     window.identifier,
-                    window.str_arg,
-                    window.real_arg,
+                    window.sargs,
+                    window.fargs,
                 )
             )
             glowing_window.append(
-                Primitive(
+                pr.Primitive(
                     "glowing",
                     window.ptype,
                     window.identifier,
-                    window.str_arg,
-                    window.real_arg,
+                    window.sargs,
+                    window.fargs,
                 )
             )
     with open(bwindow_path, "w", encoding="ascii") as wtr:
         wtr.write("\n".join(list(map(str, blackened_window))))
     with open(gwindow_path, "w", encoding="ascii") as wtr:
         wtr.write("\n".join(list(map(str, glowing_window))))
     vmap_oct = f"vmap_{utils.id_generator()}.oct"
     cdmap_oct = f"cdmap_{utils.id_generator()}.oct"
-    raycall.oconv(
-        str(model.material_path),
-        *map(str, config["Model"].getpaths("scene")),
-        gwindow_path,
-        outpath=vmap_oct,
-        frozen=True,
-    )
+    # raycall.oconv(
+    #     str(model.material_path),
+    #     *map(str, config["Model"].getpaths("scene")),
+    #     gwindow_path,
+    #     outpath=vmap_oct,
+    #     frozen=True,
+    # )
+    with open(vmap_oct, "wb") as wtr:
+        wtr.write(
+            pr.oconv(
+                str(model.material_path),
+                *[str(s) for s in config["Model"].getpaths("scene")],
+                gwindow_path,
+                frozen=True,
+            )
+        )
     logger.info("Generating view matrix material map octree")
-    raycall.oconv(
-        str(model.material_path),
-        *map(str, config["Model"]["scene"].split()),
-        bwindow_path,
-        outpath=cdmap_oct,
-        frozen=True,
-    )
+    # raycall.oconv(
+    #     str(model.material_path),
+    #     *map(str, config["Model"]["scene"].split()),
+    #     bwindow_path,
+    #     outpath=cdmap_oct,
+    #     frozen=True,
+    # )
+    with open(cdmap_oct, "wb") as wtr:
+        wtr.write(
+            pr.oconv(
+                str(model.material_path),
+                *[str(s) for s in config["Model"].getpaths("scene")],
+                bwindow_path,
+                frozen=True,
+            )
+        )
     logger.info("Generating direct-sun matrix material map octree")
     os.remove(bwindow_path)
     os.remove(gwindow_path)
     return vmap_oct, cdmap_oct
 
 
 def direct_sun_matrix_pt(
@@ -429,29 +435,30 @@
     Args:
         smx_path: path to sun only sky matrix
     Returns:
         path to resulting direct sun matrix
     """
 
     logger.info("Direct sun matrix for sensor grid")
+    cdsenv = [model.material_path, model.black_env_path, *model.cfs_paths]
+    _cfs_name = "".join([Path(cfs).stem for cfs in model.cfs_paths])
     for grid_name, sender_grid in model.sender_grid.items():
         mpath.pcdsmx[grid_name] = Path(
-            "Matrices", f"pcdsmx_{model.name}_{grid_name}.mtx"
+            "Matrices", f"pcdsmx_{model.name}_{grid_name}_{_cfs_name}.mtx"
         )
         if regen(mpath.pcdsmx[grid_name], config):
             logger.info("Generating using rcontrib...")
             rcvr_sun = matrix.sun_as_receiver(
                 basis="r6",
                 smx_path=mpath.smx_sun,
                 window_normals=model.window_normals,
                 full_mod=True,
             )
             cdsmx_opt = config["SimControl"].getoptions("cdsmx_opt")
             cdsmx_opt["n"] = config["SimControl"].getint("nprocess")
-            cdsenv = [model.material_path, model.black_env_path, *model.cfs_paths]
             sun_oct = Path(f"sun_{utils.id_generator()}.oct")
             matrix.rcvr_oct(rcvr_sun, cdsenv, sun_oct)
             matrix.rcontrib(
                 sender_grid,
                 rcvr_sun.modifier,
                 sun_oct,
                 mpath.pcdsmx[grid_name],
@@ -476,38 +483,36 @@
     logger.info("Direct sun matrix for view (image)")
     rcvr_sun = matrix.sun_as_receiver(
         basis="r6", smx_path=mpath.smx_sun_img, window_normals=model.window_normals
     )
     mod_names = [f"{int(line[3:]):04d}" for line in rcvr_sun.modifier.splitlines()]
     sun_oct = Path(f"sun_{utils.id_generator()}.oct")
     cdsenv = [model.material_path, model.black_env_path, *model.cfs_paths]
+    _cfs_name = "".join([Path(cfs).stem for cfs in model.cfs_paths])
     matrix.rcvr_oct(rcvr_sun, cdsenv, sun_oct)
     cdsmx_opt = config["SimControl"].getoptions("cdsmx_opt")
     cdsmx_opt["n"] = config["SimControl"].getint("nprocess")
     cdsmx_opt_list = utils.opt2list(cdsmx_opt)
     for view, sndr in model.sender_view.items():
         mpath.vmap[view] = Path("Matrices", f"vmap_{model.name}_{view}.hdr")
         mpath.cdmap[view] = Path("Matrices", f"cdmap_{model.name}_{view}.hdr")
-        # view = model.views[view]
-        # vdict.pop("c", None)
-        # vdict.pop("pj", None)
-        rpict_opt = Options()
+        rpict_opt = pr.SamplingParameters()
         rpict_opt.ps = 1
         rpict_opt.ab = 0
         rpict_opt.av = (0.31831, 0.31831, 0.31831)
-        cmd = raycall.get_rpict_command(model.views[view], rpict_opt, octree=vmap_oct)
-        logger.info("Generating view matrix material map with: \n %s", " ".join(cmd))
-        utils.run_write(cmd, mpath.vmap[view])
-        cmd[-1] = cdmap_oct
-        logger.info(
-            "Generating direct-sun matrix material map with: \n %s", " ".join(cmd)
-        )
-        utils.run_write(cmd, mpath.cdmap[view])
-        mpath.vcdfmx[view] = Path("Matrices", f"vcdfmx_{model.name}_{view}")
-        mpath.vcdrmx[view] = Path("Matrices", f"vcdrmx_{model.name}_{view}")
+        with open(mpath.vmap[view], "wb") as wtr:
+            wtr.write(
+                pr.rpict(model.views[view].args(), vmap_oct, params=rpict_opt.args())
+            )
+        with open(mpath.cdmap[view], "wb") as wtr:
+            wtr.write(
+                pr.rpict(model.views[view].args(), cdmap_oct, params=rpict_opt.args())
+            )
+        mpath.vcdfmx[view] = Path("Matrices", f"vcdfmx_{model.name}_{view}_{_cfs_name}")
+        mpath.vcdrmx[view] = Path("Matrices", f"vcdrmx_{model.name}_{view}_{_cfs_name}")
         tempf = Path("Matrices", "vcdfmx")
         tempr = Path("Matrices", "vcdrmx")
         if regen(mpath.vcdfmx[view], config):
             logger.info("Generating direct sun f matrix for %s", view)
             matrix.rcontrib(sndr, rcvr_sun.modifier, sun_oct, tempf, cdsmx_opt_list)
             mpath.vcdfmx[view].mkdir(exist_ok=True)
             for idx, file in enumerate(sorted(tempf.glob("*.hdr"))):
@@ -711,24 +716,26 @@
         vresl = []
         vdresl = []
         with tf.TemporaryDirectory() as td:
             vrescdr = Path(tf.mkdtemp(dir=td))
             vrescdf = Path(tf.mkdtemp(dir=td))
             vrescd = Path(tf.mkdtemp(dir=td))
             cmds = []
-            cmds.append(
-                mtxmult.get_imgmult_cmd(
-                    mpath.vcdrmx[view] / "%04d.hdr", mpath.smx_sun_img, odir=vrescdr
+            if mpath.vcdrmx != {}:
+                cmds.append(
+                    mtxmult.get_imgmult_cmd(
+                        mpath.vcdrmx[view] / "%04d.hdr", mpath.smx_sun_img, odir=vrescdr
+                    )
                 )
-            )
-            cmds.append(
-                mtxmult.get_imgmult_cmd(
-                    mpath.vcdfmx[view] / "%04d.hdr", mpath.smx_sun_img, odir=vrescdf
+            if mpath.vcdfmx != {}:
+                cmds.append(
+                    mtxmult.get_imgmult_cmd(
+                        mpath.vcdfmx[view] / "%04d.hdr", mpath.smx_sun_img, odir=vrescdf
+                    )
                 )
-            )
             for wname in model.window_groups:
                 _vrespath = tf.mkdtemp(dir=td)
                 _vdrespath = tf.mkdtemp(dir=td)
                 cmds.append(
                     mtxmult.get_imgmult_cmd(
                         mpath.vvmx[view + wname],
                         model.bsdf_xml[wname],
@@ -837,99 +844,115 @@
         wea_data,
         wea_meta,
         daylight_hours_only=config.getboolean("Site", "daylight_hours_only"),
         start_hour=config.getfloat("Site", "start_hour"),
         end_hour=config.getfloat("Site", "end_hour"),
     )
     if regen(mpath.smx, config):
-        sky.gendaymtx(
-            mpath.smx,
-            int(config["SimControl"]["smx_basis"][-1]),
-            data=wea_data,
-            meta=wea_meta,
-            rotate=config["Site"]["orientation"],
-        )
+        with open(mpath.smx, "wb") as wtr:
+            wtr.write(
+                sky.genskymtx(
+                    mfactor=int(config["SimControl"]["smx_basis"][-1]),
+                    data=wea_data,
+                    meta=wea_meta,
+                    rotate=config["Site"].getfloat("orientation"),
+                )
+            )
     prep_2phase_pt(mpath, model, config)
     prep_2phase_vu(mpath, model, config)
     if not config.getboolean("SimControl", "no_multiply", fallback=False):
         calc_2phase_pt(mpath, model, datetime_stamps)
         calc_2phase_vu(mpath, model, datetime_stamps)
     return mpath
 
 
 def three_phase(
     model: MradModel, config: ConfigParser, direct: bool = False
 ) -> MradPath:
     """3/5-phase simulation workflow."""
     do_multiply = config.getboolean("SimControl", "no_multiply", fallback=False)
-    psteps = 12 if direct else 4
-    if do_multiply:
-        psteps += 2
     mpath = MradPath()
     wea_meta, wea_data, wea_name = get_wea_data(config)
     mpath.smx = Path("Matrices") / (wea_name + ".smx")
     wea_data, datetime_stamps = sky.filter_wea(
         wea_data,
         wea_meta,
         daylight_hours_only=config.getboolean("Site", "daylight_hours_only"),
         start_hour=config.getfloat("Site", "start_hour"),
         end_hour=config.getfloat("Site", "end_hour"),
     )
     if regen(mpath.smx, config):
-        sky.gendaymtx(
-            mpath.smx,
-            int(config["SimControl"]["smx_basis"][-1]),
-            data=wea_data,
-            meta=wea_meta,
-            rotate=config["Site"]["orientation"],
-        )
+        with open(mpath.smx, "wb") as wtr:
+            wtr.write(
+                sky.genskymtx(
+                    mfactor=int(config["SimControl"]["smx_basis"][-1]),
+                    data=wea_data,
+                    meta=wea_meta,
+                    rotate=config["Site"].getfloat("orientation"),
+                )
+            )
     view_matrix_pt(mpath, model, config)
     view_matrix_vu(mpath, model, config)
     daylight_matrix(mpath, model, config)
     if direct:
+        if not (orientation := config["Site"].getfloat("orientation")) in (None, 0):
+            rotate_radians = math.radians(orientation)
+            rotated_window_normals = [
+                n.rotate_3d(geom.Vector(0, 0, 1), rotate_radians)
+                for n in model.window_normals
+            ]
         wea_data_d6, datetime_stamps_d6 = sky.filter_wea(
             wea_data,
             wea_meta,
             daylight_hours_only=False,
             start_hour=0,
             end_hour=0,
             remove_zero=True,
-            window_normals=model.window_normals,
+            window_normals=rotated_window_normals
+            if orientation
+            else model.window_normals,
         )
         mpath.smxd = Path("Matrices") / (wea_name + "_d.smx")
-        sky.gendaymtx(
-            mpath.smxd,
-            int(config["SimControl"]["smx_basis"][-1]),
-            data=wea_data,
-            meta=wea_meta,
-            direct=True,
-        )
+        with open(mpath.smxd, "wb") as wtr:
+            wtr.write(
+                sky.genskymtx(
+                    mfactor=int(config["SimControl"]["smx_basis"][-1]),
+                    data=wea_data,
+                    meta=wea_meta,
+                    sun_only=True,
+                )
+            )
         mpath.smx_sun_img = Path("Matrices") / (wea_name + "_d6_img.smx")
-        sky.gendaymtx(
-            mpath.smx_sun_img,
-            int(config["SimControl"]["cdsmx_basis"][-1]),
-            data=wea_data_d6,
-            meta=wea_meta,
-            rotate=config["Site"]["orientation"],
-            onesun=True,
-            direct=True,
-        )
+        with open(mpath.smx_sun_img, "wb") as wtr:
+            wtr.write(
+                sky.genskymtx(
+                    mfactor=int(config["SimControl"]["cdsmx_basis"][-1]),
+                    data=wea_data_d6,
+                    meta=wea_meta,
+                    rotate=config["Site"].getfloat("orientation"),
+                    onesun=True,
+                    sun_only=True,
+                )
+            )
         mpath.smx_sun = Path("Matrices") / (wea_name + "_d6.smx")
-        sky.gendaymtx(
-            mpath.smx_sun,
-            int(config["SimControl"]["cdsmx_basis"][-1]),
-            data=wea_data,
-            meta=wea_meta,
-            rotate=config["Site"]["orientation"],
-            onesun=True,
-            direct=True,
-        )
+        with open(mpath.smx_sun, "wb") as wtr:
+            wtr.write(
+                sky.genskymtx(
+                    mfactor=int(config["SimControl"]["cdsmx_basis"][-1]),
+                    data=wea_data,
+                    meta=wea_meta,
+                    rotate=config["Site"].getfloat("orientation"),
+                    onesun=True,
+                    sun_only=True,
+                )
+            )
         vmap_oct, cdmap_oct = blacken_env(model, config)
         direct_sun_matrix_pt(mpath, model, config)
-        direct_sun_matrix_vu(mpath, model, vmap_oct, cdmap_oct, config)
+        if len(datetime_stamps_d6) > 0:
+            direct_sun_matrix_vu(mpath, model, vmap_oct, cdmap_oct, config)
         daylight_matrix(mpath, model, config, direct=True)
         view_matrix_pt(mpath, model, config, direct=True)
         view_matrix_vu(mpath, model, config, direct=True)
         os.remove(vmap_oct)
         os.remove(cdmap_oct)
         if not do_multiply:
             calc_5phase_pt(
```

### Comparing `frads-0.2.8/frads/mtxmult.py` & `frads-0.3.0/frads/mtxmult.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     cmds: List[List[str]] = []
     outs: List[str] = []
     for sky in sorted(sky_dir.glob("*")):
         out_path = out_dir / sky.with_suffix(".hdr")
         cmd = ["dctimestep"] + [str(f) for f in mtx]
         cmd.append(str(sky))
         cmds.append(cmd)
-        outs.append(out_path)
+        outs.append(str(out_path))
     utils.batch_process(cmds, opaths=outs, nproc=nproc)
 
 
 def batch_pcomb(
     inp: List[Path], ops: List[str], out_dir: Path, nproc: Optional[int] = None
 ) -> None:
     """
```

### Comparing `frads-0.2.8/frads/ncp.py` & `frads-0.3.0/frads/ncp.py`

 * *Files identical despite different names*

### Comparing `frads-0.2.8/frads/parsers.py` & `frads-0.3.0/frads/parsers.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,26 @@
 This module contains all data parsing routines.
 """
 import argparse
 import configparser
 from datetime import datetime
 from pathlib import Path
 import re
-import subprocess as sp
 from typing import Tuple, Any
 from typing import Dict
 from typing import Generator
 from typing import List
 from typing import Sequence
 from typing import Union
 
 from frads import geom
-from frads.types import Primitive
 from frads.types import PaneProperty
 from frads.types import View
-from frads.types import WeaMetaData
-from frads.types import WeaData
+from frads.sky import WeaMetaData
+from frads.sky import WeaData
 
 
 def parse_mrad_config(cfg_path: Path) -> configparser.ConfigParser:
     """Parse mrad configuration file."""
     if not cfg_path.is_file():
         raise FileNotFoundError(cfg_path)
     config = configparser.ConfigParser(
@@ -50,15 +48,14 @@
     data = []
     for li in content:
         line = li.split(",")
         year = int(line[0])
         month = int(line[1])
         day = int(line[2])
         hour = int(line[3]) - 1
-        hours = hour + 0.5
         dir_norm = float(line[14])
         dif_hor = float(line[15])
         cc = float(line[19])
         aod = float(line[26])
         data.append(
             WeaData(datetime(year, month, day, hour, 30), dir_norm, dif_hor, cc, aod)
         )
@@ -271,73 +268,20 @@
     """Parse real arguments to polygon.
     Args:
         primitive: a dictionary object containing a primitive
 
     Returns:
         modified primitive
     """
-    coords = real_args[1:]
-    arg_cnt = int(real_args[0])
+    coords = real_args
+    arg_cnt = len(real_args)
     vertices = [geom.Vector(*coords[i : i + 3]) for i in range(0, arg_cnt, 3)]
     return geom.Polygon(vertices)
 
 
-def parse_primitive(lines: list) -> List[Primitive]:
-    """Parse Radiance primitives inside a file path into a list of dictionary.
-    Args:
-        lines: list of lines as strings
-
-    Returns:
-        list of primitives as dictionaries
-
-    Notes:
-        Dropping support for alias type
-    """
-    # Expand in-line commands
-    cmd_lines = [(idx, line) for idx, line in enumerate(lines) if line.startswith("!")]
-    cmd_results = []
-    for cmd in cmd_lines:
-        cmd_results.append(
-            sp.run(cmd[1][1:], check=True, stdout=sp.PIPE).stdout.decode().splitlines()
-        )
-    counter = 0
-    for idx, item in enumerate(cmd_lines):
-        counter += item[0]
-        lines[counter : counter + 1] = cmd_results[idx]
-        counter += len(cmd_results[idx]) - 1 - item[0]
-
-    content = " ".join(
-        [i.strip() for i in lines if i.strip() != "" and i[0] != "#"]
-    ).split()
-    primitives: List[Primitive] = []
-    idx = 0
-    while idx < len(content):
-        _modifier = content[idx]
-        _type = content[idx + 1]
-        if _type == "alias":
-            # _name_to = content[idx + 2]
-            # _name_from = content[idx + 3]
-            # primitives.append(
-            # Alias(_modifier, _name_to, _name_from)
-            # )
-            idx += 4
-            continue
-        _identifier = content[idx + 2]
-        str_arg_cnt = int(content[idx + 3])
-        _str_args = content[idx + 3 : idx + 4 + str_arg_cnt]
-        idx += 5 + str_arg_cnt
-        real_arg_cnt = int(content[idx])
-        _real_args = [float(i) for i in content[idx : idx + 1 + real_arg_cnt]]
-        idx += real_arg_cnt + 1
-        primitives.append(
-            Primitive(_modifier, _type, _identifier, _str_args, _real_args)
-        )
-    return primitives
-
-
 def parse_rad_header(header_str: str) -> tuple:
     """Parse a Radiance matrix file header.
 
     Args:
         header_str(str): header as string
     Returns:
         A tuple contain nrow, ncol, ncomp, datatype
@@ -383,15 +327,17 @@
     vparser.add_argument("-vs", type=float)
     vparser.add_argument("-vl", type=float)
     vparser.add_argument("-x", type=int)
     vparser.add_argument("-y", type=int)
     vparser.add_argument("-vf", type=argparse.FileType("r"))
     args, _ = vparser.parse_known_args(args_list)
     if args.vf is not None:
-        args, _ = vparser.parse_known_args(args.vf.readline().strip().split(), namespace=args)
+        args, _ = vparser.parse_known_args(
+            args.vf.readline().strip().split(), namespace=args
+        )
         args.vf.close()
     if None in (args.vp, args.vd):
         raise ValueError("Invalid view")
     view = View(geom.Vector(*args.vp), geom.Vector(*args.vd))
     if args.vt is not None:
         view.vtype = args.vt[-1]
     if args.x is not None:
```

### Comparing `frads-0.2.8/frads/room.py` & `frads-0.3.0/frads/room.py`

 * *Files identical despite different names*

### Comparing `frads-0.2.8/frads/sky.py` & `frads-0.3.0/frads/sky.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,33 +4,87 @@
 
 import datetime
 import logging
 import math
 import os
 from pathlib import Path
 import subprocess as sp
-from typing import SupportsFloat, Any
-from typing import List
-from typing import Optional
-from typing import Sequence
-from typing import Tuple
-from typing import Union
-
-from frads import geom
-from frads import parsers
-from frads.types import WeaMetaData
-from frads.types import WeaData
-from frads import utils
+from typing import Any, List, NamedTuple, Optional, Sequence, Tuple, Union
+
+import pyradiance as pr
+
+from frads import geom, utils
 
 logger: logging.Logger = logging.getLogger("frads.sky")
 
 # Solar disk solid angle (sr)
 SOLAR_SA = 6.7967e-5
 
 
+class WeaMetaData(NamedTuple):
+    """Weather related meta data object.
+
+    Attributes:
+        city: City.
+        country: Country.
+        latitude: Latitude.
+        longitude: Longitude.
+        timezone: Timezone as standard meridian.
+        elevation: Site elevation (m).
+    """
+
+    city: str
+    country: str
+    latitude: float
+    longitude: float
+    timezone: int
+    elevation: float
+
+    def wea_header(self) -> str:
+        """Return a .wea format header."""
+        return (
+            f"place {self.city}_{self.country}\n"
+            f"latitude {self.latitude}\n"
+            f"longitude {self.longitude}\n"
+            f"time_zone {self.timezone}\n"
+            f"site_elevation {self.elevation}\n"
+            "weather_data_file_units 1\n"
+        )
+
+
+class WeaData(NamedTuple):
+    """Weather related data object.
+
+    Attributes:
+        month: Month.
+        day: Day.
+        hour: Hour.
+        minute: Minutes.
+        second: Seconds.
+        hours: Times with minutes as fraction.
+        dni: Direct normal irradiance (W/m2).
+        dhi: Diffuse horizontal irradiance (W/m2).
+        aod: Aeroal Optical Depth (default = 0).
+        cc: Cloud cover (default = 0).
+        year: default = 2000.
+    """
+
+    time: datetime.datetime
+    dni: float
+    dhi: float
+    aod: float = 0
+    cc: float = 0
+
+    def __str__(self) -> str:
+        return f"{self.time.month} {self.time.day} {self.time.hour+self.time.minute/60} {self.dni} {self.dhi}"
+
+    def dt_str(self) -> str:
+        return f"{self.time.month:02d}{self.time.day:02d}_{self.time.hour:02d}{self.time.minute:02d}"
+
+
 def basis_glow(sky_basis: str) -> str:
     """
     Generate a set of regular sky and ground glow primitives string.
 
     Args:
         sky_basis(str): sky sampling basis, e.g. r1, r4
     Returns:
@@ -83,15 +137,15 @@
         mf(int): multiplication factor, usually 1, 2, or 4.
     Returns:
         A tuple of full set of sun light and source primitive string
         and associated modifier string.
     """
     runlen = 144 * mf**2 + 3
     mod_str = os.linesep.join([f"sol{i}" for i in range(1, runlen)])
-    dirs, omgs = utils.calc_reinsrc_dir(mf)
+    dirs, _ = utils.calc_reinsrc_dir(mf)
     lines = []
     for i, d in enumerate(dirs):
         lines.append(
             f"void light sol{i} 0 0 3 1 1 1 sol{i} source sun "
             f"0 0 4 {d.x:.6g} {d.y:.6g} {d.z:.6g} 0.533"
         )
     return os.linesep.join(lines) + os.linesep, mod_str
@@ -112,15 +166,15 @@
         smx_path(str): Optional, sky matrix path, usually the output of gendaymtx
         window_normals(str): Optional, window normals
     Returns:
         A tuple of culled set of sun light and source primitive string,
         corresponding modifier strings, and the full set of modifier string.
     """
     runlen = 144 * mf**2 + 3
-    dirs, omgs = utils.calc_reinsrc_dir(mf)
+    dirs, _ = utils.calc_reinsrc_dir(mf)
     full_mod_str = os.linesep.join([f"sol{i}" for i in range(1, runlen)])
     win_norm = []
     if smx_path is not None:
         cmd1 = ["rmtxop", "-ff", "-c", ".3", ".6", ".1", "-t", str(smx_path)]
         cmd2 = ["getinfo", "-"]
         cmd3 = ["total", f"-if{runlen-1}", "-t,"]
         proc1 = sp.run(cmd1, check=True, stdout=sp.PIPE)
@@ -158,26 +212,33 @@
                 f"0 0 4 {d.x:.6g} {d.y:.6g} {d.z:.6g} 0.533"
             )
     logger.debug(out_lines)
     logger.debug(mod_str)
     return os.linesep.join(out_lines), os.linesep.join(mod_str), full_mod_str
 
 
-def gendaymtx(
-    out: Union[str, Path],
-    mf: int,
+def genskymtx(
     data: Optional[Sequence[WeaData]] = None,
     meta: Optional[WeaMetaData] = None,
-    wpath: Optional[Path] = None,
-    direct: bool = False,
-    solar: bool = False,
+    wpath: Optional[Union[str, Path]] = None,
     onesun: bool = False,
+    header: bool = True,
+    average: bool = False,
+    sun_only: bool = False,
+    sky_only: bool = False,
+    sun_file: Optional[str] = None,
+    sun_mods: Optional[str] = None,
+    daylight_hours_only: bool = False,
+    sky_color: Optional[List[float]] = None,
+    ground_color: Optional[List[float]] = None,
     rotate: Optional[float] = None,
-    binary: bool = False,
-) -> List[str]:
+    outform: Optional[str] = None,
+    solar_radiance: bool = False,
+    mfactor: int = 1,
+) -> bytes:
     """
     Call gendaymtx to generate a sky/sun matrix
     and write results to out.  It takes either a .wea file path
     or wea data and metadata (defined in frads.types).
     If both are provided, .wea file path will be used.
 
     Args:
@@ -192,90 +253,203 @@
         rotate(float, optional): rotate the sky counter-clock wise, looking down.
         binary(bool, optional): Whether to have outputs in single precision floats.
     Returns:
         cmd(List[str]): the gendaymtx command called.
     Raises:
         ValueError: An error occurs if neither a .wea path nor wea data is provided.
     """
-    stdin = None
-    cmd = ["gendaymtx", "-m", str(mf)]
-    if binary:
-        cmd.append("-of")
-    if direct:
-        cmd.append("-d")
-    if onesun:
-        cmd.extend(["-5", ".533"])
-    if rotate is not None:
-        cmd.extend(["-r", str(rotate)])
-    if solar:
-        cmd.append("-O1")
-    if wpath is not None:
-        cmd.append(str(wpath))
-    elif (data is not None) and (meta is not None):
-        wea_input = meta.wea_header() + "\n".join(map(str, data))
-        stdin = wea_input.encode("utf-8")
+    if wpath is None:
+        if data is not None and meta is not None:
+            inp = gen_wea(
+                [d.time for d in data],
+                [d.dni for d in data],
+                [d.dhi for d in data],
+                meta.latitude,
+                meta.longitude,
+                meta.timezone,
+                elevation=meta.elevation,
+                location=meta.city + meta.country,
+            ).encode()
+        else:
+            raise ValueError("Either a .wea path or wea data is required.")
     else:
-        raise ValueError("Need to specify either .wea path or wea data.")
-    with open(out, "wb") as wtr:
-        logger.info("Calling gendaymtx with:\n%s", " ".join(cmd))
-        sp.run(cmd, check=True, input=stdin, stdout=wtr)
-    return cmd
-
+        inp = wpath
+    _err, _out = pr.gendaymtx(
+        inp,
+        header=header,
+        average=average,
+        sun_only=sun_only,
+        sky_only=sky_only,
+        solar_radiance=solar_radiance,
+        sun_file=sun_file,
+        sun_mods=sun_mods,
+        daylight_hours_only=daylight_hours_only,
+        sky_color=sky_color,
+        ground_color=ground_color,
+        rotate=rotate,
+        outform=outform,
+        onesun=onesun,
+        mfactor=mfactor,
+    )
+    logger.warning(_err)
+    return _out
 
-def gen_perez_sky(row, meta, grefl: float = 0.2, spect: str = "0", rotate=None) -> str:
-    gendaylit = gendaylit_cmd(
-        str(row.month),
-        str(row.day),
-        str(row.hours),
-        str(meta.latitude),
-        str(meta.longitude),
-        str(meta.timezone),
-        dir_norm_ir=str(row.dni),
-        dif_hor_ir=str(row.dhi),
+    # stdin = None
+    # cmd = ["gendaymtx", "-m", str(mf)]
+    # if binary:
+    #     cmd.append("-of")
+    # if direct:
+    #     cmd.append("-d")
+    # if onesun:
+    #     cmd.extend(["-5", ".533"])
+    # if rotate is not None:
+    #     cmd.extend(["-r", str(rotate)])
+    # if solar:
+    #     cmd.append("-O1")
+    # if wpath is not None:
+    #     cmd.append(str(wpath))
+    # elif (data is not None) and (meta is not None):
+    #     wea_input = meta.wea_header() + "\n".join(map(str, data))
+    #     stdin = wea_input.encode("utf-8")
+    # else:
+    #     raise ValueError("Need to specify either .wea path or wea data.")
+    # if out is not None:
+    #     with open(out, "wb") as wtr:
+    #         logger.info("Calling gendaymtx with:\n%s", " ".join(cmd))
+    #         sp.run(cmd, check=True, input=stdin, stdout=wtr)
+    # return cmd
+
+
+# def gen_perez_sky(row: WeaData, meta, grefl: float = 0.2, spect: str = "0", rotate=None) -> str:
+#     solar = False if spect == "0" else True
+#     gendaylit = gendaylit_cmd(
+#         str(row.time.month),
+#         str(row.time.day),
+#         str(row.time.hour + row.time.minute / 60 + row.time.second / 3600),
+#         str(meta.latitude),
+#         str(meta.longitude),
+#         str(meta.timezone),
+#         dir_norm_ir=str(row.dni),
+#         dif_hor_ir=str(row.dhi),
+#         solar=solar,
+#         grefl=grefl,
+#     )
+#     out = []
+#     rot = f"| xform -rz {rotate}" if rotate is not None else ""
+#     out.append(f"!{' '.join(gendaylit)}{rot} \n")
+#     out.append("skyfunc glow sglow 0 0 4 1 1 1 0\n")
+#     out.append("sglow source sky 0 0 4 0 0 1 180\n")
+#     out.append("sglow source ground 0 0 4 0 0 -1 180\n")
+#     return " ".join(out)
+
+
+def gen_perez_sky(
+    dt,
+    latitude: float,
+    longitude: float,
+    timezone: int,
+    year: Optional[int] = None,
+    dirnorm: Optional[float] = None,
+    diffhor: Optional[float] = None,
+    dirhor: Optional[float] = None,
+    dirnorm_illum: Optional[float] = None,
+    diffhor_illum: Optional[float] = None,
+    solar: bool = False,
+    grefl: Optional[float] = None,
+    rotate: Optional[float] = None,
+) -> bytes:
+    sun = pr.gendaylit(
+        dt,
+        latitude,
+        longitude,
+        timezone,
+        year,
+        dirnorm=dirnorm,
+        diffhor=diffhor,
+        dirhor=dirhor,
+        dirnorm_illum=dirnorm_illum,
+        diffhor_illum=diffhor_illum,
+        solar=solar,
+        grefl=grefl,
     )
-    out = []
-    rot = f"| xform -rz {rotate}" if rotate is not None else ""
-    out.append(f"!{' '.join(gendaylit)}{rot} \n")
-    out.append("skyfunc glow sglow 0 0 4 1 1 1 0\n")
-    out.append("sglow source sky 0 0 4 0 0 1 180\n")
-    out.append("sglow source ground 0 0 4 0 0 -1 180\n")
-    return " ".join(out)
+    if rotate:
+        sun = pr.xform(sun, rotatez=rotate)
+    out = [b"skyfunc glow sglow 0 0 4 1 1 1 0"]
+    out.append(b"sglow source sky 0 0 4 0 0 1 180")
+    out.append(b"sglow source ground 0 0 4 0 0 -1 180")
+    return sun + b"\n".join(out)
 
 
 def gendaylit_cmd(
     month: str,
     day: str,
     hours: str,
     lat: str,
     lon: str,
     tzone: str,
-    year: str = None,
-    dir_norm_ir: str = None,
+    year: Optional[str] = None,
+    grefl: Optional[float] = None,
+    dir_norm_ir: Optional[str] = None,
     dif_hor_ir: Optional[str] = None,
     dir_hor_ir: Optional[str] = None,
     dir_norm_il: Optional[str] = None,
-    dif_hor_il: str = None,
+    dif_hor_il: Optional[str] = None,
     solar: bool = False,
 ) -> list:
     """Get a gendaylit command as a list."""
     cmd = ["gendaylit", month, day, hours]
     cmd += ["-a", lat, "-o", lon, "-m", tzone]
+    if grefl is not None:
+        cmd += ["-g", str(grefl)]
     if year is not None:
         cmd += ["-y", year]
     if None not in (dir_norm_ir, dif_hor_ir):
         cmd += ["-W", str(dir_norm_ir), str(dif_hor_ir)]
     if None not in (dir_hor_ir, dif_hor_ir):
         cmd += ["-G", str(dir_hor_ir), str(dif_hor_ir)]
     if None not in (dir_norm_il, dif_hor_il):
         cmd += ["-L", str(dir_norm_il), str(dif_hor_il)]
     if solar:
         cmd += ["-O", "1"]
     return cmd
 
 
+def gen_wea(
+    datetimes: Sequence[datetime.datetime],
+    dirnorm: Sequence[float],
+    diffhor: Sequence[float],
+    latitude: float,
+    longitude: float,
+    timezone: int,
+    elevation: Optional[float] = None,
+    location: Optional[str] = None,
+) -> str:
+    """Generate wea file from datetime, location, and sky."""
+    if len(datetimes) != len(dirnorm) != len(diffhor):
+        raise ValueError("datetimes, dirnorm, and diffhor must be the same length")
+    rows = []
+    if location is None or location == "":
+        location = "_".join(
+            [str(i) for i in [latitude, longitude, timezone, elevation]]
+        )
+    if elevation is None:
+        elevation = 0
+    rows.append(f"place {location}")
+    rows.append(f"latitude {latitude}")
+    rows.append(f"longitude {longitude}")
+    rows.append(f"time_zone {timezone}")
+    rows.append(f"site_elevation {elevation}")
+    rows.append("weather_data_file_units 1")
+    for dt, dni, dhi in zip(datetimes, dirnorm, diffhor):
+        _hrs = dt.hour + dt.minute / 60  # middle of hour
+        _row = f"{dt.month} {dt.day} {_hrs} {dni} {dhi}"
+        rows.append(_row)
+    return "\n".join(rows)
+
+
 def solar_angle(
     lat: float,
     lon: float,
     mer: float,
     month,
     day: int,
     hour,
@@ -342,15 +516,15 @@
 def filter_data_with_zero_dni(data):
     """Filter out data entries with zero direct normal irradiance."""
     return [row for row in data if row.dni != 0]
 
 
 def solar_minute(data: WeaData) -> int:
     # assuming never leap year
-    mo_da = [0,31,59,90,120,151,181,212,243,273,304,334]
+    mo_da = [0, 31, 59, 90, 120, 151, 181, 212, 243, 273, 304, 334]
     jd = mo_da[data.time.month - 1] + data.time.day
     return 24 * 60 * (jd - 1) + int(data.time.hour * 60.0 + data.time.minute + 0.5)
 
 
 def filter_data_by_direct_sun(
     data: Sequence[WeaData],
     meta: WeaMetaData,
@@ -366,37 +540,39 @@
         data: Sequence[WeaData],
         meta: WeaMetaData,
         window_normal: Optional[Sequence[geom.Vector]] = None,
     Returns:
         data(List[WeaData]):
     """
     wea_input = meta.wea_header() + "\n".join(map(str, data))
+    # pr.gendaymtx(wea_input, daylight_only=True, )
     proc = sp.run(
         ["gendaymtx", "-u", "-D", "-"],
         check=True,
         input=wea_input,
         encoding="ascii",
         stderr=sp.PIPE,
         stdout=sp.PIPE,
     )
-    prims = parsers.parse_primitive(proc.stdout.splitlines())
+    # prims = parsers.parse_primitive(proc.stdout.splitlines())
+    prims = pr.parse_primitive(proc.stdout)
     light_prims = [prim for prim in prims if prim.ptype == "light"]
     keep_minutes = []
     if window_normal is not None:
         source_prims = [prim for prim in prims if prim.ptype == "source"]
         for lpr, spr in zip(light_prims, source_prims):
-            if lpr.real_arg[1] > 0:
-                sdir = geom.Vector(*spr.real_arg[1:4])
+            if lpr.fargs[0] > 0:
+                sdir = geom.Vector(*spr.fargs[:3])
                 for normal in window_normal:
                     if normal * sdir < -0.035:  # 2deg tolerance
                         keep_minutes.append(int(spr.modifier.lstrip("solar")))
                         break
     else:
         for lpr in light_prims:
-            if lpr.real_arg[1] > 0:
+            if lpr.fargs[0] > 0:
                 keep_minutes.append(int(lpr.identifier.lstrip("solar")))
     # inminutes = [solar_minute(d) for d in data]
     inminutes = []
     extra_day = 0
     for d in data:
         inm = solar_minute(d)
         if d.time.month == 2 and d.time.day == 29:
@@ -404,22 +580,22 @@
         inm += extra_day
         inminutes.append(inm)
     new_dataline = [data for data, minu in zip(data, inminutes) if minu in keep_minutes]
     return new_dataline
 
 
 def filter_wea(
-    wea_data: List[WeaData],
+    wea_data: Sequence[WeaData],
     meta_data: WeaMetaData,
     start_hour: Optional[float] = None,
     end_hour: Optional[float] = None,
     daylight_hours_only: bool = False,
     remove_zero: bool = False,
     window_normals: Optional[List[geom.Vector]] = None,
-) -> Tuple[List[WeaData], List[Any]]:
+) -> Tuple[Sequence[WeaData], List[Any]]:
     """
     Obtain and prepare weather file data.
 
     Args:
         wea_data(List[WeaData]): A list of WeaData.
         meta_data(WeaMetaData): A instance of WeaMetaData object.
         start_hour(float, optional): Filter out wea data before this hour.
@@ -450,11 +626,11 @@
         wea_data = filter_data_by_direct_sun(
             wea_data, meta_data, window_normal=window_normals
         )
         logger.info(
             "Filtering zero DNI hours and suns not seen by window: %d rows remaining",
             len(wea_data),
         )
-    datetime_stamps = [str(row) for row in wea_data]
+    datetime_stamps = [row.dt_str() for row in wea_data]
     if len(wea_data) == 0:
         logger.warning("Empty wea file")
     return wea_data, datetime_stamps
```

### Comparing `frads-0.2.8/frads/types.py` & `frads-0.3.0/frads/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 # frads/types.py
 """
 This module contains all data types used across frads.
 The exceptions are the Vector and Polygon class in the geom.py module.
 
 """
 
-import datetime
 from dataclasses import dataclass
 from dataclasses import field
 from pathlib import Path
-from typing import Dict
-from typing import Iterable
-from typing import List
-from typing import NamedTuple
-from typing import Optional
-from typing import Sequence
-from typing import Tuple
-from typing import Union
+from typing import Dict, Iterable, List, NamedTuple, Optional, Sequence, Tuple, Union
+
 
 from frads.geom import Polygon
 from frads.geom import Vector
 
 
 class Primitive(NamedTuple):
     """Radiance Primitive.
@@ -73,106 +66,14 @@
         return output
 
     def __str__(self) -> str:
         output = f"{self.modifier} alias {self.name_to} {self.name_from}"
         return output
 
 
-@dataclass(frozen=True)
-class Sender:
-    """Sender object for matrix generation.
-
-    Attributes:
-        form: types of sender, {surface(s)|view(v)|points(p)}
-        sender: the sender string
-        xres: sender x dimension
-        yres: sender y dimension
-    """
-
-    form: str
-    sender: bytes
-    xres: Optional[int]
-    yres: Optional[int]
-
-
-@dataclass
-class Receiver:
-    """Receiver object for matrix generation.
-
-    Attributes:
-        receiver: receiver string which can be appended to one another
-        basis: receiver basis, usually kf, r4, r6;
-        modifier: modifiers to the receiver objects;
-    """
-
-    receiver: str
-    basis: str
-    modifier: str = ""
-
-    def __add__(self, other) -> "Receiver":
-        return Receiver(
-            self.receiver + "\n" + other.receiver, self.basis, self.modifier
-        )
-
-
-@dataclass
-class ScatteringData:
-    """Scattering data object.
-
-    Attributes:
-        sdata: scattering data in nested lists.
-        ncolumn: number of columns
-        nrow: number of rows
-    """
-
-    sdata: List[float]
-    ncolumn: int
-    nrow: int
-
-    def __str__(self) -> str:
-        out = "#?RADIANCE\nNCOMP=3\n"
-        out += f"NROWS={self.nrow}\nNCOLS={self.ncolumn}\n"
-        out += "FORMAT=ascii\n\n"
-        for col in range(self.ncolumn):
-            for row in range(self.nrow):
-                val = self.sdata[row + col * self.ncolumn]
-                string = "\t".join([f"{val:7.5f}"] * 3)
-                out += string + "\t"
-            out += "\n"
-        return out
-
-
-@dataclass
-class BSDFData:
-    """BSDF data object.
-
-    Attributes:
-        bsdf: BSDF data.
-        ncolumn: number of columns
-        nrow: number of rows
-    """
-
-    bsdf: List[float]
-    ncolumn: int
-    nrow: int
-
-
-@dataclass(frozen=True)
-class RadMatrix:
-    """Radiance matrix object.
-
-    Attributes:
-        tf: front-side transmission
-        tb: back-side transmission
-    """
-
-    tf: ScatteringData
-    tb: ScatteringData
-
-
 class PaneProperty(NamedTuple):
     """Window pane property object.
 
     Attributes:
         name str: material name.
         thickness float: pane thickness.
         gtype str: material type.
@@ -212,75 +113,17 @@
         measured_data: measured data as a PaneProperty object.
         coated_rgb: Coated side RGB.
         glass_rgb: Non-coated side RGB.
         trans_rgb: Transmittance RGB.
     """
 
     measured_data: PaneProperty
-    coated_rgb: List[float]
-    glass_rgb: List[float]
-    trans_rgb: List[float]
-
-
-class WeaMetaData(NamedTuple):
-    """Weather related meta data object.
-
-    Attributes:
-        city: City.
-        country: Country.
-        latitude: Latitude.
-        longitude: Longitude.
-        timezone: Timezone as standard meridian.
-        elevation: Site elevation (m).
-    """
-
-    city: str
-    country: str
-    latitude: float
-    longitude: float
-    timezone: int
-    elevation: float
-
-    def wea_header(self) -> str:
-        """Return a .wea format header."""
-        return (
-            f"place {self.city}_{self.country}\n"
-            f"latitude {self.latitude}\n"
-            f"longitude {self.longitude}\n"
-            f"time_zone {self.timezone}\n"
-            f"site_elevation {self.elevation}\n"
-            "weather_data_file_units 1\n"
-        )
-
-
-class WeaData(NamedTuple):
-    """Weather related data object.
-
-    Attributes:
-        month: Month.
-        day: Day.
-        hour: Hour.
-        minute: Minutes.
-        second: Seconds.
-        hours: Times with minutes as fraction.
-        dni: Direct normal irradiance (W/m2).
-        dhi: Diffuse horizontal irradiance (W/m2).
-        aod: Aeroal Optical Depth (default = 0).
-        cc: Cloud cover (default = 0).
-        year: default = 2000.
-    """
-
-    time: datetime.datetime
-    dni: float
-    dhi: float
-    aod: float = 0
-    cc: float = 0
-
-    def __str__(self) -> str:
-        return f"{self.time.month} {self.time.day} {self.time.hour+self.time.minute/60} {self.dni} {self.dhi}"
+    coated_rgb: Iterable[float]
+    glass_rgb: Iterable[float]
+    trans_rgb: Iterable[float]
 
 
 class MradModel(NamedTuple):
     """Mrad model object.
     Attributes:
         name: Model name
         material_path: Material path
@@ -400,14 +243,32 @@
 
     name: str
     visible_transmittance: float
     primitive: Primitive
 
 
 @dataclass
+class EPlusWindowMaterialComplexShade:
+    """EnergyPlus complex window material data container."""
+
+    name: str
+    layer_type: str
+    thickness: float
+    conductivity: float
+    ir_transmittance: float
+    front_emissivity: float
+    back_emissivity: float
+    top_opening_multiplier: float
+    bottom_opening_multiplier: float
+    left_side_opening_multiplier: float
+    right_side_opening_multiplier: float
+    front_opening_multiplier: float
+
+
+@dataclass
 class EPlusConstruction:
     """EnergyPlus construction data container."""
 
     name: str
     type: str
     layers: list
 
@@ -457,14 +318,15 @@
     angular_fisheye = "a"
     planisphere_fishsye = "s"
 
 
 @dataclass
 class View:
     """View data object."""
+
     position: Vector
     direction: Vector
     up: Vector = Vector(0, 0, 1)
     vtype: str = "v"
     vert: float = 45
     hori: float = 45
     aft: float = 0
@@ -568,15 +430,15 @@
 
 class Options:
     aa: float = FloatArg()
     ab: int = IntArg()
     ad: int = IntArg()
     ar: int = IntArg()
     as_: int = IntArg()
-    av: Tuple[float] = TupleArg()
+    av: Tuple[float, float, float] = TupleArg()
     aw: int = IntArg()
     dc: float = FloatArg()
     dj: float = FloatArg()
     dr: int = IntArg()
     dp: int = IntArg()
     ds: float = FloatArg()
     dt: float = FloatArg()
```

### Comparing `frads-0.2.8/frads/utils.py` & `frads-0.3.0/frads/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,123 +4,55 @@
 from io import TextIOWrapper
 import logging
 import math
 from pathlib import Path
 import random
 import string
 import subprocess as sp
-from typing import Any, Dict, Optional, List
-from typing import Set
-from typing import Tuple
-from typing import Union
-
-from frads import geom
-from frads import parsers
-from frads.types import Primitive
+from typing import Any, Dict, Optional, List, Set, Tuple, Union
+import sys
+sys.path.insert(0, ".")
+
+from frads import geom, parsers
 from frads.types import PaneRGB
-from frads.types import ScatteringData
-from frads.types import BSDFData
+from pyradiance import Primitive, parse_primitive
 
 
 logger: logging.Logger = logging.getLogger("frads.utils")
 
 
 GEOM_TYPE = ["polygon", "ring", "tube", "cone"]
 
 MATERIAL_TYPE = ["plastic", "glass", "trans", "dielectric", "BSDF"]
 
-BASIS_DICT = {
-    "145": "Klems Full",
-    "73": "Klems Half",
-    "41": "Klems Quarter",
-}
 
 TREG_BASE = [
     (90.0, 0),
     (78.0, 30),
     (66.0, 30),
     (54.0, 24),
     (42.0, 24),
     (30.0, 18),
     (18.0, 12),
     (6.0, 6),
     (0.0, 1),
 ]
 
-ABASE_LIST = {
-    "Klems Full": [
-        (0.0, 1),
-        (5.0, 8),
-        (15.0, 16),
-        (25.0, 20),
-        (35.0, 24),
-        (45.0, 24),
-        (55.0, 24),
-        (65.0, 16),
-        (75.0, 12),
-        (90.0, 0),
-    ],
-    "Klems Half": [
-        (0.0, 1),
-        (6.5, 8),
-        (19.5, 12),
-        (32.5, 16),
-        (46.5, 20),
-        (61.5, 12),
-        (76.5, 4),
-        (90.0, 0),
-    ],
-    "Klems Quarter": [(0.0, 1), (9.0, 8), (27.0, 12), (46.0, 12), (66.0, 8), (90.0, 0)],
-}
-
-
-def tmit2tmis(tmit: float) -> float:
-    """Convert from transmittance to transmissivity."""
-    tmis = round(
-        (math.sqrt(0.8402528435 + 0.0072522239 * tmit**2) - 0.9166530661)
-        / 0.0036261119
-        / tmit,
-        3,
-    )
-    return max(0, min(tmis, 1))
-
 
 def polygon2prim(polygon: geom.Polygon, modifier: str, identifier: str) -> Primitive:
     """Generate a primitive from a polygon."""
-    return Primitive(modifier, "polygon", identifier, ["0"], polygon.to_real())
+    return Primitive(modifier, "polygon", identifier, [""], polygon.to_real())
 
 
 def unpack_idf(path: str) -> dict:
     """Read and parse and idf files."""
     with open(path, "r") as rdr:
         return parsers.parse_idf(rdr.read())
 
 
-def sdata2bsdf(sdata: ScatteringData) -> BSDFData:
-    """Convert sdata object to bsdf object."""
-    basis = BASIS_DICT[str(sdata.ncolumn)]
-    lambdas = angle_basis_coeff(basis)
-    bsdf = []
-    for irow in range(sdata.nrow):
-        for icol, lam in zip(range(sdata.ncolumn), lambdas):
-            bsdf.append(sdata.sdata[icol + irow * sdata.ncolumn] / lam)
-    return BSDFData(bsdf, sdata.ncolumn, sdata.nrow)
-
-
-def bsdf2sdata(bsdf: BSDFData) -> ScatteringData:
-    """Covert a bsdf object into a sdata object."""
-    basis = BASIS_DICT[str(bsdf.ncolumn)]
-    lambdas = angle_basis_coeff(basis)
-    sdata = []
-    for irow in range(bsdf.nrow):
-        for icol, lam in zip(range(bsdf.ncolumn), lambdas):
-            sdata.append(bsdf.bsdf[icol + irow * bsdf.ncolumn] * lam)
-    return ScatteringData(sdata, bsdf.ncolumn, bsdf.nrow)
-
-
 def frange_inc(start, stop, step):
     """Generate increasing non-integer range."""
     r = start
     while r < stop:
         yield r
         r += step
 
@@ -164,38 +96,38 @@
         chars = string.ascii_uppercase + string.digits
     return "".join(random.choice(chars) for _ in range(size))
 
 
 def unpack_primitives(file: Union[str, Path, TextIOWrapper]) -> List[Primitive]:
     """Open a file a to parse primitive."""
     if isinstance(file, TextIOWrapper):
-        lines = file.readlines()
+        lines = file.read()
     else:
         with open(file, "r", encoding="ascii") as rdr:
-            lines = rdr.readlines()
-    return parsers.parse_primitive(lines)
+            lines = rdr.read()
+    return parse_primitive(lines)
 
 
 def primitive_normal(primitive_paths: List[str]) -> Set[geom.Vector]:
     """Return a set of normal vectors given a list of primitive paths."""
     _primitives: List[Primitive] = []
     _normals: List[geom.Vector]
     for path in primitive_paths:
         _primitives.extend(unpack_primitives(path))
-    _normals = [parsers.parse_polygon(prim.real_arg).normal for prim in _primitives]
+    _normals = [parsers.parse_polygon(prim.fargs).normal for prim in _primitives]
     return set(_normals)
 
 
 def samp_dir(primlist: list) -> geom.Vector:
     """Calculate the primitives' average sampling
     direction weighted by area."""
     primlist = [p for p in primlist if p.ptype in ("polygon", "ring")]
     normal_area = geom.Vector()
     for prim in primlist:
-        polygon = parsers.parse_polygon(prim.real_arg)
+        polygon = parsers.parse_polygon(prim.fargs)
         normal_area += polygon.normal.scale(polygon.area)
     sdir = normal_area.scale(1.0 / len(primlist))
     sdir = sdir.normalize()
     return sdir
 
 
 def up_vector(primitives: list) -> geom.Vector:
@@ -204,21 +136,19 @@
     Args:
         primitives: list of dictionary (primitives)
 
     Returns:
         returns a str as x,y,z
 
     """
-    xaxis = geom.Vector(1, 0, 0)
-    yaxis = geom.Vector(0, 1, 0)
     norm_dir = samp_dir(primitives)
-    if norm_dir not in (xaxis, xaxis.scale(-1)):
-        upvect = xaxis.cross(norm_dir)
+    if norm_dir != geom.Vector(0, 0, 1):
+        upvect = norm_dir.cross(geom.Vector(0, 0, 1).cross(norm_dir)).normalize()
     else:
-        upvect = yaxis.cross(norm_dir)
+        upvect = geom.Vector(0, 1, 0)
     return upvect
 
 
 def neutral_plastic_prim(
     mod: str, ident: str, refl: float, spec: float, rough: float
 ) -> Primitive:
     """Generate a neutral color plastic material.
@@ -230,16 +160,16 @@
         rough (float): material roughness (0.0 - 1.0)
 
     Returns:
         A material primtive
     """
     err_msg = "reflectance, speculariy, and roughness have to be 0-1"
     assert all(0 <= i <= 1 for i in [spec, refl, rough]), err_msg
-    real_args = [5, refl, refl, refl, spec, rough]
-    return Primitive(mod, "plastic", ident, ["0"], real_args)
+    real_args = [refl, refl, refl, spec, rough]
+    return Primitive(mod, "plastic", ident, [], real_args)
 
 
 def neutral_trans_prim(
     mod: str, ident: str, trans: float, refl: float, spec: float, rough: float
 ) -> Primitive:
     """Generate a neutral color plastic material.
     Args:
@@ -253,16 +183,16 @@
         A material primtive
     """
     color = trans + refl
     t_diff = trans / color
     tspec = 0
     err_msg = "reflectance, speculariy, and roughness have to be 0-1"
     assert all(0 <= i <= 1 for i in [spec, refl, rough]), err_msg
-    real_args = [7, color, color, color, spec, rough, t_diff, tspec]
-    return Primitive(mod, "trans", ident, ["0"], real_args)
+    real_args = [color, color, color, spec, rough, t_diff, tspec]
+    return Primitive(mod, "trans", ident, [], real_args)
 
 
 def color_plastic_prim(mod, ident, refl, red, green, blue, specu, rough) -> Primitive:
     """Generate a colored plastic material.
     Args:
         mod(str): modifier to the primitive
         ident(str): identifier to the primitive
@@ -279,16 +209,16 @@
     red_eff = 0.3
     green_eff = 0.59
     blue_eff = 0.11
     weighted = red * red_eff + green * green_eff + blue * blue_eff
     matr = round(red / weighted * refl, 3)
     matg = round(green / weighted * refl, 3)
     matb = round(blue / weighted * refl, 3)
-    real_args = [5, matr, matg, matb, specu, rough]
-    return Primitive(mod, "plastic", ident, "0", real_args)
+    real_args = [matr, matg, matb, specu, rough]
+    return Primitive(mod, "plastic", ident, [], real_args)
 
 
 def glass_prim(
     mod, ident, tr: float, tg: float, tb: float, refrac: float = 1.52
 ) -> Primitive:
     """Generate a glass material.
 
@@ -297,30 +227,30 @@
         ident (str): identifier to the primtive
         tr, tg, tb (float): transmmisivity in each channel (0.0 - 1.0)
         refrac (float): refraction index (default=1.52)
     Returns:
         material primtive (dict)
 
     """
-    tmsv_red = tmit2tmis(tr)
-    tmsv_green = tmit2tmis(tg)
-    tmsv_blue = tmit2tmis(tb)
-    real_args = [4, tmsv_red, tmsv_green, tmsv_blue, refrac]
-    return Primitive(mod, "glass", ident, ["0"], real_args)
+    tmsv_red = tr * 1.08981 
+    tmsv_green = tg * 1.08981
+    tmsv_blue = tb * 1.08981
+    real_args = [tmsv_red, tmsv_green, tmsv_blue, refrac]
+    return Primitive(mod, "glass", ident, [], real_args)
 
 
 def bsdf_prim(
     mod,
     ident,
     xmlpath,
     upvec,
     pe: bool = False,
     thickness: float = 0.0,
     xform=None,
-    real_args: str = "0",
+    real_args: list = [""],
 ) -> Primitive:
     """Create a BSDF primtive."""
     str_args = [xmlpath, str(upvec)]
     str_args_count = 5
     if pe:
         _type = "aBSDF"
     else:
@@ -328,42 +258,17 @@
         str_args = [str(thickness), *str_args]
         _type = "BSDF"
     if xform is not None:
         str_args_count += len(xform.split())
         str_args.extend(*xform.split())
     else:
         str_args.append(".")
-    str_args = [str(str_args_count), *str_args]
     return Primitive(mod, _type, ident, str_args, real_args)
 
 
-def lambda_calc(theta_lr: float, theta_up: float, nphi: float) -> float:
-    """."""
-    return (
-        (
-            math.cos(math.pi / 180 * theta_lr) ** 2
-            - math.cos(math.pi / 180 * theta_up) ** 2
-        )
-        * math.pi
-        / nphi
-    )
-
-
-def angle_basis_coeff(basis: str) -> List[float]:
-    """Calculate klems basis coefficient"""
-    ablist = ABASE_LIST[basis]
-    lambdas = []
-    for i in range(len(ablist) - 1):
-        tu = ablist[i + 1][0]
-        tl = ablist[i][0]
-        np = ablist[i][1]
-        lambdas.extend([lambda_calc(tl, tu, np) for _ in range(np)])
-    return lambdas
-
-
 def opt2list(opt: dict) -> List[str]:
     """Convert option dictionary to list.
 
     Key: str
     Value: str | float | int | bool | list
 
     Args:
@@ -515,15 +420,15 @@
     # _grid = [p for p in raw_pts if pt_incls.test_inside(p) > 0]
     grid = [p.to_list() + grid_dir.to_list() for p in _grid]
     return grid
 
 
 def material_lib() -> Dict[str, Any]:
     """Generate a list of generic material primitives."""
-    tmis = tmit2tmis(0.6)
+    tmis = 0.6 * 1.08981
     return {
         "neutral_lambertian_0.2": neutral_plastic_prim(
             "void", "neutral_lambertian_0.2", 0.2, 0, 0
         ),
         "neutral_lambertian_0.5": neutral_plastic_prim(
             "void", "neutral_lambertian_0.5", 0.5, 0, 0
         ),
@@ -547,29 +452,27 @@
 def get_glazing_primitive(panes: List[PaneRGB]) -> Primitive:
     """Generate a BRTDfunc to represent a glazing system."""
     if len(panes) > 2:
         raise ValueError("Only double pane supported")
     name = "+".join([pane.measured_data.name for pane in panes])
     if len(panes) == 1:
         str_arg = [
-            "10",
             "sr_clear_r",
             "sr_clear_g",
             "sr_clear_b",
             "st_clear_r",
             "st_clear_g",
             "st_clear_b",
             "0",
             "0",
             "0",
             "glaze1.cal",
         ]
         coated_real = 1 if panes[0].measured_data.coated_side == "front" else -1
         real_arg = [
-            19,
             0,
             0,
             0,
             0,
             0,
             0,
             0,
@@ -592,15 +495,14 @@
         if panes[1].measured_data.coated_side == "back":
             s4r_r, s4r_g, s4r_b = panes[1].coated_rgb
             s3r_r, s3r_g, s3r_b = panes[1].glass_rgb
         else:  # front or neither side coated
             s4r_r, s4r_g, s4r_b = panes[1].glass_rgb
             s3r_r, s3r_g, s3r_b = panes[1].coated_rgb
         str_arg = [
-            "10",
             (
                 f"if(Rdot,cr(fr({s4r_r:.3f}),ft({s34t_r:.3f}),fr({s2r_r:.3f})),"
                 f"cr(fr({s1r_r:.3f}),ft({s12t_r:.3f}),fr({s3r_r:.3f})))"
             ),
             (
                 f"if(Rdot,cr(fr({s4r_g:.3f}),ft({s34t_g:.3f}),fr({s2r_g:.3f})),"
                 f"cr(fr({s1r_g:.3f}),ft({s12t_g:.3f}),fr({s3r_g:.3f})))"
@@ -613,49 +515,18 @@
             f"ft({s34t_g:.3f})*ft({s12t_g:.3f})",
             f"ft({s34t_b:.3f})*ft({s12t_b:.3f})",
             "0",
             "0",
             "0",
             "glaze2.cal",
         ]
-        real_arg = [9, 0, 0, 0, 0, 0, 0, 0, 0, 0]
+        real_arg = [0, 0, 0, 0, 0, 0, 0, 0, 0]
     return Primitive("void", "BRTDfunc", name, str_arg, real_arg)
 
 
-def get_flush_corner_rays_command(ray_cnt: int, xres: int) -> list:
-    """Flush the corner rays from a fisheye view.
-
-    Args:
-        ray_cnt: ray count;
-        xres: resolution of the square image;
-
-    Returns:
-        Command to generate cropped rays
-
-    """
-    cmd = [
-        "rcalc",
-        "-if6",
-        "-of",
-        "-e",
-        f"DIM:{xres};CNT:{ray_cnt}",
-        "-e",
-        "pn=(recno-1)/CNT+.5",
-        "-e",
-        "frac(x):x-floor(x)",
-        "-e",
-        "xpos=frac(pn/DIM);ypos=pn/(DIM*DIM)",
-        "-e",
-        "incir=if(.25-(xpos-.5)*(xpos-.5)-(ypos-.5)*(ypos-.5),1,0)",
-        "-e",
-        "$1=$1;$2=$2;$3=$3;$4=$4*incir;$5=$5*incir;$6=$6*incir",
-    ]
-    return cmd
-
-
 def batch_process(
     commands: List[List[str]],
     inputs: Optional[List[bytes]] = None,
     opaths: Optional[List[Path]] = None,
     nproc: Optional[int] = None,
 ) -> None:
     """Run commands in batches.
@@ -698,13 +569,7 @@
         for igrp, cgrp in zip(stdin_groups, command_groups):
             processes = [sp.Popen(command, stdin=sp.PIPE) for command in cgrp]
             for proc, sin in zip(processes, igrp):
                 if (proc.stdin is not None) and (sin is not None):
                     proc.stdin.write(sin)
             for proc in processes:
                 proc.wait()
-
-
-def run_write(command, out, stdin=None) -> None:
-    """Run command and write stdout to file."""
-    with open(out, "wb") as wtr:
-        sp.run(command, check=True, input=stdin, stdout=wtr)
```

### Comparing `frads-0.2.8/frads.egg-info/PKG-INFO` & `frads-0.3.0/frads.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: frads
-Version: 0.2.8
-Summary: Wrapper for Radiance simulation control
+Version: 0.3.0
+Summary: Wrapper for Radiance related simulation workflows
 License: BSD 3-Clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 
 ![Install + Test](https://github.com/LBNL-ETA/frads/actions/workflows/main.yml/badge.svg)
-![CodeQL](https://github.com/LBNL-ETA/frads/actions/workflows/codeql-analysis.yml/badge.svg)
 [![Upload Python Package](https://github.com/LBNL-ETA/frads/actions/workflows/python-publish.yml/badge.svg)](https://github.com/LBNL-ETA/frads/actions/workflows/python-publish.yml)
+![Downloads](https://img.shields.io/pypi/dm/frads.svg)
 # _frads_: Framework for Radiance simulation control
 
 This is the repository for _frads_ development. Radiance is a free and open-source, raytracing-based lighting engine that is used extensively by engineering firms for innovative solar control, lighting, and daylighting design to improve the energy efficiency of buildings. With matrix algebraic methods, climate-based annual simulations can now be conducted in less than two minutes. _frads_ automates setup of these simulations by providing end users with an open-source, high-level abstraction of the Radiance command-line workflow (Unix toolbox model), helping to reduce the steep learning curve and associated user errors. _frads_ also provides the necessary infrastructure needed for seamless integration of Radiance and other modeling tools, such as EnergyPlus.
 
 [Documentation](https://lbnl-eta.github.io/frads/)
 
 ## Contact/ Support
@@ -43,29 +43,14 @@
 
 	$ python
 	Python 3.X.X
 	[GCC 4.x] on linux
 	Type "help", "copyright", "credits" or "license" for more information.
 	>>>
 
-### Install Radiance
-
-If you haven't already, you will need to install Radiance. `frads` will check your Radiance
-installation, so make sure you install it first.
-
-To install Radiance, visit Radiance Github [repo](https://github.com/LBNL-ETA/Radiance/releases)
- to download the latest release for your operating system.
-
-You can verify that Radiance is installed properly by typing in the command-line:
-
-```
-$ rtrace -version
-RADIANCE 5.4a ...
-```
-
 ### Install frads
 
 After you have Python installed, you should have `pip` command available in your shell environment as well. You can then use `pip` to install `frads`:
 
 	$ python -m pip install frads
 
 Alternatively, more recent version of `frads` can be installed directly from github as well. Watch for the passing/failed tag on github to check if the current version passed the tests.:
```

### Comparing `frads-0.2.8/frads.egg-info/SOURCES.txt` & `frads-0.3.0/frads.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 MANIFEST.in
 README.md
+license.txt
 pyproject.toml
 setup.cfg
 frads/__init__.py
 frads/cli.py
 frads/color.py
 frads/color_data.py
 frads/epjson2rad.py
-frads/gencolorsky.py
+frads/eprad.py
 frads/geom.py
 frads/matrix.py
 frads/methods.py
 frads/mtxmult.py
 frads/ncp.py
 frads/parsers.py
-frads/raycall.py
 frads/room.py
 frads/sky.py
 frads/types.py
 frads/utils.py
+frads/window.py
 frads.egg-info/PKG-INFO
 frads.egg-info/SOURCES.txt
 frads.egg-info/dependency_links.txt
 frads.egg-info/entry_points.txt
 frads.egg-info/not-zip-safe
+frads.egg-info/requires.txt
 frads.egg-info/top_level.txt
 frads/data/WC.DAT
 frads/data/mrad_default.cfg
 test/test_color.py
 test/test_epjson2rad.py
 test/test_geom.py
 test/test_matrix.py
 test/test_methods.py
 test/test_mtxmult.py
 test/test_ncp.py
 test/test_parsers.py
-test/test_raycall.py
 test/test_sky.py
 test/test_utils.py
+test/test_window.py
 test/Resources/USA_CA_Oakland.Intl.AP.724930_TMY3.epw
 test/Resources/blinds30.xml
 test/Resources/klems_aniso_high.xml
 test/Resources/oak.wea
 test/Resources/test.wea
```

### Comparing `frads-0.2.8/setup.cfg` & `frads-0.3.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -12,20 +12,16 @@
 [options]
 zip_safe = False
 include_package_data = True
 packages = frads
 
 [options.entry_points]
 console_scripts = 
-	ep2rad = frads.cli:epjson2rad_cmd
-	gencolorsky = frads.gencolorsky:main
 	gen = frads.cli:gen
 	mrad = frads.cli:mrad
-	rpxop = frads.cli:rpxop
-	varays = frads.cli:varays
 
 [flake8]
 max-line-length = 88
 extend-ignore = E203
 
 [egg_info]
 tag_build =
```

### Comparing `frads-0.2.8/test/Resources/USA_CA_Oakland.Intl.AP.724930_TMY3.epw` & `frads-0.3.0/test/Resources/USA_CA_Oakland.Intl.AP.724930_TMY3.epw`

 * *Files identical despite different names*

### Comparing `frads-0.2.8/test/Resources/blinds30.xml` & `frads-0.3.0/test/Resources/blinds30.xml`

 * *Files identical despite different names*

### Comparing `frads-0.2.8/test/Resources/klems_aniso_high.xml` & `frads-0.3.0/test/Resources/klems_aniso_high.xml`

 * *Files identical despite different names*

### Comparing `frads-0.2.8/test/Resources/oak.wea` & `frads-0.3.0/test/Resources/oak.wea`

 * *Files identical despite different names*

### Comparing `frads-0.2.8/test/test_color.py` & `frads-0.3.0/test/test_color.py`

 * *Files identical despite different names*

### Comparing `frads-0.2.8/test/test_epjson2rad.py` & `frads-0.3.0/test/test_epjson2rad.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,42 @@
+import json
 from pathlib import Path
 import os
 import glob
 import sys
 sys.path.append(".")
 from frads import epjson2rad
 
 
 
 test_dir = Path(__file__).resolve().parent
 
 
 def test_cfscase():
+    os.chdir("test")
     epjson1 = test_dir / "Resources" / "CmplxGlz_SingleZone_DoubleClearAir.epJSON"
-    epjson2rad.epjson2rad(epjson2rad.read_ep_input(epjson1))
-    assert os.path.isfile("Room_102.cfg")
+    with open(epjson1) as fp:
+        json_data = json.load(fp)
+    epjson2rad(json_data, epw="")
+    assert os.path.isfile("Room 102.cfg")
     assert os.path.isfile("./Objects/Room102_South_Wall.rad")
     assert os.path.isfile("./Objects/Room102_South_Wall_window.rad")
     assert os.path.isfile("./Objects/Room102_Ceiling.rad")
-    os.remove("Room_102.cfg")
+    os.remove("Room 102.cfg")
     obj_files = glob.glob("./Objects/Room_102*.rad")
     for file in obj_files:
         os.remove(file)
+    os.chdir("..")
 
 def test_refcase():
+    os.chdir("test")
     epjson2 = test_dir / "Resources" / "RefBldgMediumOfficeNew2004_Chicago.epJSON"
-    epjson2rad.epjson2rad(epjson2rad.read_ep_input(epjson2))
+    with open(epjson2) as fp:
+        json_data = json.load(fp)
+    epjson2rad(json_data, epw="")
     assert os.path.isfile("./Objects/Perimeter_bot_ZN_1_Wall_South.rad")
     assert os.path.isfile("./Objects/Perimeter_mid_ZN_3_Ceiling.rad")
     assert os.path.isfile("Perimeter_bot_ZN_1.cfg")
     assert os.path.isfile("Perimeter_bot_ZN_2.cfg")
     assert os.path.isfile("Perimeter_bot_ZN_3.cfg")
     assert os.path.isfile("Perimeter_bot_ZN_4.cfg")
     assert os.path.isfile("Perimeter_mid_ZN_1.cfg")
@@ -41,7 +49,12 @@
     assert os.path.isfile("Perimeter_top_ZN_4.cfg")
     cfg_files = glob.glob("./Perimeter*.cfg")
     obj_files = glob.glob("./Objects/Perimeter*.rad")
     for file in obj_files:
         os.remove(file)
     for file in cfg_files:
         os.remove(file)
+    os.chdir("..")
+
+if __name__ == "__main__":
+    test_cfscase()
+    test_refcase()
```

### Comparing `frads-0.2.8/test/test_geom.py` & `frads-0.3.0/test/test_geom.py`

 * *Files identical despite different names*

### Comparing `frads-0.2.8/test/test_matrix.py` & `frads-0.3.0/test/test_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 import sys
 sys.path.append(".")
 
 from frads import geom
 from frads import matrix
-from frads.types import Primitive
+import pyradiance as pr
 from frads.types import View
 from frads.types import ViewType
 
 window_polygon = [
     geom.Polygon([geom.Vector(0, 0, 0),
                   geom.Vector(0, 0, 3),
                   geom.Vector(2, 0, 3),
@@ -17,16 +17,16 @@
     geom.Polygon([geom.Vector(3, 0, 0),
                   geom.Vector(3, 0, 3),
                   geom.Vector(5, 0, 3),
                   geom.Vector(5, 0, 0),
                   ])
 ]
 window_primitives = [
-    Primitive("void", "polygon", "window1", ("0"), window_polygon[0].to_real()),
-    Primitive("void", "polygon", "window2", ("0"), window_polygon[1].to_real())
+    pr.Primitive("void", "polygon", "window1", ("0"), window_polygon[0].to_real()),
+    pr.Primitive("void", "polygon", "window2", ("0"), window_polygon[1].to_real())
 ]
 
 def test_surface_as_sender():
     basis = "kf"
     sender = matrix.surface_as_sender(
         window_primitives, basis, offset=None, left=None)
     assert sender.form == "s"
```

### Comparing `frads-0.2.8/test/test_mtxmult.py` & `frads-0.3.0/test/test_mtxmult.py`

 * *Files identical despite different names*

### Comparing `frads-0.2.8/test/test_ncp.py` & `frads-0.3.0/test/test_ncp.py`

 * *Files identical despite different names*

### Comparing `frads-0.2.8/test/test_parsers.py` & `frads-0.3.0/test/test_parsers.py`

 * *Files identical despite different names*

### Comparing `frads-0.2.8/test/test_sky.py` & `frads-0.3.0/test/test_sky.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from datetime import datetime
 from pathlib import Path
 import sys
 sys.path.append(".")
 
 from frads import geom
+import pyradiance as pr
 from frads import parsers
 from frads import sky
 from frads import utils
-from frads.types import WeaData
-from frads.types import WeaMetaData
+from frads.sky import WeaData
+from frads.sky import WeaMetaData
 import logging
 
 logger = logging.getLogger()
 logger.setLevel(50)
 
 
 test_dir = Path(__file__).resolve().parent
@@ -36,15 +37,15 @@
 
 
 def test_gen_sun_source_full():
     """Generate sun sources for matrix generation."""
     reinsrc4_path = test_dir / "Resources" / "reinsrc4.rad"
     mf = 4
     prim_str, mod_str = sky.gen_sun_source_full(mf)
-    prims = parsers.parse_primitive(prim_str.splitlines())
+    prims = pr.parse_primitive(prim_str)
     answer_prims = utils.unpack_primitives(reinsrc4_path)
     for aprim, prim in zip(prims, answer_prims):
         assert str(aprim) == str(prim)
 
 def test_gendaymtx():
     """Generate a psuedo reinhart 6 sun matrix file given lat, lon, etc..."""
     # sky.gendaymtx(
```

### Comparing `frads-0.2.8/test/test_utils.py` & `frads-0.3.0/test/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 sys.path.append(".")
 
 from frads import geom
 from frads import utils
 from frads.types import PaneProperty
 from frads.types import PaneRGB
-from frads.types import Primitive
+from pyradiance import Primitive
 
 
 test_dir_path = Path(os.path.dirname(__file__))
 resource_dir = test_dir_path / "Resources"
 check_decimal_to = 6
 reinsrc6_path = resource_dir / "reinsrc6.rad"
 grid_path = resource_dir / "grid.pts"
```

