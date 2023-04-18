# Comparing `tmp/pysolid-0.2.3.tar.gz` & `tmp/pysolid-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysolid-0.2.3.tar", last modified: Mon Oct 24 05:59:03 2022, max compression
+gzip compressed data, was "pysolid-0.3.0.tar", last modified: Tue Apr 18 14:35:51 2023, max compression
```

## Comparing `pysolid-0.2.3.tar` & `pysolid-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 05:59:03.272215 pysolid-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-24 05:57:25.000000 pysolid-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8248 2022-10-24 05:59:03.272215 pysolid-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7324 2022-10-24 05:57:25.000000 pysolid-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-24 05:59:03.272215 pysolid-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-10-24 05:57:25.000000 pysolid-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 05:59:03.272215 pysolid-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 05:59:03.272215 pysolid-0.2.3/src/pysolid/
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-10-24 05:57:25.000000 pysolid-0.2.3/src/pysolid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6689 2022-10-24 05:57:25.000000 pysolid-0.2.3/src/pysolid/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)    14019 2022-10-24 05:57:25.000000 pysolid-0.2.3/src/pysolid/point.py
--rw-r--r--   0 runner    (1001) docker     (121)    56224 2022-10-24 05:57:25.000000 pysolid-0.2.3/src/pysolid/solid.for
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-10-24 05:57:25.000000 pysolid-0.2.3/src/pysolid/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 05:59:03.272215 pysolid-0.2.3/src/pysolid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8248 2022-10-24 05:59:03.000000 pysolid-0.2.3/src/pysolid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-10-24 05:59:03.000000 pysolid-0.2.3/src/pysolid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 05:59:03.000000 pysolid-0.2.3/src/pysolid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-10-24 05:59:03.000000 pysolid-0.2.3/src/pysolid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-24 05:59:03.000000 pysolid-0.2.3/src/pysolid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:35:51.213416 pysolid-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:35:51.213416 pysolid-0.3.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-18 14:35:36.000000 pysolid-0.3.0/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:35:51.213416 pysolid-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-18 14:35:36.000000 pysolid-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:35:51.213416 pysolid-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-18 14:35:36.000000 pysolid-0.3.0/.github/workflows/build-and-publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-18 14:35:36.000000 pysolid-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 14:35:36.000000 pysolid-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-04-18 14:35:51.213416 pysolid-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-04-18 14:35:36.000000 pysolid-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:35:51.213416 pysolid-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   495964 2023-04-18 14:35:36.000000 pysolid-0.3.0/docs/logo.pptx
+-rw-r--r--   0 runner    (1001) docker     (123)   159418 2023-04-18 14:35:36.000000 pysolid-0.3.0/docs/plot_grid_SET.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   144624 2023-04-18 14:35:36.000000 pysolid-0.3.0/docs/plot_point_SET.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-18 14:35:36.000000 pysolid-0.3.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-18 14:35:36.000000 pysolid-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-18 14:35:36.000000 pysolid-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:35:51.213416 pysolid-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-18 14:35:36.000000 pysolid-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:35:51.213416 pysolid-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:35:51.213416 pysolid-0.3.0/src/pysolid/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-18 14:35:36.000000 pysolid-0.3.0/src/pysolid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-04-18 14:35:36.000000 pysolid-0.3.0/src/pysolid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-04-18 14:35:36.000000 pysolid-0.3.0/src/pysolid/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56952 2023-04-18 14:35:36.000000 pysolid-0.3.0/src/pysolid/solid.for
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:35:51.213416 pysolid-0.3.0/src/pysolid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-04-18 14:35:51.000000 pysolid-0.3.0/src/pysolid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-18 14:35:51.000000 pysolid-0.3.0/src/pysolid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:35:51.000000 pysolid-0.3.0/src/pysolid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-18 14:35:51.000000 pysolid-0.3.0/src/pysolid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 14:35:51.000000 pysolid-0.3.0/src/pysolid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:35:51.213416 pysolid-0.3.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1333 2023-04-18 14:35:36.000000 pysolid-0.3.0/tests/grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1294 2023-04-18 14:35:36.000000 pysolid-0.3.0/tests/point.py
```

### Comparing `pysolid-0.2.3/LICENSE` & `pysolid-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysolid-0.2.3/PKG-INFO` & `pysolid-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: pysolid
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Python wrapper for solid to compute solid Earth tides
 Home-page: https://github.com/insarlab/PySolid
-Download-URL: https://github.com/insarlab/PySolid/archive/v0.2.3.tar.gz
 Author: Zhang Yunjun, Dennis Milbert
 Author-email: yunjunzgeo@gmail.com
 License: GPL-3.0-or-later
 Project-URL: Bug Reports, https://github.com/insarlab/PySolid/issues
 Project-URL: Source, https://github.com/insarlab/PySolid
 Keywords: solid Eartth tides,deformation,geodesy,geophysics
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Language](https://img.shields.io/badge/python-3.6%2B-blue.svg)](https://www.python.org/)
-[![CircleCI](https://img.shields.io/circleci/build/github/insarlab/PySolid.svg?logo=circleci&label=test)](https://circleci.com/gh/insarlab/PySolid)
-[![Version](https://img.shields.io/github/v/release/insarlab/PySolid?color=green)](https://github.com/insarlab/PySolid/releases)
-[![License](https://img.shields.io/badge/license-GPLv3+-yellow.svg)](https://github.com/insarlab/PySolid/blob/main/LICENSE)
-[![Citation](https://img.shields.io/badge/doi-10.1109%2FTGRS.2022.3168509-blue)](https://doi.org/10.1109/TGRS.2022.3168509)
+[![Language](https://img.shields.io/badge/python-3.8%2B-blue.svg?style=flat-square)](https://www.python.org/)
+[![CircleCI](https://img.shields.io/circleci/build/github/insarlab/PySolid.svg?logo=circleci&label=test&style=flat-square)](https://circleci.com/gh/insarlab/PySolid)
+[![Version](https://img.shields.io/github/v/release/insarlab/PySolid?color=brightgreen&label=version&style=flat-square)](https://github.com/insarlab/PySolid/releases)
+[![Conda Download](https://img.shields.io/conda/dn/conda-forge/pysolid?color=green&style=flat-square)](https://anaconda.org/conda-forge/pysolid)
+[![License](https://img.shields.io/badge/license-GPLv3+-yellow.svg?style=flat-square)](https://github.com/insarlab/PySolid/blob/main/LICENSE)
+[![Citation](https://img.shields.io/badge/doi-10.1109%2FTGRS.2022.3168509-blue?style=flat-square)](https://doi.org/10.1109/TGRS.2022.3168509)
 
 ## PySolid
 
-The Python based solid Earth tides (PySolid) is a thin Python wrapper of the [`solid.for`](http://geodesyworld.github.io/SOFTS/solid.htm) program (by Dennis Milbert based on [_dehanttideinelMJD.f_](https://iers-conventions.obspm.fr/content/chapter7/software/dehanttideinel/) from V. Dehant, S. Mathews, J. Gipson and C. Bruyninx) to calculate [solid Earth tides](https://en.wikipedia.org/wiki/Earth_tide) in east/north/up direction (section 7.1.1 in the [2010 IERS Conventions](https://www.iers.org/IERS/EN/Publications/TechnicalNotes/tn36.html)). Solid Earth tides introduces very long spatial wavelength components in SAR/InSAR observations, as shown in the Sentinel-1 data with regular acquisitions and large swaths (Yunjun et al., 2022).
+The Python based solid Earth tides (PySolid) is a thin Python wrapper of the [`solid.for`](http://geodesyworld.github.io/SOFTS/solid.htm) program (by Dennis Milbert based on [_dehanttideinelMJD.f_](https://iers-conventions.obspm.fr/content/chapter7/software/dehanttideinel/) from V. Dehant, S. Mathews, J. Gipson and C. Bruyninx) to calculate [solid Earth tides](https://en.wikipedia.org/wiki/Earth_tide) in east, north and up directions (section 7.1.1 in the [2010 IERS Conventions](https://www.iers.org/IERS/EN/Publications/TechnicalNotes/tn36.html)). Solid Earth tides introduce large offsets in SAR observations and long spatial wavelength ramps in InSAR observations, as shown in the Sentinel-1 data with regular acquisitions and large swaths ([Yunjun et al., 2022](https://doi.org/10.1109/TGRS.2022.3168509)).
 
 This is research code provided to you "as is" with NO WARRANTIES OF CORRECTNESS. Use at your own risk.
 
 ### 1. Install
 
 PySolid is available on the [conda-forge](https://anaconda.org/conda-forge/pysolid) channel and the main archive of the [Debian](https://tracker.debian.org/pkg/pysolid) GNU/Linux OS. The released version can be install via `conda` as:
 
@@ -43,17 +44,16 @@
 
 or via `apt` (or other package managers) for [Debian-derivative OS](https://wiki.debian.org/Derivatives/Census) users, including [Ubuntu](https://ubuntu.com), as:
 
 ```shell
 apt install python3-pysolid
 ```
 
-Installing via `conda` and `apt` is recomended because PySolid contains Fortran source code, which required compilcation. Otherwise, you may build it from source as described below.
-
-#### 1.1 Build from source
+<details>
+<p><summary>Or build from source:</summary></p>
 
 PySolid relies on a few Python modules as described in [requirements.txt](./requirements.txt) and [NumPy's f2py](https://numpy.org/doc/stable/f2py/) to build the Fortran source code. You could use `conda` to install all the dependencies, including the Fortran compiler, or use your own installed Fortran compiler and `pip` to install the rest.
 
 ##### a. Download source code
 
 ```bash
 # run "cd PySolid; git pull" to update to the latest development version
@@ -74,36 +74,41 @@
 python -m pip install -r PySolid/requirements.txt
 ```
 
 ##### c. Install PySolid
 
 ```bash
 # option 1: use pip to install pysolid into the current environment
-# use "pip install -e" to install in the development mode
 python -m pip install PySolid
 
-# option 2: manually compile the Fortran code and setup environment variable
+# option 2: use pip to install pysolid in develop mode (editable) into the current environment
+# setting an environmental variable as below is required for editable installs via pyproject.toml
+export SETUPTOOLS_ENABLE_FEATURES="legacy-editable"
+python -m pip install -e PySolid
+
+# option 3: manually compile the Fortran code and setup environment variable
 cd PySolid/src/pysolid
 f2py -c -m solid solid.for
 export PYTHONPATH=${PYTHONPATH}:~/tools/PySolid
 ```
 
-#### 1.2 Test the installation
+##### d. Test the installation
 
 To test the installation, run the following:
 
 ```bash
 python -c "import pysolid; print(pysolid.__version__)"
 python PySolid/tests/grid.py
 python PySolid/tests/point.py
 ```
+</details>
 
 ### 2. Usage
 
-PySolid could compute solid Earth tides in two modes: **point** and **grid**. Both modes produce displacement in east, north and up direction.
+PySolid could compute solid Earth tides in two modes: **point** and **grid**. Both modes produce displacement in east, north and up directions.
 
 +   **Point mode:** compute 1D tides time-series at a specific point for a given time period
 +   **Grid mode:** compute 2D tides grid at a specific time for a given spatial grid
 
 #### 2.1 Point Mode [[notebook](./docs/plot_point_SET.ipynb)]
 
 ```python
@@ -154,15 +159,15 @@
 # compute SET via pysolid
 tide_e, tide_n, tide_u = pysolid.calc_solid_earth_tides_grid(
     dt_obj, meta,
     display=False,
     verbose=True,
 )
 
-# project SET from ENU to radar line-of-sight (LOS) direction with positive for motion towards satellite
+# project SET from ENU to satellite line-of-sight (LOS) direction with positive for motion towards the satellite
 # inc_angle : incidence angle of the LOS vector (from ground to radar platform) measured from vertical.
 # az_angle  : azimuth   angle of the LOS vector (from ground to radar platform) measured from the north, with anti-clockwirse as positive.
 inc_angle = np.deg2rad(34)   # radian, typical value for Sentinel-1
 az_angle = np.deg2rad(-102)  # radian, typical value for Sentinel-1 descending track
 tide_los = (  tide_e * np.sin(inc_angle) * np.sin(az_angle) * -1
             + tide_n * np.sin(inc_angle) * np.cos(az_angle)
             + tide_u * np.cos(inc_angle))
@@ -172,7 +177,9 @@
   <img width="800" src="https://yunjunzhang.files.wordpress.com/2021/01/set_grid-3.png">
 </p>
 
 ### 3. Citing this work
 
 +   Yunjun, Z., Fattahi, H., Pi, X., Rosen, P., Simons, M., Agram, P., & Aoki, Y. (2022). Range Geolocation Accuracy of C-/L-band SAR and its Implications for Operational Stack Coregistration. _IEEE Trans. Geosci. Remote Sens., 60_, 1-19, doi:[10.1109/TGRS.2022.3168509](https://doi.org/10.1109/TGRS.2022.3168509), [arXiv](https://doi.org/10.31223/X5F641), [data](https://zenodo.org/record/6360749), [notebooks](https://github.com/yunjunz/2022-Geolocation).
 +   Milbert, D. (2018), "solid: Solid Earth Tide", [Online]. Available: http://geodesyworld.github.io/SOFTS/solid.htm. Accessd on: 2020-09-06.
+
+
```

### Comparing `pysolid-0.2.3/README.md` & `pysolid-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-[![Language](https://img.shields.io/badge/python-3.6%2B-blue.svg)](https://www.python.org/)
-[![CircleCI](https://img.shields.io/circleci/build/github/insarlab/PySolid.svg?logo=circleci&label=test)](https://circleci.com/gh/insarlab/PySolid)
-[![Version](https://img.shields.io/github/v/release/insarlab/PySolid?color=green)](https://github.com/insarlab/PySolid/releases)
-[![License](https://img.shields.io/badge/license-GPLv3+-yellow.svg)](https://github.com/insarlab/PySolid/blob/main/LICENSE)
-[![Citation](https://img.shields.io/badge/doi-10.1109%2FTGRS.2022.3168509-blue)](https://doi.org/10.1109/TGRS.2022.3168509)
+[![Language](https://img.shields.io/badge/python-3.8%2B-blue.svg?style=flat-square)](https://www.python.org/)
+[![CircleCI](https://img.shields.io/circleci/build/github/insarlab/PySolid.svg?logo=circleci&label=test&style=flat-square)](https://circleci.com/gh/insarlab/PySolid)
+[![Version](https://img.shields.io/github/v/release/insarlab/PySolid?color=brightgreen&label=version&style=flat-square)](https://github.com/insarlab/PySolid/releases)
+[![Conda Download](https://img.shields.io/conda/dn/conda-forge/pysolid?color=green&style=flat-square)](https://anaconda.org/conda-forge/pysolid)
+[![License](https://img.shields.io/badge/license-GPLv3+-yellow.svg?style=flat-square)](https://github.com/insarlab/PySolid/blob/main/LICENSE)
+[![Citation](https://img.shields.io/badge/doi-10.1109%2FTGRS.2022.3168509-blue?style=flat-square)](https://doi.org/10.1109/TGRS.2022.3168509)
 
 ## PySolid
 
-The Python based solid Earth tides (PySolid) is a thin Python wrapper of the [`solid.for`](http://geodesyworld.github.io/SOFTS/solid.htm) program (by Dennis Milbert based on [_dehanttideinelMJD.f_](https://iers-conventions.obspm.fr/content/chapter7/software/dehanttideinel/) from V. Dehant, S. Mathews, J. Gipson and C. Bruyninx) to calculate [solid Earth tides](https://en.wikipedia.org/wiki/Earth_tide) in east/north/up direction (section 7.1.1 in the [2010 IERS Conventions](https://www.iers.org/IERS/EN/Publications/TechnicalNotes/tn36.html)). Solid Earth tides introduces very long spatial wavelength components in SAR/InSAR observations, as shown in the Sentinel-1 data with regular acquisitions and large swaths (Yunjun et al., 2022).
+The Python based solid Earth tides (PySolid) is a thin Python wrapper of the [`solid.for`](http://geodesyworld.github.io/SOFTS/solid.htm) program (by Dennis Milbert based on [_dehanttideinelMJD.f_](https://iers-conventions.obspm.fr/content/chapter7/software/dehanttideinel/) from V. Dehant, S. Mathews, J. Gipson and C. Bruyninx) to calculate [solid Earth tides](https://en.wikipedia.org/wiki/Earth_tide) in east, north and up directions (section 7.1.1 in the [2010 IERS Conventions](https://www.iers.org/IERS/EN/Publications/TechnicalNotes/tn36.html)). Solid Earth tides introduce large offsets in SAR observations and long spatial wavelength ramps in InSAR observations, as shown in the Sentinel-1 data with regular acquisitions and large swaths ([Yunjun et al., 2022](https://doi.org/10.1109/TGRS.2022.3168509)).
 
 This is research code provided to you "as is" with NO WARRANTIES OF CORRECTNESS. Use at your own risk.
 
 ### 1. Install
 
 PySolid is available on the [conda-forge](https://anaconda.org/conda-forge/pysolid) channel and the main archive of the [Debian](https://tracker.debian.org/pkg/pysolid) GNU/Linux OS. The released version can be install via `conda` as:
 
@@ -21,17 +22,16 @@
 
 or via `apt` (or other package managers) for [Debian-derivative OS](https://wiki.debian.org/Derivatives/Census) users, including [Ubuntu](https://ubuntu.com), as:
 
 ```shell
 apt install python3-pysolid
 ```
 
-Installing via `conda` and `apt` is recomended because PySolid contains Fortran source code, which required compilcation. Otherwise, you may build it from source as described below.
-
-#### 1.1 Build from source
+<details>
+<p><summary>Or build from source:</summary></p>
 
 PySolid relies on a few Python modules as described in [requirements.txt](./requirements.txt) and [NumPy's f2py](https://numpy.org/doc/stable/f2py/) to build the Fortran source code. You could use `conda` to install all the dependencies, including the Fortran compiler, or use your own installed Fortran compiler and `pip` to install the rest.
 
 ##### a. Download source code
 
 ```bash
 # run "cd PySolid; git pull" to update to the latest development version
@@ -52,36 +52,41 @@
 python -m pip install -r PySolid/requirements.txt
 ```
 
 ##### c. Install PySolid
 
 ```bash
 # option 1: use pip to install pysolid into the current environment
-# use "pip install -e" to install in the development mode
 python -m pip install PySolid
 
-# option 2: manually compile the Fortran code and setup environment variable
+# option 2: use pip to install pysolid in develop mode (editable) into the current environment
+# setting an environmental variable as below is required for editable installs via pyproject.toml
+export SETUPTOOLS_ENABLE_FEATURES="legacy-editable"
+python -m pip install -e PySolid
+
+# option 3: manually compile the Fortran code and setup environment variable
 cd PySolid/src/pysolid
 f2py -c -m solid solid.for
 export PYTHONPATH=${PYTHONPATH}:~/tools/PySolid
 ```
 
-#### 1.2 Test the installation
+##### d. Test the installation
 
 To test the installation, run the following:
 
 ```bash
 python -c "import pysolid; print(pysolid.__version__)"
 python PySolid/tests/grid.py
 python PySolid/tests/point.py
 ```
+</details>
 
 ### 2. Usage
 
-PySolid could compute solid Earth tides in two modes: **point** and **grid**. Both modes produce displacement in east, north and up direction.
+PySolid could compute solid Earth tides in two modes: **point** and **grid**. Both modes produce displacement in east, north and up directions.
 
 +   **Point mode:** compute 1D tides time-series at a specific point for a given time period
 +   **Grid mode:** compute 2D tides grid at a specific time for a given spatial grid
 
 #### 2.1 Point Mode [[notebook](./docs/plot_point_SET.ipynb)]
 
 ```python
@@ -132,15 +137,15 @@
 # compute SET via pysolid
 tide_e, tide_n, tide_u = pysolid.calc_solid_earth_tides_grid(
     dt_obj, meta,
     display=False,
     verbose=True,
 )
 
-# project SET from ENU to radar line-of-sight (LOS) direction with positive for motion towards satellite
+# project SET from ENU to satellite line-of-sight (LOS) direction with positive for motion towards the satellite
 # inc_angle : incidence angle of the LOS vector (from ground to radar platform) measured from vertical.
 # az_angle  : azimuth   angle of the LOS vector (from ground to radar platform) measured from the north, with anti-clockwirse as positive.
 inc_angle = np.deg2rad(34)   # radian, typical value for Sentinel-1
 az_angle = np.deg2rad(-102)  # radian, typical value for Sentinel-1 descending track
 tide_los = (  tide_e * np.sin(inc_angle) * np.sin(az_angle) * -1
             + tide_n * np.sin(inc_angle) * np.cos(az_angle)
             + tide_u * np.cos(inc_angle))
```

### Comparing `pysolid-0.2.3/setup.py` & `pysolid-0.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,25 @@
 # Author: Zhang Yunjun, Jan 2021
 # Copyright 2020, by the California Institute of Technology.
-# Note by Yunjun, Oct 2022: "pip install pysolid" does not work,
-#   because a Fortran compiler is required but not available via pip
-
-
-import os
-import sys
 
 # always prefer setuptools over distutils
 import setuptools
 from numpy.distutils.core import setup, Extension
 
-# Grab from pysolid.version: version
-# link: https://stackoverflow.com/questions/53648900
-sys.path.append(os.path.join(os.path.dirname(__file__), 'src'))
-from pysolid.version import version
-
-# Grab from README file: long_description
-with open("README.md", "r") as f:
-    long_description = f.read()
+# read the contents of README file
+def readme():
+    with open("README.md") as f:
+        return f.read()
 
 setup(
-    name='pysolid',
-    version=version,
+    ## add the following redundant setup for setuptools<60, the latter is required for numpy.distutils
+    name="pysolid",
     description="A Python wrapper for solid to compute solid Earth tides",
     url="https://github.com/insarlab/PySolid",
-    download_url=("https://github.com/insarlab/PySolid/archive/v{}.tar.gz".format(version)),
-    long_description=long_description,
+    long_description=readme(),
     long_description_content_type="text/markdown",
     author="Zhang Yunjun, Dennis Milbert",
     author_email="yunjunzgeo@gmail.com",
     license="GPL-3.0-or-later",
     license_files=("LICENSE",),
 
     classifiers=[
@@ -44,31 +33,31 @@
     keywords="solid Eartth tides, deformation, geodesy, geophysics",
 
     project_urls={
         "Bug Reports": "https://github.com/insarlab/PySolid/issues",
         "Source": "https://github.com/insarlab/PySolid",
     },
 
-    # package discovery
-    packages=setuptools.find_packages("src"),  # include all packages under src
-    package_dir={"": "src"},                   # tell distutils packages are under src
-
-    # build fortran deps with numpy.f2py
-    ext_modules=[
-        Extension(name='pysolid.solid', sources=['src/pysolid/solid.for']),
-    ],
-
     # dependencies
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     install_requires=[
-        'numpy',
-        'scipy',
-        'matplotlib',
-        'scikit-image',
+        "numpy",
+        "scipy",
+        "matplotlib",
+        "scikit-image",
     ],
 
+    # package discovery
+    packages=setuptools.find_packages("src"),  # include all packages under src
+    package_dir={"": "src"},                   # tell distutils packages are under src
+
     # data files
     include_package_data=True,
     package_data={
         "pysolid": ["solid.for"],
     },
+
+    ## fortran extensions to build with numpy.f2py
+    ext_modules=[
+        Extension(name="pysolid.solid", sources=["src/pysolid/solid.for"])
+    ],
 )
```

### Comparing `pysolid-0.2.3/src/pysolid/grid.py` & `pysolid-0.3.0/src/pysolid/grid.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # Copyright 2020, by the California Institute of Technology.
 #######################################################################
 # Recommend usage:
 #   import pysolid
 #   pysolid.calc_solid_earth_tides_grid()
 
 
-import datetime as dt
 import os
 
 import numpy as np
 from skimage.transform import resize
 
 
 ##################################  Earth tides - grid mode  ###################################
@@ -69,43 +68,19 @@
     width  = np.rint(int(atr['WIDTH'])  / num_step - 1e-4).astype(int)
     lat_step = float(atr['Y_STEP']) * num_step
     lon_step = float(atr['X_STEP']) * num_step
     vprint('SOLID  : calculate solid Earth tides in east/north/up direction')
     vprint('SOLID  : shape: {s}, step size: {la:.4f} by {lo:.4f} deg'.format(
         s=(length, width), la=lat_step, lo=lon_step))
 
-    ## calc solid Earth tides and write to text file
-    txt_file = os.path.abspath('solid.txt')
-    if os.path.isfile(txt_file):
-        os.remove(txt_file)
-
-    vprint('SOLID  : calculating / writing data to txt file: {}'.format(txt_file))
-
-    # Run twice to circumvent fortran bug which cuts off last file in loop - Simran, Jun 2020
-    for _ in range(2):
-        solid_grid(dt_obj.year, dt_obj.month, dt_obj.day,
-                   dt_obj.hour, dt_obj.minute, dt_obj.second,
-                   lat0, lat_step, length-1,
-                   lon0, lon_step, width-1)
-
-    ## read data from text file
-    vprint('PYSOLID: read data from text file: {}'.format(txt_file))
-    grid_size = int(length * width)
-    fc = np.loadtxt(txt_file,
-                    dtype=float,
-                    usecols=(2,3,4),
-                    delimiter=',',
-                    skiprows=0,
-                    max_rows=grid_size+100)[:grid_size]
-    tide_e = fc[:, 0].reshape(length, width)
-    tide_n = fc[:, 1].reshape(length, width)
-    tide_u = fc[:, 2].reshape(length, width)
-
-    # remove the temporary text file
-    os.remove(txt_file)
+    ## calc solid Earth tides
+    tide_e, tide_n, tide_u = solid_grid(dt_obj.year, dt_obj.month, dt_obj.day,
+                                        dt_obj.hour, dt_obj.minute, dt_obj.second,
+                                        lat0, lat_step, length,
+                                        lon0, lon_step, width)
 
     # resample to the input size
     if num_step > 1:
         out_shape = (int(atr['LENGTH']), int(atr['WIDTH']))
         vprint('PYSOLID: resize data to the shape of {} using order-1 spline interpolation'.format(out_shape))
         kwargs = dict(order=1, mode='edge', anti_aliasing=True, preserve_range=True)
         tide_e = resize(tide_e, out_shape, **kwargs)
```

### Comparing `pysolid-0.2.3/src/pysolid/point.py` & `pysolid-0.3.0/src/pysolid/point.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,43 +165,23 @@
         from pysolid.solid import solid_point
     except ImportError:
         msg = "Cannot import name 'solid' from 'pysolid'!"
         msg += '\n    Maybe solid.for is NOT compiled yet.'
         msg += '\n    Check instruction at: https://github.com/insarlab/PySolid.'
         raise ImportError(msg)
 
-    ## calc solid Earth tides and write to text file
-    txt_file = os.path.abspath('solid.txt')
-    if os.path.isfile(txt_file):
-        os.remove(txt_file)
-
-    # Run twice to circumvent fortran bug which cuts off last file in loop - Simran, Jun 2020
+    # calc solid Earth tides
     t = dt.datetime.strptime(date_str, '%Y%m%d')
-    for _ in range(2):
-        solid_point(lat, lon, t.year, t.month, t.day, step_sec)
-
-    ## read data from text file
-    num_row = int(24 * 60 * 60 / step_sec)
-    fc = np.loadtxt(txt_file,
-                    dtype=float,
-                    delimiter=',',
-                    skiprows=0,
-                    max_rows=num_row)
+    secs, tide_e, tide_n, tide_u  = solid_point(
+        lat, lon, t.year, t.month, t.day, step_sec
+    )
 
-    tide_e = fc[:, 1].flatten()
-    tide_n = fc[:, 2].flatten()
-    tide_u = fc[:, 3].flatten()
-
-    secs   = fc[:, 0].flatten()
     dt_out = [t + dt.timedelta(seconds=sec) for sec in secs]
     dt_out = np.array(dt_out)
 
-    # remove the temporary text file
-    os.remove(txt_file)
-
     return dt_out, tide_e, tide_n, tide_u
 
 
 #########################################  Plot  ###############################################
 def plot_solid_earth_tides_point(dt_out, tide_e, tide_n, tide_u, lalo=None,
                                  out_fig=None, save=False, display=True):
     """Plot the solid Earth tides at one point."""
```

### Comparing `pysolid-0.2.3/src/pysolid/solid.for` & `pysolid-0.3.0/src/pysolid/solid.for`

 * *Files 4% similar despite different names*

```diff
@@ -3,42 +3,41 @@
 *** Author: Dennis Milbert, 2018-06-01. The code is available at:
 ***     http://geodesyworld.github.io/SOFTS/solid.htm and can be downloaded as:
 ***     wget http://geodesyworld.github.io/SOFTS/solid.for.txt -O solid.for
 *** The code is based on dehanttideinel.f provided by V. Dehant, S. Mathews, 
 ***     J. Gipson and C. Bruyninx. The latest version of dehanttideinel.f and its 
 ***     dependent subroutines can be download from IERS conventions website as:
 ***     wget -r -l1 --no-parent -R "index.html*" -nH --cut-dirs=3 https://iers-conventions.obspm.fr/content/chapter7/software/dehanttideinel
-*** Z. Yunjun and S. Sangha, Sep 2020: modify solid() to solid_point/grid() as subroutines.
+*** Sep 2020: modify solid() to solid_point/grid() as subroutines, Z. Yunjun and S. Sangha.
+*** Apr 2023: return numpy arrays instead of writing txt file, S. Staniewicz.
 
       subroutine solid_grid(iyr,imo,idy,ihh,imm,iss,
-     * glad0,steplat,nlat,
-     * glod0,steplon,nlon)
-
+     * glad0,steplat,nlat,glod0,steplon,nlon,tide_e,tide_n,tide_u)
+ 
 *** calculate solid earth tides (SET) for one spatial grid given the date/time
 *** Arguments: iyr/imo/idy/ihh/imm/iss - int, date/time for YYYY/MM/DD/HH/MM/SS
 ***            glad0/glad1/steplat     - float, north(Y_FIRST)/south/step(negative) in deg
-***            glod0/glod1/steplon     - float, west(X_FIRST) /east /step(positive) in deg
-*** Returns:   latitude,  longitude,  SET_east,  SET_north,  SET_up
+***            glod0/glod1/steplon     - float, west (X_FIRST)/east /step(positive) in deg
+*** Returns:   tide_e/tide_n/tide_u    - 2D np.ndarray, east/north/up component of SET in m
 
       implicit double precision(a-h,o-z)
       dimension rsun(3),rmoon(3),etide(3),xsta(3)
       integer iyr,imo,idy,ihh,imm,iss
       integer nlat,nlon
       double precision glad0,steplat
       double precision glod0,steplon
+      real(8), intent(out), dimension(nlat,nlon) :: tide_e
+      real(8), intent(out), dimension(nlat,nlon) :: tide_n
+      real(8), intent(out), dimension(nlat,nlon) :: tide_u
       !***^ leap second table limit flag
       logical lflag
       common/stuff/rad,pi,pi2
       common/comgrs/a,e2
-
-*** open output file
-
-      lout=1
-      open(lout,file='solid.txt',form='formatted',status='unknown')
-      write(lout,'(a)') '# program solid -- UTC version -- 2018jun01'
+      !f2py intent(in) iyr,imo,idy,ihh,imm,iss,glad0,steplat,nlat,glod0,steplon,nlon
+      !f2py intent(out) tide_e,tide_n,tide_u
 
 *** constants
 
       pi=4.d0*datan(1.d0)
       pi2=pi+pi
       rad=180.d0/pi
 
@@ -46,71 +45,63 @@
 
       a=6378137.d0
       e2=6.69438002290341574957d-03
 
 *** input section
 
       if(iyr.lt.1901.or.iyr.gt.2099) then
-        write(lout,'(a,i5)') 'ERROR: year NOT in [1901-2099]:',iyr
-        go to 98
+        print *, 'ERROR: year NOT in [1901-2099]:',iyr
+        return
       endif
 
       if(imo.lt.1.or.imo.gt.12) then
-        write(lout,'(a,i3)') 'ERROR: month NOT in [1-12]:',imo
-        go to 98
+        print *, 'ERROR: month NOT in [1-12]:',imo
+        return
       endif
 
       if(idy.lt.1.or.idy.gt.31) then
-        write(lout,'(a,i3)') 'ERROR: day NOT in [1-31]:',idy
-        go to 98
+        print *, 'ERROR: day NOT in [1-31]:',idy
+        return
       endif
 
       if(ihh.lt.0.or.ihh.gt.23) then
-        write(lout,'(a,i3)') 'ERROR: hour NOT in [0-23]:',ihh
-        go to 98
+        print *, 'ERROR: hour NOT in [0-23]:',ihh
+        return
       endif
 
       if(imm.lt.0.or.imm.gt.59) then
-        write(lout,'(a,i3)') 'ERROR: minute NOT in [0-59]:',imm
-        go to 98
+        print *, 'ERROR: minute NOT in [0-59]:',imm
+        return
       endif
 
       if(iss.lt.0.or.iss.gt.59) then
-        write(lout,'(a,i3)') 'ERROR: second NOT in [0-59]:',iss
-        go to 98
+        print *, 'ERROR: second NOT in [0-59]:',iss
+        return
       endif
 
       if(glad0.lt.-90.d0.or.glad0.gt.90.d0) then
-        write(lout,'(a,G0.9)') 'ERROR: lat0 NOT in [-90,+90]:',glad0
-        go to 98
+        print *, 'ERROR: lat0 NOT in [-90,+90]:',glad0
+        return
       endif
 
       if(glod0.lt.-360.d0.or.glod0.gt.360.d0) then
-        write(lout,'(a,G0.9)') 'ERROR: lon0 NOT in [-360,+360]',glod0
-        go to 98
+        print *, 'ERROR: lon0 NOT in [-360,+360]',glod0
+        return
       endif
 
-*** output header
-
       glad1=glad0+nlat*steplat
       glod1=glod0+nlon*steplon
 
-      write(lout,'(a,i5,2i3)') '# year, month, day =',iyr,imo,idy
-      write(lout,'(a,3i3)') '# hour, minute, second =',ihh,imm,iss
-      write(lout,'(a,4f15.9)') '# S, N, W, E =',glad1,glad0,glod0,glod1
-      write(lout,'(a,f15.9,i6)') '# step_lat, num_lat =',steplat,nlat
-      write(lout,'(a,f15.9,i6)') '# step_lon, num_lon =',steplon,nlon
-
 *** loop over the grid
 
-      do ilat=0,nlat
-        do ilon=0,nlon
+      do ilat=1,nlat
+        do ilon=1,nlon
 
-        glad=glad0+ilat*steplat
-        glod=glod0+ilon*steplon
+        glad = glad0 + (ilat-1)*steplat
+        glod = glod0 + (ilon-1)*steplon
 
 *** position of observing point (positive East)
 
         if(glod.lt.  0.d0) glod=glod+360.d0
         if(glod.ge.360.d0) glod=glod-360.d0
 
         gla0=glad/rad
@@ -149,59 +140,60 @@
 
         !***^ tide vector
         call rge(gla0,glo0,ut,vt,wt,xt,   yt,   zt)
 
         call mjdciv(mjd,fmjd               +0.001d0/86400.d0,
      *              iyr,imo,idy,ihr,imn,sec-0.001d0)
 
-        !*** write output to file
-        write(lout,'(*(G0.9,:,",  "))') glad,glod,vt,ut,wt
+        !*** write output respective arrays
+        tide_e(ilat, ilon) = vt
+        tide_n(ilat, ilon) = ut
+        tide_u(ilat, ilon) = wt
 
         enddo
       enddo
 
 *** end of processing and flag for leap second
 
       if(lflag) then
-        write(*,'(a)') 'Mild Warning -- time crossed leap second table'
-        write(*,'(a)') '  boundaries.  Boundary edge value used instead'
+        print *, 'Mild Warning -- time crossed leap second table'
+        print *, '  boundaries.  Boundary edge value used instead'
       endif
-      close(lout)
 
-      go to 99
-   98 write(*,'(a)') 'Check arguments.'
 
       return
-   99 end
+      end
 
 *-----------------------------------------------------------------------
-      subroutine solid_point(glad,glod,iyr,imo,idy,step_sec)
+      subroutine solid_point(glad,glod,iyr,imo,idy,step_sec,
+     * secs,tide_e,tide_n,tide_u)
 
 *** calculate SET at given location for one day with step_sec seconds resolution
-*** Arguments: glad/glod   - float, latitude/longitude in deg
-***            iyr/imo/idy - int, start date/time in UTC
-***            step_sec    - int, time step in seconds
-*** Returns:   seconds,  SET_east,  SET_north,  SET_up
+*** Arguments: glad/glod            - float, latitude/longitude in deg
+***            iyr/imo/idy          - int, start date/time in UTC
+***            step_sec             - int, time step in seconds
+*** Returns:   secs                 - 1D np.ndarray, seconds since start
+***            tide_e/tide_n/tide_u - 1D np.ndarray, east/north/up component of SET in m
 
       implicit double precision(a-h,o-z)
       dimension rsun(3),rmoon(3),etide(3),xsta(3)
       double precision glad,glod
       integer iyr,imo,idy
       integer nloop, step_sec
       double precision tdel2
+      real(8), intent(out), dimension(60*60*24/step_sec) :: secs
+      real(8), intent(out), dimension(60*60*24/step_sec) :: tide_e
+      real(8), intent(out), dimension(60*60*24/step_sec) :: tide_n
+      real(8), intent(out), dimension(60*60*24/step_sec) :: tide_u
       !*** leap second table limit flag
       logical lflag
       common/stuff/rad,pi,pi2
       common/comgrs/a,e2
-
-*** open output file
-
-      lout=1
-      open(lout,file='solid.txt',form='formatted',status='unknown')
-      write(lout,'(a)') '# program solid -- UTC version -- 2018jun01'
+      !f2py intent(in) glad,glod,iyr,imo,idy,step_sec
+      !f2py intent(out) secs,tide_e,tide_n,tide_u
 
 *** constants
 
       pi=4.d0*datan(1.d0)
       pi2=pi+pi
       rad=180.d0/pi
 
@@ -209,42 +201,38 @@
 
       a=6378137.d0
       e2=6.69438002290341574957d-03
 
 *** check inputs section
 
       if(glad.lt.-90.d0.or.glad.gt.90.d0) then
-        write(lout,'(a,G0.9)') 'ERROR: lat NOT in [-90,+90]:',glad
-        go to 98
+        print *, 'ERROR: lat NOT in [-90,+90]:',glad
+        return
       endif
 
       if(glod.lt.-360.d0.or.glod.gt.360.d0) then
-        write(lout,'(a,G0.9)') 'ERROR: lon NOT in [-360,+360]:',glod
-        go to 98
+        print *, 'ERROR: lon NOT in [-360,+360]:',glod
+        return
       endif
 
       if(iyr.lt.1901.or.iyr.gt.2099) then
-        write(lout,'(a,i5)') 'ERROR: year NOT in [1901-2099]:',iyr
-        go to 98
+        print *, 'ERROR: year NOT in [1901-2099]:',iyr
+        return
       endif
 
       if(imo.lt.1.or.imo.gt.12) then
-        write(lout,'(a,i3)') 'ERROR: month NOT in [1-12]:',imo
-        go to 98
+        print *, 'ERROR: month NOT in [1-12]:',imo
+        return
       endif
 
       if(idy.lt.1.or.idy.gt.31) then
-        write(lout,'(a,i3)') 'ERROR: day NOT in [1-31]:',idy
-        go to 98
+        print *, 'ERROR: day NOT in [1-31]:',idy
+        return
       endif
 
-*** output header
-
-      write(lout,'(a,i5,2i3)') '# year, month, day =',iyr,imo,idy
-      write(lout,'(a,2f15.9)') '# lat, lon =',glad,glod
 
 *** position of observing point (positive East)
 
       if(glod.lt.  0.d0) glod=glod+360.d0
       if(glod.ge.360.d0) glod=glod-360.d0
 
       gla0=glad/rad
@@ -264,19 +252,17 @@
       call civmjd(iyr,imo,idy,ihr,imn,sec,mjd,fmjd)
       !*** normalize civil time
       call mjdciv(mjd,fmjd,iyr,imo,idy,ihr,imn,sec)
       call setjd0(iyr,imo,idy)
 
 *** loop over time
 
-      !*** tdel2=1.d0/60.d0/24.d0
-      !*** do iloop=0,60*24
       nloop=60*60*24/step_sec
       tdel2=1.d0/DFLOAT(nloop)
-      do iloop=0,nloop
+      do iloop=1,nloop
         !*** false means flag not raised
         !*** mjd/fmjd in UTC
         !*** mjd/fmjd in UTC
         !*** mjd/fmjd in UTC
         lflag=.false.
         call sunxyz (mjd,fmjd,rsun,lflag)
         call moonxyz(mjd,fmjd,rmoon,lflag)
@@ -288,37 +274,36 @@
 *** determine local geodetic horizon components (topocentric)
 
         !*** tide vector
         call rge(gla0,glo0,ut,vt,wt,xt,   yt,   zt)
 
         call mjdciv(mjd,fmjd,iyr,imo,idy,ihr,imn,sec)
 
-        !*** write output to file
         tsec=ihr*3600.d0+imn*60.d0+sec
-        write(lout,'((f8.1,:,",  "),*(f10.6,:,",  "))') tsec,vt,ut,wt
+
+        secs(iloop) = tsec
+        tide_e(iloop) = vt
+        tide_n(iloop) = ut
+        tide_u(iloop) = wt
 
         !*** update fmjd for the next round
         fmjd=fmjd+tdel2
         !*** force 1 sec. granularity
         fmjd=(idnint(fmjd*86400.d0))/86400.d0
       enddo
 
 *** end of processing and flag of leap second
 
       if(lflag) then
-        write(*,'(a)') 'Mild Warning -- time crossed leap second table'
-        write(*,'(a)') '  boundaries.  Boundary edge value used instead'
+        print *, 'Mild Warning -- time crossed leap second table'
+        print *, '  boundaries.  Boundary edge value used instead'
       endif
-      close(lout)
-
-      go to 99
-   98 write(*,'(a)') 'Check arguments.'
 
       return
-   99 end
+      end
 
 *@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
       subroutine detide(xsta,mjd,fmjd,xsun,xmon,dxtide,lflag)
 
 *** computation of tidal corrections of station displacements caused
 ***    by lunar and solar gravitational attraction
 *** UTC version
@@ -357,15 +342,16 @@
 *** modified to use TT time system to call step 2 functions
 *** sign correction by V.Dehant to match eq.16b, p.81, Conventions
 *** applied by Dennis Milbert 2007may05
 *** UTC version by Dennis Milbert 2018june01
 
       implicit double precision(a-h,o-z)
       double precision xsta(3),xsun(3),xmon(3),dxtide(3),xcorsta(3)
-      double precision h20,l20,h3,l3,h2,l2
+      double precision h20,l20,h3,l3,h2,l2,fmjd
+      integer mjd
       double precision mass_ratio_sun,mass_ratio_moon
       logical lflag,leapflag
       !*** leap second table limit flag
       !*** leap second table limit flag
       save  /limitflag/
       common/limitflag/leapflag
 
@@ -529,16 +515,16 @@
 *** this subroutine gives the corrections induced by the latitude dependence
 *** given by l^(1) in mahtews et al (1991)
 
 ***  input: xsta,xsun,xmon,fac3sun,fac3mon
 *** output: xcorsta
 
       implicit double precision (a-h,o-z)
-      dimension xsta(3),xsun(3),xmon(3),xcorsta(3)
-      double precision l1,l1d,l1sd
+      double precision xsta(3),xsun(3),xmon(3),xcorsta(3)
+      double precision l1,l1d,l1sd,fac2sun,fac2mon
       data l1d/0.0012d0/,l1sd/0.0024d0/
 
       rsta=enorm8(xsta)
       sinphi=xsta(3)/rsta
       cosphi=dsqrt(xsta(1)**2+xsta(2)**2)/rsta
       sinla=xsta(2)/cosphi/rsta
       cosla=xsta(1)/cosphi/rsta
@@ -589,15 +575,15 @@
 *** last change:  vd   17 may 00   1:20 pm
 *** these are the subroutines for the step2 of the tidal corrections.
 *** they are called to account for the frequency dependence
 *** of the love numbers.
 
       implicit double precision (a-h,o-z)
       double precision xsta(3),xcorsta(3),datdi(9,31)
-      double precision deg2rad
+      double precision deg2rad, fhr, t
       data deg2rad/0.017453292519943295769d0/
 
 *** note, following table is derived from dehanttideinelMJD.f (2000oct30 16:10)
 *** has minor differences from that of dehanttideinel.f (2000apr17 14:10)
 *** D.M. edited to strictly follow published table 7.5a (2006aug08 13:46)
 
 *** cf. table 7.5a of IERS conventions 2003 (TN.32, pg.82)
@@ -746,15 +732,15 @@
 
       return
       end
 *-----------------------------------------------------------------------
       subroutine step2lon(xsta,fhr,t,xcorsta)
 
       implicit double precision (a-h,o-z)
-      double precision deg2rad
+      double precision deg2rad,fhr,t
       double precision xsta(3),xcorsta(3),datdi(9,5)
       data deg2rad/0.017453292519943295769d0/
 
 *** cf. table 7.5b of IERS conventions 2003 (TN.32, pg.82)
 *** columns are s,h,p,N',ps, dR(ip),dT(ip),dR(op),dT(op)
 *** IERS cols.= s,h,p,N',ps, dR(ip),dR(op),dT(ip),dT(op)
 *** units of mm
@@ -832,15 +818,16 @@
 *** this subroutine gives the out-of-phase corrections induced by
 *** mantle inelasticity in the diurnal band
 
 ***  input: xsta,xsun,xmon,fac2sun,fac2mon
 *** output: xcorsta
 
       implicit double precision (a-h,o-z)
-      dimension xsta(3),xsun(3),xmon(3),xcorsta(3)
+      double precision xsta(3),xsun(3),xmon(3),xcorsta(3)
+      double precision fac2sun,fac2mon
       data dhi/-0.0025d0/,dli/-0.0007d0/
 
       rsta=enorm8(xsta)
       sinphi=xsta(3)/rsta
       cosphi=dsqrt(xsta(1)**2+xsta(2)**2)/rsta
       cos2phi=cosphi**2-sinphi**2
       sinla=xsta(2)/cosphi/rsta
@@ -874,15 +861,16 @@
 *** this subroutine gives the out-of-phase corrections induced by
 *** mantle inelasticity in the diurnal band
 
 ***  input: xsta,xsun,xmon,fac2sun,fac2mon
 *** output: xcorsta
 
       implicit double precision (a-h,o-z)
-      dimension xsta(3),xsun(3),xmon(3),xcorsta(3)
+      double precision xsta(3),xsun(3),xmon(3),xcorsta(3)
+      double precision fac2sun, fac2mon
       data dhi/-0.0022d0/,dli/-0.0007d0/
 
       rsta=enorm8(xsta)
       sinphi=xsta(3)/rsta
       cosphi=dsqrt(xsta(1)**2+xsta(2)**2)/rsta
       sinla=xsta(2)/cosphi/rsta
       cosla=xsta(1)/cosphi/rsta
@@ -919,14 +907,15 @@
 ***  input:   x(i),i=1,2,3  -- components of vector x
 ***           y(i),i=1,2,3  -- components of vector y
 ***  output:  scal          -- scalar product of x and y
 ***           r1,r2         -- lengths of the two vectors x and y
 
       implicit double precision (a-h,o-z)
       double precision x(3),y(3)
+      double precision r1,r2,scal
 
       r1=dsqrt(x(1)*x(1) + x(2)*x(2) + x(3)*x(3))
       r2=dsqrt(y(1)*y(1) + y(2)*y(2) + y(3)*y(3))
       scal=    x(1)*y(1) + x(2)*y(2) + x(3)*y(3)
 
       return
       end
@@ -965,15 +954,17 @@
 ***         lflag  -- leap second table limit flag,  false:flag not raised
 *** 1."satellite orbits: models, methods, applications" montenbruck & gill(2000)
 *** section 3.3.2, pg. 72-73
 *** 2."astronomy on the personal computer, 4th ed." montenbruck & pfleger (2005)
 *** section 3.2, pg. 38-39  routine MiniMoon
 
       implicit double precision(a-h,o-z)
-      dimension rm(3)
+      double precision rm(3)
+      integer mjd
+      double precision fmjd
       logical lflag,leapflag
       !*** leap second table limit flag
       !*** leap second table limit flag
       save  /limitflag/
       common/limitflag/leapflag
       common/stuff/rad,pi,pi2
 
@@ -1101,14 +1092,16 @@
 
 *** convert mjd/fmjd in UTC time to Greenwich hour angle (in radians)
 
 *** "satellite orbits: models, methods, applications" montenbruck & gill(2000)
 *** section 2.3.1, pg. 33
 
       implicit double precision(a-h,o-z)
+      integer mjd
+      double precision fmjd,ghar
       common/stuff/rad,pi,pi2
 
 *** need UTC to get sidereal time ("astronomy on the personal computer", 4th ed)
 ***                               (pg.43, montenbruck & pfleger, springer, 2005)
 
       !*** UTC time (sec of day)
       !*** UTC time (fract. day)
@@ -1152,15 +1145,17 @@
 ***         lflag  -- leap second table limit flag,  false:flag not raised
 *** 1."satellite orbits: models, methods, applications" montenbruck & gill(2000)
 *** section 3.3.2, pg. 70-71
 *** 2."astronomy on the personal computer, 4th ed." montenbruck & pfleger (2005)
 *** section 3.2, pg. 39  routine MiniSun
 
       implicit double precision(a-h,o-z)
-      dimension rs(3)
+      double precision rs(3)
+      double precision fmjd
+      integer mjd
       logical lflag,leapflag
       !*** leap second table limit flag
       !*** leap second table limit flag
       save  /limitflag/
       common/limitflag/leapflag
       common/stuff/rad,pi,pi2
 
@@ -1235,14 +1230,15 @@
       end
 ********************************************************************************
       subroutine lhsaaz(u,v,w,ra,az,va)
 
 *** determine range,azimuth,vertical angle from local horizon coord.
 
       implicit double precision(a-h,o-z)
+      double precision u,v,w,ra,az,va
       
       s2=u*u+v*v
       r2=s2+w*w
       
       s =dsqrt(s2)
       ra=dsqrt(r2)
       
@@ -1253,14 +1249,15 @@
       end
 *-----------------------------------------------------------------------
       subroutine geoxyz(gla,glo,eht,x,y,z)
 
 *** convert geodetic lat, long, ellip ht. to x,y,z
 
       implicit double precision(a-h,o-z)
+      double precision gla,glo,eht,x,y,z
       common/comgrs/a,e2
 
       sla=dsin(gla)
       cla=dcos(gla)
       w2=1.d0-e2*sla*sla
       w=dsqrt(w2)
       en=a/w
@@ -1274,14 +1271,15 @@
 *-----------------------------------------------------------------------
       subroutine rge(gla,glo,u,v,w,x,y,z)
 
 *** given a rectangular cartesian system (x,y,z)
 *** compute a geodetic h cartesian sys   (u,v,w)
 
       implicit double precision(a-h,o-z)
+      double precision gla,glo,u,v,w,x,y,z
 
       sb=dsin(gla)
       cb=dcos(gla)
       sl=dsin(glo)
       cl=dcos(glo)
 
       u=-sb*cl*x-sb*sl*y+cb*z
@@ -1293,14 +1291,15 @@
 *-----------------------------------------------------------------------
       subroutine rot1(theta,x,y,z,u,v,w)
       
 *** rotate coordinate axes about 1 axis by angle of theta radians
 *** x,y,z transformed into u,v,w
 
       implicit double precision(a-h,o-z)
+      double precision theta,x,y,z,u,v,w
       
       s=dsin(theta)
       c=dcos(theta)
             
       u=x
       v=c*y+s*z
       w=c*z-s*y
@@ -1310,14 +1309,15 @@
 *-----------------------------------------------------------------------
       subroutine rot3(theta,x,y,z,u,v,w)
       
 *** rotate coordinate axes about 3 axis by angle of theta radians
 *** x,y,z transformed into u,v,w
 
       implicit double precision(a-h,o-z)
+      double precision theta,x,y,z,u,v,w
       
       s=dsin(theta)
       c=dcos(theta)
             
       u=c*x+s*y
       v=c*y-s*x
       w=z
@@ -1330,15 +1330,15 @@
       subroutine setjd0(iyr,imo,idy)
 
 *** set the integer part of a modified julian date as epoch, mjd0
 *** the modified julian day is derived from civil time as in civmjd()
 *** allows single number expression of time in seconds w.r.t. mjd0
 
       implicit double precision(a-h,o-z)
-      integer y
+      integer y,iyr,imo,idy
       save /mjdoff/
       common/mjdoff/mjd0
 
       if(iyr.lt.1900) stop 34587
 
       if(imo.le.2) then
         y=iyr-1
@@ -1365,15 +1365,16 @@
 
 *** imo in range 1-12, idy in range 1-31
 *** only valid in range mar-1900 thru feb-2100     (leap year protocols)
 *** ref: hofmann-wellenhof, 2nd ed., pg 34-35
 *** adapted from civmjd()
 
       implicit double precision(a-h,o-z)
-      integer y
+      integer y,iyr,imo,idy,ihr,imn
+      double precision sec,tsec
       save /mjdoff/
       common/mjdoff/mjd0
 
       if(iyr.lt.1900) stop 34589
 
       if(imo.le.2) then
         y=iyr-1
@@ -1398,14 +1399,16 @@
 
 *** imo in range 1-12, idy in range 1-31
 *** only valid in range mar-1900 thru feb-2100
 *** ref: hofmann-wellenhof, 2nd ed., pg 34-35
 *** adapted from mjdciv()
 
       implicit double precision(a-h,o-z)
+      integer iyr,imo,idy,ihr,imn
+      double precision sec,tsec
       save /mjdoff/
       common/mjdoff/mjd0
 
       mjd=mjd0+tsec/86400.d0
 *** the following equation preserves significant digits
       fmjd=dmod(tsec,86400.d0)/86400.d0
 
@@ -1441,15 +1444,16 @@
 
 *** imo in range 1-12, idy in range 1-31
 *** only valid in range mar-1900 thru feb-2100     (leap year protocols)
 *** ref: hofmann-wellenhof, 2nd ed., pg 34-35
 *** operation confirmed against table 3.3 values on pg.34
 
       implicit double precision(a-h,o-z)
-      integer y
+      integer y,iyr,imo,idy,ihr,imn,mjd
+      double precision sec,fmjd
 
       if(iyr.lt.1900) stop 34588
 
       if(imo.le.2) then
         y=iyr-1
         m=imo+12
       else
@@ -1472,14 +1476,16 @@
 
 *** imo in range 1-12, idy in range 1-31
 *** only valid in range mar-1900 thru feb-2100
 *** ref: hofmann-wellenhof, 2nd ed., pg 34-35
 *** operation confirmed for leap years (incl. year 2000)
 
       implicit double precision(a-h,o-z)
+      integer mjd,iyr,imo,idy,ihr,imn
+      double precision fmjd,sec
 
       rjd=mjd+fmjd+2400000.5d0
       ia=(rjd+0.5d0)
       ib=ia+1537
       ic=(ib-122.1d0)/365.25d0
       id=365.25d0*ic
       ie=(ib-id)/30.6001d0
@@ -1506,38 +1512,41 @@
 *** new supplemental time functions ************************************
 ************************************************************************
       double precision function utc2ttt(tutc)
 
 *** convert utc (sec) to terrestrial time (sec)
 
       implicit double precision(a-h,o-z)
+      double precision tutc
 
       ttai   = utc2tai(tutc)
       utc2ttt= tai2tt(ttai)
 
       return
       end
 *-----------------------------------------------------------------------
       double precision function gps2ttt(tgps)
 
 *** convert gps time (sec) to terrestrial time (sec)
 
       implicit double precision(a-h,o-z)
+      double precision tgps
 
       ttai   = gps2tai(tgps)
       gps2ttt= tai2tt(ttai)
 
       return
       end
 *-----------------------------------------------------------------------
       double precision function utc2tai(tutc)
 
 *** convert utc (sec) to tai (sec)
 
       implicit double precision(a-h,o-z)
+      double precision tutc
 
       utc2tai = tutc - getutcmtai(tutc)
 
       return
       end
 *-----------------------------------------------------------------------
       double precision function getutcmtai(tsec)
@@ -1545,17 +1554,18 @@
 *** get utc - tai (s)
 
 ***** "Julian Date Converter"
 ***** http://aa.usno.navy.mil/data/docs/JulianDate.php
 ***** http://www.csgnetwork.com/julianmodifdateconv.html
 
       implicit double precision(a-h,o-z)
-      !*** upper limit, leap second table, 2023jun28
+      double precision tsec
+      !*** upper limit, leap second table, 2023dec28
       !*** lower limit, leap second table, 1972jan01
-      parameter(MJDUPPER=60123)
+      parameter(MJDUPPER=60306)
       parameter(MJDLOWER=41317)
 
       !*** leap second table limit flag
       logical leapflag
       save  /limitflag/
       !*** leap second table limit flag
       common/limitflag/leapflag
@@ -1628,15 +1638,15 @@
 *** 2009 JAN  1 =JD 2454832.5  TAI-UTC=  34.0s
 *** 2012 JUL  1 =JD 2456109.5  TAI-UTC=  35.0s
 *** 2015 JUL  1 =JD 2457204.5  TAI-UTC=  36.0s
 *** 2017 JAN  1 =JD 2457754.5  TAI-UTC=  37.0s
 ***** other leap second references at:
 ***** http://hpiers.obspm.fr/eoppc/bul/bulc/Leap_Second_History.dat
 ***** http://hpiers.obspm.fr/eoppc/bul/bulc/bulletinc.dat
-***** File expires on 28 June 2023
+***** File expires on 28 December 2023
 
 *** test against newest leaps first
 
       if    (mjd0t.ge.57754) then
         !*** 2017 JAN 1 = 57754
         tai_utc = 37.d0
       elseif(mjd0t.ge.57204) then
@@ -1737,26 +1747,28 @@
       end
 *-----------------------------------------------------------------------
       double precision function tai2tt(ttai)
 
 *** convert tai (sec) to terrestrial time (sec)
 
       implicit double precision(a-h,o-z)
+      double precision ttai
 
 ***** http://tycho.usno.navy.mil/systime.html
       tai2tt = ttai + 32.184d0
 
       return
       end
 *-----------------------------------------------------------------------
       double precision function gps2tai(tgps)
 
 *** convert gps time (sec) to tai (sec)
 
       implicit double precision(a-h,o-z)
+      double precision tgps
 
 ***** http://leapsecond.com/java/gpsclock.htm
 ***** http://tycho.usno.navy.mil/leapsec.html
       gps2tai = tgps + 19.d0
 
       return
       end
```

### Comparing `pysolid-0.2.3/src/pysolid.egg-info/PKG-INFO` & `pysolid-0.3.0/src/pysolid.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: pysolid
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Python wrapper for solid to compute solid Earth tides
 Home-page: https://github.com/insarlab/PySolid
-Download-URL: https://github.com/insarlab/PySolid/archive/v0.2.3.tar.gz
 Author: Zhang Yunjun, Dennis Milbert
 Author-email: yunjunzgeo@gmail.com
 License: GPL-3.0-or-later
 Project-URL: Bug Reports, https://github.com/insarlab/PySolid/issues
 Project-URL: Source, https://github.com/insarlab/PySolid
 Keywords: solid Eartth tides,deformation,geodesy,geophysics
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Language](https://img.shields.io/badge/python-3.6%2B-blue.svg)](https://www.python.org/)
-[![CircleCI](https://img.shields.io/circleci/build/github/insarlab/PySolid.svg?logo=circleci&label=test)](https://circleci.com/gh/insarlab/PySolid)
-[![Version](https://img.shields.io/github/v/release/insarlab/PySolid?color=green)](https://github.com/insarlab/PySolid/releases)
-[![License](https://img.shields.io/badge/license-GPLv3+-yellow.svg)](https://github.com/insarlab/PySolid/blob/main/LICENSE)
-[![Citation](https://img.shields.io/badge/doi-10.1109%2FTGRS.2022.3168509-blue)](https://doi.org/10.1109/TGRS.2022.3168509)
+[![Language](https://img.shields.io/badge/python-3.8%2B-blue.svg?style=flat-square)](https://www.python.org/)
+[![CircleCI](https://img.shields.io/circleci/build/github/insarlab/PySolid.svg?logo=circleci&label=test&style=flat-square)](https://circleci.com/gh/insarlab/PySolid)
+[![Version](https://img.shields.io/github/v/release/insarlab/PySolid?color=brightgreen&label=version&style=flat-square)](https://github.com/insarlab/PySolid/releases)
+[![Conda Download](https://img.shields.io/conda/dn/conda-forge/pysolid?color=green&style=flat-square)](https://anaconda.org/conda-forge/pysolid)
+[![License](https://img.shields.io/badge/license-GPLv3+-yellow.svg?style=flat-square)](https://github.com/insarlab/PySolid/blob/main/LICENSE)
+[![Citation](https://img.shields.io/badge/doi-10.1109%2FTGRS.2022.3168509-blue?style=flat-square)](https://doi.org/10.1109/TGRS.2022.3168509)
 
 ## PySolid
 
-The Python based solid Earth tides (PySolid) is a thin Python wrapper of the [`solid.for`](http://geodesyworld.github.io/SOFTS/solid.htm) program (by Dennis Milbert based on [_dehanttideinelMJD.f_](https://iers-conventions.obspm.fr/content/chapter7/software/dehanttideinel/) from V. Dehant, S. Mathews, J. Gipson and C. Bruyninx) to calculate [solid Earth tides](https://en.wikipedia.org/wiki/Earth_tide) in east/north/up direction (section 7.1.1 in the [2010 IERS Conventions](https://www.iers.org/IERS/EN/Publications/TechnicalNotes/tn36.html)). Solid Earth tides introduces very long spatial wavelength components in SAR/InSAR observations, as shown in the Sentinel-1 data with regular acquisitions and large swaths (Yunjun et al., 2022).
+The Python based solid Earth tides (PySolid) is a thin Python wrapper of the [`solid.for`](http://geodesyworld.github.io/SOFTS/solid.htm) program (by Dennis Milbert based on [_dehanttideinelMJD.f_](https://iers-conventions.obspm.fr/content/chapter7/software/dehanttideinel/) from V. Dehant, S. Mathews, J. Gipson and C. Bruyninx) to calculate [solid Earth tides](https://en.wikipedia.org/wiki/Earth_tide) in east, north and up directions (section 7.1.1 in the [2010 IERS Conventions](https://www.iers.org/IERS/EN/Publications/TechnicalNotes/tn36.html)). Solid Earth tides introduce large offsets in SAR observations and long spatial wavelength ramps in InSAR observations, as shown in the Sentinel-1 data with regular acquisitions and large swaths ([Yunjun et al., 2022](https://doi.org/10.1109/TGRS.2022.3168509)).
 
 This is research code provided to you "as is" with NO WARRANTIES OF CORRECTNESS. Use at your own risk.
 
 ### 1. Install
 
 PySolid is available on the [conda-forge](https://anaconda.org/conda-forge/pysolid) channel and the main archive of the [Debian](https://tracker.debian.org/pkg/pysolid) GNU/Linux OS. The released version can be install via `conda` as:
 
@@ -43,17 +44,16 @@
 
 or via `apt` (or other package managers) for [Debian-derivative OS](https://wiki.debian.org/Derivatives/Census) users, including [Ubuntu](https://ubuntu.com), as:
 
 ```shell
 apt install python3-pysolid
 ```
 
-Installing via `conda` and `apt` is recomended because PySolid contains Fortran source code, which required compilcation. Otherwise, you may build it from source as described below.
-
-#### 1.1 Build from source
+<details>
+<p><summary>Or build from source:</summary></p>
 
 PySolid relies on a few Python modules as described in [requirements.txt](./requirements.txt) and [NumPy's f2py](https://numpy.org/doc/stable/f2py/) to build the Fortran source code. You could use `conda` to install all the dependencies, including the Fortran compiler, or use your own installed Fortran compiler and `pip` to install the rest.
 
 ##### a. Download source code
 
 ```bash
 # run "cd PySolid; git pull" to update to the latest development version
@@ -74,36 +74,41 @@
 python -m pip install -r PySolid/requirements.txt
 ```
 
 ##### c. Install PySolid
 
 ```bash
 # option 1: use pip to install pysolid into the current environment
-# use "pip install -e" to install in the development mode
 python -m pip install PySolid
 
-# option 2: manually compile the Fortran code and setup environment variable
+# option 2: use pip to install pysolid in develop mode (editable) into the current environment
+# setting an environmental variable as below is required for editable installs via pyproject.toml
+export SETUPTOOLS_ENABLE_FEATURES="legacy-editable"
+python -m pip install -e PySolid
+
+# option 3: manually compile the Fortran code and setup environment variable
 cd PySolid/src/pysolid
 f2py -c -m solid solid.for
 export PYTHONPATH=${PYTHONPATH}:~/tools/PySolid
 ```
 
-#### 1.2 Test the installation
+##### d. Test the installation
 
 To test the installation, run the following:
 
 ```bash
 python -c "import pysolid; print(pysolid.__version__)"
 python PySolid/tests/grid.py
 python PySolid/tests/point.py
 ```
+</details>
 
 ### 2. Usage
 
-PySolid could compute solid Earth tides in two modes: **point** and **grid**. Both modes produce displacement in east, north and up direction.
+PySolid could compute solid Earth tides in two modes: **point** and **grid**. Both modes produce displacement in east, north and up directions.
 
 +   **Point mode:** compute 1D tides time-series at a specific point for a given time period
 +   **Grid mode:** compute 2D tides grid at a specific time for a given spatial grid
 
 #### 2.1 Point Mode [[notebook](./docs/plot_point_SET.ipynb)]
 
 ```python
@@ -154,15 +159,15 @@
 # compute SET via pysolid
 tide_e, tide_n, tide_u = pysolid.calc_solid_earth_tides_grid(
     dt_obj, meta,
     display=False,
     verbose=True,
 )
 
-# project SET from ENU to radar line-of-sight (LOS) direction with positive for motion towards satellite
+# project SET from ENU to satellite line-of-sight (LOS) direction with positive for motion towards the satellite
 # inc_angle : incidence angle of the LOS vector (from ground to radar platform) measured from vertical.
 # az_angle  : azimuth   angle of the LOS vector (from ground to radar platform) measured from the north, with anti-clockwirse as positive.
 inc_angle = np.deg2rad(34)   # radian, typical value for Sentinel-1
 az_angle = np.deg2rad(-102)  # radian, typical value for Sentinel-1 descending track
 tide_los = (  tide_e * np.sin(inc_angle) * np.sin(az_angle) * -1
             + tide_n * np.sin(inc_angle) * np.cos(az_angle)
             + tide_u * np.cos(inc_angle))
@@ -172,7 +177,9 @@
   <img width="800" src="https://yunjunzhang.files.wordpress.com/2021/01/set_grid-3.png">
 </p>
 
 ### 3. Citing this work
 
 +   Yunjun, Z., Fattahi, H., Pi, X., Rosen, P., Simons, M., Agram, P., & Aoki, Y. (2022). Range Geolocation Accuracy of C-/L-band SAR and its Implications for Operational Stack Coregistration. _IEEE Trans. Geosci. Remote Sens., 60_, 1-19, doi:[10.1109/TGRS.2022.3168509](https://doi.org/10.1109/TGRS.2022.3168509), [arXiv](https://doi.org/10.31223/X5F641), [data](https://zenodo.org/record/6360749), [notebooks](https://github.com/yunjunz/2022-Geolocation).
 +   Milbert, D. (2018), "solid: Solid Earth Tide", [Online]. Available: http://geodesyworld.github.io/SOFTS/solid.htm. Accessd on: 2020-09-06.
+
+
```

