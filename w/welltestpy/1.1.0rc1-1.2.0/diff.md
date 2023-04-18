# Comparing `tmp/welltestpy-1.1.0rc1.tar.gz` & `tmp/welltestpy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "welltestpy-1.1.0rc1.tar", last modified: Wed Jul 28 14:10:07 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `welltestpy-1.1.0rc1.tar` & `welltestpy-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 14:10:07.252604 welltestpy-1.1.0rc1/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3607 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (121)      129 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6089 2021-07-28 14:10:07.252604 welltestpy-1.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4205 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2083 2021-07-28 14:10:07.252604 welltestpy-1.1.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 14:10:07.248604 welltestpy-1.1.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1021 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (121)     5588 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/tests/test_welltestpy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 14:10:07.248604 welltestpy-1.1.0rc1/welltestpy/
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-07-28 14:10:07.000000 welltestpy-1.1.0rc1/welltestpy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 14:10:07.252604 welltestpy-1.1.0rc1/welltestpy/data/
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16854 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/data/campaignlib.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    28167 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/data/data_io.py
--rw-r--r--   0 runner    (1001) docker     (121)    17933 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/data/testslib.py
--rw-r--r--   0 runner    (1001) docker     (121)    27408 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/data/varlib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 14:10:07.252604 welltestpy-1.1.0rc1/welltestpy/estimate/
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/estimate/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    21705 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/estimate/estimators.py
--rw-r--r--   0 runner    (1001) docker     (121)     6155 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/estimate/spotpylib.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    22391 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/estimate/steady_lib.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    23759 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/estimate/transient_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 14:10:07.252604 welltestpy-1.1.0rc1/welltestpy/process/
--rw-r--r--   0 runner    (1001) docker     (121)      635 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9647 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/process/processlib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 14:10:07.252604 welltestpy-1.1.0rc1/welltestpy/tools/
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3571 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/tools/diagnostic_plots.py
--rw-r--r--   0 runner    (1001) docker     (121)    28700 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/tools/plotter.py
--rw-r--r--   0 runner    (1001) docker     (121)    12190 2021-07-28 14:09:08.000000 welltestpy-1.1.0rc1/welltestpy/tools/trilib.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 14:10:07.252604 welltestpy-1.1.0rc1/welltestpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      655 2021-07-28 14:10:07.000000 welltestpy-1.1.0rc1/welltestpy.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/_version.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/data/__init__.py
+-rw-r--r--   0        0        0    16759 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/data/campaignlib.py
+-rwxr-xr-x   0        0        0    28056 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/data/data_io.py
+-rw-r--r--   0        0        0    17774 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/data/testslib.py
+-rw-r--r--   0        0        0    27120 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/data/varlib.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/estimate/__init__.py
+-rwxr-xr-x   0        0        0    30495 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/estimate/estimators.py
+-rw-r--r--   0        0        0     6480 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/estimate/spotpylib.py
+-rwxr-xr-x   0        0        0    22373 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/estimate/steady_lib.py
+-rwxr-xr-x   0        0        0    23794 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/estimate/transient_lib.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/process/__init__.py
+-rw-r--r--   0        0        0     9415 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/process/processlib.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/tools/__init__.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/tools/diagnostic_plots.py
+-rw-r--r--   0        0        0    29697 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/tools/plotter.py
+-rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 welltestpy-1.2.0/src/welltestpy/tools/trilib.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 welltestpy-1.2.0/tests/test_process.py
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 welltestpy-1.2.0/tests/test_welltestpy.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 welltestpy-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 welltestpy-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 welltestpy-1.2.0/README.md
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 welltestpy-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 welltestpy-1.2.0/PKG-INFO
```

### Comparing `welltestpy-1.1.0rc1/LICENSE` & `welltestpy-1.2.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021 Sebastian Müller, Jarno Herrmann
+Copyright (c) 2023 Sebastian Müller, Jarno Herrmann
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `welltestpy-1.1.0rc1/PKG-INFO` & `welltestpy-1.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: welltestpy
-Version: 1.1.0rc1
+Version: 1.2.0
 Summary: welltestpy - package to handle well-based Field-campaigns.
-Home-page: https://github.com/GeoStat-Framework/welltestpy
-Author: Sebastian Müller, Jarno Herrmann
-Author-email: info@geostat-framework.org
-Maintainer: Sebastian Müller
-Maintainer-email: info@geostat-framework.org
-License: MIT
+Project-URL: Homepage, https://github.com/GeoStat-Framework/welltestpy
 Project-URL: Documentation, https://welltestpy.readthedocs.io
 Project-URL: Source, https://github.com/GeoStat-Framework/welltestpy
 Project-URL: Tracker, https://github.com/GeoStat-Framework/welltestpy/issues
 Project-URL: Changelog, https://github.com/GeoStat-Framework/welltestpy/blob/main/CHANGELOG.md
 Project-URL: Conda-Forge, https://anaconda.org/conda-forge/welltestpy
-Platform: any
+Author-email: "Sebastian Müller, Jarno Herrmann" <info@geostat-framework.org>
+License-Expression: MIT
+License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
@@ -32,19 +29,34 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Requires-Python: >=3.7
+Requires-Dist: anaflow>=1.0.0
+Requires-Dist: matplotlib>=3.0.0
+Requires-Dist: numpy>=1.14.5
+Requires-Dist: packaging>=20
+Requires-Dist: scipy>=1.1.0
+Requires-Dist: spotpy>=1.5.0
+Provides-Extra: check
+Requires-Dist: black<24,>=23; extra == 'check'
+Requires-Dist: isort[colors]<6; extra == 'check'
+Requires-Dist: pylint<3; extra == 'check'
 Provides-Extra: doc
+Requires-Dist: m2r2>=0.2.8; extra == 'doc'
+Requires-Dist: numpydoc>=1.1; extra == 'doc'
+Requires-Dist: sphinx-gallery>=0.8; extra == 'doc'
+Requires-Dist: sphinx-rtd-theme<1.1,>=1; extra == 'doc'
+Requires-Dist: sphinx>=4; extra == 'doc'
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest-cov>=3; extra == 'test'
+Description-Content-Type: text/markdown
 
 # Welcome to welltestpy
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1229051.svg)](https://doi.org/10.5281/zenodo.1229051)
 [![PyPI version](https://badge.fury.io/py/welltestpy.svg)](https://badge.fury.io/py/welltestpy)
 [![Build Status](https://github.com/GeoStat-Framework/welltestpy/workflows/Continuous%20Integration/badge.svg?branch=main)](https://github.com/GeoStat-Framework/welltestpy/actions)
 [![Coverage Status](https://coveralls.io/repos/github/GeoStat-Framework/welltestpy/badge.svg?branch=main)](https://coveralls.io/github/GeoStat-Framework/welltestpy?branch=main)
@@ -62,112 +74,57 @@
 
 ## Installation
 
 You can install the latest version with the following command:
 
     pip install welltestpy
 
+Or from conda
 
-## Documentation for welltestpy
-
-You can find the documentation under [https://welltestpy.readthedocs.io][doc_link].
-
-
-### Example 1: A campaign containing a pumping test
-
-In the following, we will take a look at an artificial pumping test campaign,
-that is stored in a file called `Cmp_UFZ-campaign.cmp`.
-
-```python
-import welltestpy as wtp
-
-# load the campaign
-campaign = wtp.load_campaign("Cmp_UFZ-campaign.cmp")
-
-# plot the well constellation and a test overview
-campaign.plot_wells()
-campaign.plot()
-```
-
-#### This will give the following plots:
+    conda install -c conda-forge welltestpy
 
-<p align="center">
-<img src="https://raw.githubusercontent.com/GeoStat-Framework/welltestpy/main/docs/source/pics/01_wells.png" alt="Wells" width="600px"/>
-</p>
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/GeoStat-Framework/welltestpy/main/docs/source/pics/01_pumptest.png" alt="Pumptest" width="600px"/>
-</p>
 
+## Documentation for welltestpy
 
-### Example 2: Estimate transmissivity and storativity
-
-The pumping test from example 1 can now be loaded and used to estimate the values for
-transmissivity and storativity.
-
-```python
-import welltestpy as wtp
-
-campaign = wtp.load_campaign("Cmp_UFZ-campaign.cmp")
-estimation = wtp.estimate.Theis("Estimate_theis", campaign, generate=True)
-estimation.run()
-```
-
-#### This will give the following plots:
-
-Type-Curve fitting:
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/GeoStat-Framework/welltestpy/main/docs/source/pics/02_fit.png" alt="Fit" width="600px"/>
-</p>
-
-Evolution of parameter estimation with SCE:
+You can find the documentation including tutorials and examples under
+https://welltestpy.readthedocs.io.
 
-<p align="center">
-<img src="https://raw.githubusercontent.com/GeoStat-Framework/welltestpy/main/docs/source/pics/02_paratrace.png" alt="Trace" width="600px"/>
-</p>
 
-Scatterplot of paramter distribution during estimation:
+## Citing welltestpy
 
-<p align="center">
-<img src="https://raw.githubusercontent.com/GeoStat-Framework/welltestpy/main/docs/source/pics/02_parainter.png" alt="Interaction" width="600px"/>
-</p>
+If you are using this package you can cite our
+[Groundwater publication](https://doi.org/10.1111/gwat.13121) by:
 
-The results are:
+> Müller, S., Leven, C., Dietrich, P., Attinger, S. and Zech, A. (2021):
+> How to Find Aquifer Statistics Utilizing Pumping Tests? Two Field Studies Using welltestpy.
+> Groundwater, https://doi.org/10.1111/gwat.13121
 
-* `ln(T) = -9.22` which is equivalent to `T = 0.99 * 10^-4 m^2/s`
-* `ln(S) = -9.10` which is equivalent to `S = 1.11 * 10^-4`
+To cite the code, please visit the [Zenodo page](https://doi.org/10.5281/zenodo.1229051).
 
 
-### Provided Subpackages
+## Provided Subpackages
 
 ```python
 welltestpy.data      # Subpackage to handle data from field campaigns
 welltestpy.estimate  # Subpackage to estimate field parameters
 welltestpy.process   # Subpackage to pre- and post-process data
 welltestpy.tools     # Subpackage with tools for plotting and triagulation
 ```
 
 
 ## Requirements
 
 - [NumPy >= 1.14.5](https://www.numpy.org)
 - [SciPy >= 1.1.0](https://www.scipy.org)
-- [Pandas >= 0.23.2](https://pandas.pydata.org)
 - [AnaFlow >= 1.0.0](https://github.com/GeoStat-Framework/AnaFlow)
 - [SpotPy >= 1.5.0](https://github.com/thouska/spotpy)
 - [Matplotlib >= 3.0.0](https://matplotlib.org)
 
 
 ## Contact
 
 You can contact us via <info@geostat-framework.org>.
 
 
 ## License
 
-[MIT][license_link] © 2018-2021
-
-[license_link]: https://github.com/GeoStat-Framework/welltestpy/blob/main/LICENSE
-[doc_link]: https://welltestpy.readthedocs.io
-
-
+[MIT](https://github.com/GeoStat-Framework/welltestpy/blob/main/LICENSE)
```

### Comparing `welltestpy-1.1.0rc1/README.md` & `welltestpy-1.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -18,110 +18,57 @@
 
 ## Installation
 
 You can install the latest version with the following command:
 
     pip install welltestpy
 
+Or from conda
 
-## Documentation for welltestpy
-
-You can find the documentation under [https://welltestpy.readthedocs.io][doc_link].
-
-
-### Example 1: A campaign containing a pumping test
-
-In the following, we will take a look at an artificial pumping test campaign,
-that is stored in a file called `Cmp_UFZ-campaign.cmp`.
-
-```python
-import welltestpy as wtp
-
-# load the campaign
-campaign = wtp.load_campaign("Cmp_UFZ-campaign.cmp")
-
-# plot the well constellation and a test overview
-campaign.plot_wells()
-campaign.plot()
-```
-
-#### This will give the following plots:
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/GeoStat-Framework/welltestpy/main/docs/source/pics/01_wells.png" alt="Wells" width="600px"/>
-</p>
+    conda install -c conda-forge welltestpy
 
-<p align="center">
-<img src="https://raw.githubusercontent.com/GeoStat-Framework/welltestpy/main/docs/source/pics/01_pumptest.png" alt="Pumptest" width="600px"/>
-</p>
 
+## Documentation for welltestpy
 
-### Example 2: Estimate transmissivity and storativity
-
-The pumping test from example 1 can now be loaded and used to estimate the values for
-transmissivity and storativity.
-
-```python
-import welltestpy as wtp
-
-campaign = wtp.load_campaign("Cmp_UFZ-campaign.cmp")
-estimation = wtp.estimate.Theis("Estimate_theis", campaign, generate=True)
-estimation.run()
-```
-
-#### This will give the following plots:
-
-Type-Curve fitting:
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/GeoStat-Framework/welltestpy/main/docs/source/pics/02_fit.png" alt="Fit" width="600px"/>
-</p>
-
-Evolution of parameter estimation with SCE:
+You can find the documentation including tutorials and examples under
+https://welltestpy.readthedocs.io.
 
-<p align="center">
-<img src="https://raw.githubusercontent.com/GeoStat-Framework/welltestpy/main/docs/source/pics/02_paratrace.png" alt="Trace" width="600px"/>
-</p>
 
-Scatterplot of paramter distribution during estimation:
+## Citing welltestpy
 
-<p align="center">
-<img src="https://raw.githubusercontent.com/GeoStat-Framework/welltestpy/main/docs/source/pics/02_parainter.png" alt="Interaction" width="600px"/>
-</p>
+If you are using this package you can cite our
+[Groundwater publication](https://doi.org/10.1111/gwat.13121) by:
 
-The results are:
+> Müller, S., Leven, C., Dietrich, P., Attinger, S. and Zech, A. (2021):
+> How to Find Aquifer Statistics Utilizing Pumping Tests? Two Field Studies Using welltestpy.
+> Groundwater, https://doi.org/10.1111/gwat.13121
 
-* `ln(T) = -9.22` which is equivalent to `T = 0.99 * 10^-4 m^2/s`
-* `ln(S) = -9.10` which is equivalent to `S = 1.11 * 10^-4`
+To cite the code, please visit the [Zenodo page](https://doi.org/10.5281/zenodo.1229051).
 
 
-### Provided Subpackages
+## Provided Subpackages
 
 ```python
 welltestpy.data      # Subpackage to handle data from field campaigns
 welltestpy.estimate  # Subpackage to estimate field parameters
 welltestpy.process   # Subpackage to pre- and post-process data
 welltestpy.tools     # Subpackage with tools for plotting and triagulation
 ```
 
 
 ## Requirements
 
 - [NumPy >= 1.14.5](https://www.numpy.org)
 - [SciPy >= 1.1.0](https://www.scipy.org)
-- [Pandas >= 0.23.2](https://pandas.pydata.org)
 - [AnaFlow >= 1.0.0](https://github.com/GeoStat-Framework/AnaFlow)
 - [SpotPy >= 1.5.0](https://github.com/thouska/spotpy)
 - [Matplotlib >= 3.0.0](https://matplotlib.org)
 
 
 ## Contact
 
 You can contact us via <info@geostat-framework.org>.
 
 
 ## License
 
-[MIT][license_link] © 2018-2021
-
-[license_link]: https://github.com/GeoStat-Framework/welltestpy/blob/main/LICENSE
-[doc_link]: https://welltestpy.readthedocs.io
+[MIT](https://github.com/GeoStat-Framework/welltestpy/blob/main/LICENSE)
```

### Comparing `welltestpy-1.1.0rc1/tests/test_process.py` & `welltestpy-1.2.0/tests/test_process.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# -*- coding: utf-8 -*-
 """
 This is the unittest of welltestpy.process.
 """
+import copy
 import unittest
+
 import numpy as np
-import copy
+
 import welltestpy as wtp
 
 
 class TestProcess(unittest.TestCase):
     def setUp(self):
         # generate artificial data
         self.trns_obs = wtp.data.DrawdownObs("trans", [1, 2, 3], [4, 5, 6])
```

### Comparing `welltestpy-1.1.0rc1/tests/test_welltestpy.py` & `welltestpy-1.2.0/tests/test_welltestpy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# -*- coding: utf-8 -*-
 """
 This is the unittest of AnaFlow.
 """
 
 import unittest
-import numpy as np
+
 import matplotlib as mpl
+import numpy as np
 
 mpl.use("Agg")
 
-import welltestpy as wtp
-from welltestpy.tools import triangulate, sym, plot_well_pos
-
 import anaflow as ana
 
+import welltestpy as wtp
+from welltestpy.tools import plot_well_pos, sym, triangulate
+
 
 class TestWTP(unittest.TestCase):
     def setUp(self):
         self.rate = -1e-4
         self.time = np.geomspace(10, 7200, 10)
         self.transmissivity = 1e-4
         self.storage = 1e-4
@@ -75,58 +75,68 @@
 
     def test_est_theis(self):
         campaign = wtp.load_campaign("Cmp_UFZ-campaign.cmp")
         estimation = wtp.estimate.Theis("est_theis", campaign, generate=True)
         estimation.run()
         res = estimation.estimated_para
         estimation.sensitivity()
-        self.assertAlmostEqual(np.exp(res["mu"]), self.transmissivity, 2)
-        self.assertAlmostEqual(np.exp(res["lnS"]), self.storage, 2)
+        self.assertAlmostEqual(
+            np.exp(res["transmissivity"]), self.transmissivity, 2
+        )
+        self.assertAlmostEqual(np.exp(res["storage"]), self.storage, 2)
         sens = estimation.sens
         for s_typ in self.s_types:
-            self.assertTrue(sens[s_typ]["mu"] > sens[s_typ]["lnS"])
+            self.assertTrue(
+                sens[s_typ]["transmissivity"] > sens[s_typ]["storage"]
+            )
 
     def test_est_thiem(self):
         campaign = wtp.load_campaign("Cmp_UFZ-campaign.cmp")
         estimation = wtp.estimate.Thiem("est_thiem", campaign, generate=True)
         estimation.run()
         res = estimation.estimated_para
         # since we only have one parameter,
         # we need a dummy parameter to estimate sensitivity
         estimation.gen_setup(dummy=True)
         estimation.sensitivity()
-        self.assertAlmostEqual(np.exp(res["mu"]), self.transmissivity, 2)
+        self.assertAlmostEqual(
+            np.exp(res["transmissivity"]), self.transmissivity, 2
+        )
         sens = estimation.sens
         for s_typ in self.s_types:
-            self.assertTrue(sens[s_typ]["mu"] > sens[s_typ]["dummy"])
+            self.assertTrue(
+                sens[s_typ]["transmissivity"] > sens[s_typ]["dummy"]
+            )
 
     def test_est_ext_thiem2D(self):
         campaign = wtp.load_campaign("Cmp_UFZ-campaign.cmp")
         estimation = wtp.estimate.ExtThiem2D(
             "est_ext_thiem2D", campaign, generate=True
         )
         estimation.run()
         res = estimation.estimated_para
         estimation.sensitivity()
-        self.assertAlmostEqual(np.exp(res["mu"]), self.transmissivity, 2)
+        self.assertAlmostEqual(
+            np.exp(res["trans_gmean"]), self.transmissivity, 2
+        )
         self.assertAlmostEqual(res["var"], 0.0, 0)
         sens = estimation.sens
         for s_typ in self.s_types:
-            self.assertTrue(sens[s_typ]["mu"] > sens[s_typ]["var"])
+            self.assertTrue(sens[s_typ]["trans_gmean"] > sens[s_typ]["var"])
             self.assertTrue(sens[s_typ]["var"] > sens[s_typ]["len_scale"])
 
     # def test_est_ext_thiem3D(self):
     #     campaign = wtp.load_campaign("Cmp_UFZ-campaign.cmp")
     #     estimation = wtp.estimate.ExtThiem3D(
     #         "est_ext_thiem3D", campaign, generate=True
     #     )
     #     estimation.run()
     #     res = estimation.estimated_para
     #     estimation.sensitivity()
-    #     self.assertAlmostEqual(np.exp(res["mu"]), self.transmissivity, 2)
+    #     self.assertAlmostEqual(np.exp(res["cond_gmean"]), self.transmissivity, 2)
     #     self.assertAlmostEqual(res["var"], 0.0, 0)
 
     def test_triangulate(self):
         dist_mat = np.zeros((4, 4), dtype=float)
         dist_mat[0, 1] = 3  # distance between well 0 and 1
         dist_mat[0, 2] = 4  # distance between well 0 and 2
         dist_mat[1, 2] = 2  # distance between well 1 and 2
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/__init__.py` & `welltestpy-1.2.0/src/welltestpy/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,62 @@
-# -*- coding: utf-8 -*-
 """
-Purpose
-=======
+welltestpy - a Python package to handle well-based Field-campaigns.
 
 welltestpy provides a framework to handle and plot data from well based
 field campaigns as well as a parameter estimation module.
 
 Subpackages
 ^^^^^^^^^^^
 
 .. autosummary::
-    data
-    estimate
-    process
-    tools
+   :toctree: api
+
+   data
+   estimate
+   process
+   tools
 
 Classes
 ^^^^^^^
 
 Campaign classes
 ~~~~~~~~~~~~~~~~
 
-.. currentmodule:: welltestpy.data.campaignlib
+.. currentmodule:: welltestpy.data
 
 The following classes can be used to handle field campaigns.
 
 .. autosummary::
-    Campaign
-    FieldSite
+   Campaign
+   FieldSite
 
 Field Test classes
 ~~~~~~~~~~~~~~~~~~
 
-.. currentmodule:: welltestpy.data.testslib
-
 The following classes can be used to handle field test within a campaign.
 
 .. autosummary::
-    PumpingTest
+   PumpingTest
 
 Loading routines
 ^^^^^^^^^^^^^^^^
 
-.. currentmodule:: welltestpy.data.data_io
-
 Campaign related loading routines
 
 .. autosummary::
-    load_campaign
+   load_campaign
 """
 from . import data, estimate, process, tools
 
 try:
     from ._version import __version__
 except ImportError:  # pragma: nocover
     # package is not installed
     __version__ = "0.0.0.dev0"
 
 from .data.campaignlib import Campaign, FieldSite
-from .data.testslib import PumpingTest
 from .data.data_io import load_campaign
+from .data.testslib import PumpingTest
 
 __all__ = ["__version__"]
 __all__ += ["data", "estimate", "process", "tools"]
 __all__ += ["Campaign", "FieldSite", "PumpingTest", "load_campaign"]
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/data/__init__.py` & `welltestpy-1.2.0/src/welltestpy/data/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,102 @@
-# -*- coding: utf-8 -*-
 """
 welltestpy subpackage providing datastructures.
 
-Subpackages
-^^^^^^^^^^^
-
-.. currentmodule:: welltestpy.data
-
-.. autosummary::
-    data_io
-    varlib
-    testslib
-    campaignlib
-
-Classes
-^^^^^^^
-
 Campaign classes
 ~~~~~~~~~~~~~~~~
 
-.. currentmodule:: welltestpy.data.campaignlib
-
 The following classes can be used to handle field campaigns.
 
 .. autosummary::
+   :toctree:
+
     Campaign
     FieldSite
 
 Field Test classes
 ~~~~~~~~~~~~~~~~~~
 
-.. currentmodule:: welltestpy.data.testslib
-
 The following classes can be used to handle field test within a campaign.
 
 .. autosummary::
-    PumpingTest
+   :toctree:
+
+   PumpingTest
+   Test
 
 Variable classes
 ~~~~~~~~~~~~~~~~
 
-.. currentmodule:: welltestpy.data.varlib
-
 .. autosummary::
-    Variable
-    TimeVar
-    HeadVar
-    TemporalVar
-    CoordinatesVar
-    Observation
-    StdyObs
-    DrawdownObs
-    StdyHeadObs
-    Well
+   :toctree:
+
+   Variable
+   TimeVar
+   HeadVar
+   TemporalVar
+   CoordinatesVar
+   Observation
+   StdyObs
+   DrawdownObs
+   StdyHeadObs
+   Well
 
 Routines
 ^^^^^^^^
 
 Loading routines
 ~~~~~~~~~~~~~~~~
 
-.. currentmodule:: welltestpy.data.data_io
-
 Campaign related loading routines
 
 .. autosummary::
-    load_campaign
-    load_fieldsite
+   :toctree:
+
+   load_campaign
+   load_fieldsite
 
 Field test related loading routines
 
 .. autosummary::
-    load_test
+   :toctree:
+
+   load_test
 
 Variable related loading routines
 
 .. autosummary::
-    load_var
-    load_obs
-    load_well
-"""
-from . import varlib, testslib, campaignlib, data_io
+   :toctree:
 
+   load_var
+   load_obs
+   load_well
+"""
+from . import campaignlib, data_io, testslib, varlib
+from .campaignlib import Campaign, FieldSite
+from .data_io import (
+    load_campaign,
+    load_fieldsite,
+    load_obs,
+    load_test,
+    load_var,
+    load_well,
+)
+from .testslib import PumpingTest, Test
 from .varlib import (
-    Variable,
-    TimeVar,
-    HeadVar,
-    TemporalVar,
     CoordinatesVar,
-    Observation,
-    StdyObs,
     DrawdownObs,
+    HeadVar,
+    Observation,
     StdyHeadObs,
+    StdyObs,
+    TemporalVar,
+    TimeVar,
+    Variable,
     Well,
 )
-from .testslib import PumpingTest
-from .campaignlib import (
-    FieldSite,
-    Campaign,
-)
-from .data_io import (
-    load_var,
-    load_obs,
-    load_well,
-    load_campaign,
-    load_fieldsite,
-    load_test,
-)
 
 __all__ = [
     "Variable",
     "TimeVar",
     "HeadVar",
     "TemporalVar",
     "CoordinatesVar",
@@ -118,14 +104,15 @@
     "StdyObs",
     "DrawdownObs",
     "StdyHeadObs",
     "Well",
 ]
 __all__ += [
     "PumpingTest",
+    "Test",
 ]
 __all__ += [
     "FieldSite",
     "Campaign",
 ]
 __all__ += [
     "load_var",
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/data/campaignlib.py` & `welltestpy-1.2.0/src/welltestpy/data/campaignlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,21 @@
-# -*- coding: utf-8 -*-
-"""Welltestpy subpackage providing flow datastructures for field-campaigns.
-
-.. currentmodule:: welltestpy.data.campaignlib
-
-The following classes and functions are provided
-
-.. autosummary::
-   FieldSite
-   Campaign
-"""
+"""Welltestpy subpackage providing flow datastructures for field-campaigns."""
 from copy import deepcopy as dcopy
 
 from ..tools import plotter
-from . import data_io, varlib, testslib
+from . import data_io, testslib, varlib
 
 __all__ = ["FieldSite", "Campaign"]
 
 
 class FieldSite:
     """Class for a field site.
 
     This is a class for a field site.
-    It has a name and a descrition.
+    It has a name and a description.
 
     Parameters
     ----------
     name : :class:`str`
         Name of the field site.
     description : :class:`str`, optional
         Description of the field site.
@@ -195,15 +185,15 @@
                         )
                 self.__wells = {}
                 for wel in wells:
                     self.__wells[wel.name] = dcopy(wel)
             else:
                 raise ValueError(
                     "Campaign: 'wells' should be given "
-                    + "as dictonary or list"
+                    + "as dictionary or list"
                 )
         else:
             self.__wells = {}
         self.__updatewells()
 
     def add_well(
         self, name, radius, coordinates, welldepth=1.0, aquiferdepth=None
@@ -270,15 +260,15 @@
             for wel in wells:
                 self.__wells[wel.name] = dcopy(wel)
         elif isinstance(wells, varlib.Well):
             self.__wells[wells.name] = dcopy(wells)
         else:
             raise ValueError(
                 "Campaign_addwells: 'wells' should be "
-                + "given as dictonary, list or single 'Well'"
+                + "given as dictionary, list or single 'Well'"
             )
 
     def delwells(self, wells):
         """Delete some specified wells.
 
         This will delete wells from the campaign. You can give a
         list of wells or a single well by name.
@@ -326,15 +316,15 @@
                 for tes in tests:
                     self.__tests[tes.name] = dcopy(tes)
             elif isinstance(tests, testslib.Test):
                 self.__tests[tests.name] = dcopy(tests)
             else:
                 raise ValueError(
                     "Campaign: 'tests' should be given "
-                    + "as dictonary, list or 'Test'"
+                    + "as dictionary, list or 'Test'"
                 )
         else:
             self.__tests = {}
 
     def addtests(self, tests):
         """Add some specified tests.
 
@@ -381,15 +371,15 @@
         elif isinstance(tests, testslib.Test):
             if tests.name in tuple(self.__tests.keys()):
                 raise ValueError("Campaign.addtests: 'test' already present")
             self.__tests[tests.name] = dcopy(tests)
         else:
             raise ValueError(
                 "Campaign_addtests: 'tests' should be "
-                + "given as dictonary, list or single 'Test'"
+                + "given as dictionary, list or single 'Test'"
             )
 
     def deltests(self, tests):
         """Delete some specified tests.
 
         This will delete tests from the campaign. You can give a
         list of tests or a single test by name.
@@ -417,27 +407,27 @@
 
         Parameters
         ----------
         select_tests : :class:`list`, optional
             Tests that should be plotted. If None, all will be displayed.
             Default: ``None``
         **kwargs
-            Keyword-arguments forwarded to :any:`campaign_plot`
+            Keyword-arguments forwarded to :py:func:`~welltestpy.tools.campaign_plot`
         """
         return plotter.campaign_plot(self, select_tests, **kwargs)
 
     def plot_wells(self, **kwargs):
         """Generate a plot of the wells within the campaign.
 
         This will plot an overview of the wells within the campaign.
 
         Parameters
         ----------
         **kwargs
-            Keyword-arguments forwarded to :any:`campaign_well_plot`.
+            Keyword-arguments forwarded to :py:func:`~welltestpy.tools.campaign_well_plot`.
         """
         return plotter.campaign_well_plot(self, **kwargs)
 
     def diagnostic_plot(self, pumping_test, observation_well, **kwargs):
         """Generate a diagnostic plot.
 
         Parameters
@@ -445,15 +435,15 @@
         pumping_test : :class:`str`
             The pumping well that is saved in the campaign.
 
         observation_well : :class:`str`
             Observation point to make the diagnostic plot.
 
         **kwargs
-            Keyword-arguments forwarded to :any:`campaign_well_plot`.
+            Keyword-arguments forwarded to :py:func:`~welltestpy.tools.campaign_well_plot`.
         """
         # check if this is a pumping test
         if pumping_test in self.tests:
             if not isinstance(self.tests[pumping_test], testslib.PumpingTest):
                 raise ValueError(
                     f"diagnostic_plot: test '{pumping_test}' is not of instance PumpingTest!"
                 )
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/data/data_io.py` & `welltestpy-1.2.0/src/welltestpy/data/data_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,21 @@
-# -*- coding: utf-8 -*-
-"""
-welltestpy subpackage providing input-output routines.
-
-.. currentmodule:: welltestpy.data.data_io
-
-The following functions are provided
-
-.. autosummary::
-"""
-import os
+"""welltestpy subpackage providing input-output routines."""
 import csv
+import numbers
+import os
 import shutil
-import zipfile
 import tempfile
-from io import TextIOWrapper as TxtIO, BytesIO as BytIO
-import numbers
+import zipfile
+from io import BytesIO as BytIO
+from io import TextIOWrapper as TxtIO
+
 import numpy as np
 from packaging.version import parse as version_parse
 
-from . import varlib, campaignlib, testslib
+from . import campaignlib, testslib, varlib
 
 try:
     from .._version import __version__
 except ImportError:  # pragma: nocover
     # package is not installed
     __version__ = "0.0.0.dev0"
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/data/testslib.py` & `welltestpy-1.2.0/src/welltestpy/data/testslib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,24 @@
-# -*- coding: utf-8 -*-
-"""
-welltestpy subpackage providing flow datastructures for tests on a fieldsite.
-
-.. currentmodule:: welltestpy.data.testslib
-
-The following classes and functions are provided
-
-.. autosummary::
-   Test
-   PumpingTest
-"""
+"""welltestpy subpackage providing flow datastructures for tests on a fieldsite."""
 from copy import deepcopy as dcopy
 
 import numpy as np
 
-from ..tools import plotter, diagnostic_plots
-from . import varlib, data_io
 from ..process import processlib
+from ..tools import diagnostic_plots, plotter
+from . import data_io, varlib
 
 __all__ = ["Test", "PumpingTest"]
 
 
 class Test:
     """General class for a well based test.
 
     This is a class for a well based test on a field site.
-    It has a name, a descrition and a timeframe string.
+    It has a name, a description and a timeframe string.
 
     Parameters
     ----------
     name : :class:`str`
         Name of the test.
     description : :class:`str`, optional
         Description of the test.
@@ -62,15 +51,15 @@
         This will plot the test on the given figure axes.
 
         Parameters
         ----------
         ax : :class:`Axes`
             Axes where the plot should be done.
         wells : :class:`dict`
-            Dictonary containing the well classes sorted by name.
+            Dictionary containing the well classes sorted by name.
         exclude: :class:`list`, optional
             List of wells that should be excluded from the plot.
             Default: ``None``
 
         Notes
         -----
         This will be used by the Campaign class.
@@ -79,15 +68,15 @@
         return ax
 
 
 class PumpingTest(Test):
     """Class for a pumping test.
 
     This is a class for a pumping test on a field site.
-    It has a name, a descrition, a timeframe and a pumpingwell string.
+    It has a name, a description, a timeframe and a pumpingwell string.
 
     Parameters
     ----------
     name : :class:`str`
         Name of the test.
     pumpingwell : :class:`str`
         Pumping well of the test.
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/data/varlib.py` & `welltestpy-1.2.0/src/welltestpy/data/varlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,15 @@
-# -*- coding: utf-8 -*-
-"""
-welltestpy subpackage providing flow datastructures for variables.
-
-.. currentmodule:: welltestpy.data.varlib
-
-The following classes and functions are provided
-
-.. autosummary::
-   Variable
-   TimeVar
-   HeadVar
-   TemporalVar
-   CoordinatesVar
-   Observation
-   StdyObs
-   DrawdownObs
-   StdyHeadObs
-   TimeSeries
-   Well
-"""
-from copy import deepcopy as dcopy
+"""welltestpy subpackage providing flow datastructures for variables."""
 import numbers
+from copy import deepcopy as dcopy
+
 import numpy as np
 
 from . import data_io
 
-
 __all__ = [
     "Variable",
     "TimeVar",
     "HeadVar",
     "TemporalVar",
     "CoordinatesVar",
     "Observation",
@@ -284,15 +264,15 @@
 
 
 class Observation:
     """
     Class for a observation.
 
     This is a class for time-dependent observations.
-    It has a name and a descrition.
+    It has a name and a description.
 
     Parameters
     ----------
     name : :class:`str`
         Name of the Variable.
     observation : :class:`Variable`
         Name of the Variable. Default: ``"x"``
@@ -341,19 +321,19 @@
         if time is not None:
             self._settime(time)
         if observation is not None or time is not None:
             self._checkshape()
         return self.value
 
     def __repr__(self):
-        """Represenetation."""
+        """Representation."""
         return f"Observation '{self.name}' {self.label}"
 
     def __str__(self):
-        """Represenetation."""
+        """Representation."""
         return self.__repr__()
 
     @property
     def labels(self):
         """[:class:`tuple` of] :class:`str`: ``symbol in units``."""
         if self.state == "transient":
             return self._time.label, self._observation.label
@@ -362,17 +342,17 @@
     @property
     def label(self):
         """[:class:`tuple` of] :class:`str`: ``symbol in units``."""
         return self.labels
 
     @property
     def info(self):
-        """Get informations about the observation.
+        """Get information about the observation.
 
-        Here you can display informations about the observation.
+        Here you can display information about the observation.
         """
         info = ""
         info += "Observation-name: " + str(self.name) + "\n"
         info += " -Description:    " + str(self.description) + "\n"
         info += " -Kind:           " + str(self.kind) + "\n"
         info += " -State:          " + str(self.state) + "\n"
         if self.state == "transient":
@@ -444,15 +424,15 @@
     def units(self):
         """[:class:`tuple` of] :class:`str`: units of the observation."""
         if self.state == "steady":
             return self._observation.units
         return f"{self._time.units}, {self._observation.units}"
 
     def reshape(self):
-        """Reshape obeservations to flat array."""
+        """Reshape observations to flat array."""
         if self.state == "transient":
             tmp = len(np.shape(self.time))
             self._settime(np.reshape(self.time, -1))
             shp = np.shape(self.time) + np.shape(self.observation)[tmp:]
             self._setobservation(np.reshape(self.observation, shp))
 
     def _settime(self, time):
@@ -475,15 +455,15 @@
 
     def _checkshape(self):
         if self.state == "transient" and (
             np.shape(self.time)
             != np.shape(self.observation)[: len(np.shape(self.time))]
         ):
             raise ValueError(
-                "Observation: 'observation' has a shape-missmatch with 'time'"
+                "Observation: 'observation' has a shape-mismatch with 'time'"
             )
 
     def __iter__(self):
         """Iterate over Observations."""
         if self.state == "transient":
             self.__it = np.nditer(self.time, flags=["multi_index"])
         else:
@@ -548,15 +528,15 @@
         """For steady observations, this raises a ``ValueError``."""
         if time is not None:
             raise ValueError("Observation: 'time' not allowed in steady-state")
 
 
 class TimeSeries(Observation):
     """
-    Time series obeservation.
+    Time series observation.
 
     Parameters
     ----------
     name : :class:`str`
         Name of the Variable.
     values : :class:`Variable`
         Values of the time-series.
@@ -680,17 +660,17 @@
         self.coordinates = coordinates
         self.welldepth = welldepth
         self.aquiferdepth = aquiferdepth
         self.screensize = screensize
 
     @property
     def info(self):
-        """Get informations about the variable.
+        """Get information about the variable.
 
-        Here you can display informations about the variable.
+        Here you can display information about the variable.
         """
         info = ""
         info += "----\n"
         info += "Well-name: " + str(self.name) + "\n"
         info += "--\n"
         info += self._radius.info + "\n"
         info += self.coordinates.info + "\n"
@@ -723,15 +703,15 @@
                 f"Inner radius of well '{self.name}'",
             )
         else:
             self._radius(radius)
         if not self._radius.scalar:
             raise ValueError("Well: 'radius' needs to be scalar")
         if not self.radius > 0.0:
-            raise ValueError("Well: 'radius' needs to be positiv")
+            raise ValueError("Well: 'radius' needs to be positive")
 
     @property
     def pos(self):
         """:class:`numpy.ndarray`: Position of the well."""
         return self._coordinates.value
 
     @property
@@ -782,15 +762,15 @@
                 f"depth of well '{self.name}'",
             )
         else:
             self._welldepth(welldepth)
         if not self._welldepth.scalar:
             raise ValueError("Well: 'welldepth' needs to be scalar")
         if not self.depth > 0.0:
-            raise ValueError("Well: 'welldepth' needs to be positiv")
+            raise ValueError("Well: 'welldepth' needs to be positive")
 
     @property
     def aquifer(self):
         """:class:`float`: Aquifer depth at the well."""
         return self._aquiferdepth.value
 
     @property
@@ -811,15 +791,15 @@
                 f"aquifer depth at well '{self.name}'",
             )
         else:
             self._aquiferdepth(aquiferdepth)
         if not self._aquiferdepth.scalar:
             raise ValueError("Well: 'aquiferdepth' needs to be scalar")
         if not self.aquifer > 0.0:
-            raise ValueError("Well: 'aquiferdepth' needs to be positiv")
+            raise ValueError("Well: 'aquiferdepth' needs to be positive")
 
     @property
     def is_piezometer(self):
         """:class:`bool`: Whether the well is only a standpipe piezometer."""
         return np.isclose(self.screen, 0)
 
     @property
@@ -863,21 +843,21 @@
             return np.linalg.norm(self.pos - well.pos)
         try:
             return np.linalg.norm(self.pos - well)
         except ValueError:
             raise ValueError(
                 "Well: the distant-well needs to be an "
                 "instance of Well-class "
-                "or a tupel of x-y coordinates "
+                "or a tuple of x-y coordinates "
                 "or a single distance value "
                 "and of same coordinates-type."
             )
 
     def __repr__(self):
-        """Represenetation."""
+        """Representation."""
         return f"{self.name} r={self.radius} at {self._coordinates}"
 
     def __sub__(self, well):
         """Distance between wells."""
         return self.distance(well)
 
     def __add__(self, well):
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/estimate/__init__.py` & `welltestpy-1.2.0/src/welltestpy/estimate/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,80 @@
-# -*- coding: utf-8 -*-
 """
 welltestpy subpackage providing routines to estimate pump test parameters.
 
 .. currentmodule:: welltestpy.estimate
 
 Estimators
 ^^^^^^^^^^
 
 The following estimators are provided
 
 .. autosummary::
-    ExtTheis3D
-    ExtTheis2D
-    Neuman2004
-    Theis
-    ExtThiem3D
-    ExtThiem2D
-    Neuman2004Steady
-    Thiem
+   :toctree:
 
+   ExtTheis3D
+   ExtTheis2D
+   Neuman2004
+   Theis
+   ExtThiem3D
+   ExtThiem2D
+   Neuman2004Steady
+   Thiem
 
 Base Classes
 ^^^^^^^^^^^^
 
 Transient
 ~~~~~~~~~
 
 All transient estimators are derived from the following class
 
 .. autosummary::
+   :toctree:
+
    TransientPumping
 
 Steady Pumping
 ~~~~~~~~~~~~~~
 
 All steady estimators are derived from the following class
 
 .. autosummary::
+   :toctree:
+
    SteadyPumping
+
+Helper
+^^^^^^
+
+.. autosummary::
+   :toctree:
+
+   fast_rep
 """
 from . import estimators, spotpylib, steady_lib, transient_lib
-
 from .estimators import (
-    ExtTheis3D,
     ExtTheis2D,
-    Neuman2004,
-    Theis,
-    ExtThiem3D,
+    ExtTheis3D,
     ExtThiem2D,
+    ExtThiem3D,
+    Neuman2004,
     Neuman2004Steady,
+    Theis,
     Thiem,
 )
-from .transient_lib import TransientPumping
+from .spotpylib import fast_rep
 from .steady_lib import SteadyPumping
+from .transient_lib import TransientPumping
 
 __all__ = ["estimators", "spotpylib", "steady_lib", "transient_lib"]
 __all__ += [
     "ExtTheis3D",
     "ExtTheis2D",
     "Neuman2004",
     "Theis",
     "ExtThiem3D",
     "ExtThiem2D",
     "Neuman2004Steady",
     "Thiem",
 ]
-__all__ += ["TransientPumping", "SteadyPumping"]
+__all__ += ["TransientPumping", "SteadyPumping", "fast_rep"]
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/estimate/spotpylib.py` & `welltestpy-1.2.0/src/welltestpy/estimate/spotpylib.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 welltestpy subpackage providing Spotpy classes for the estimating.
 
 .. currentmodule:: welltestpy.estimate.spotpylib
 
 The following functions and classes are provided
 
@@ -11,92 +10,104 @@
    fast_rep
 """
 import functools as ft
 
 import numpy as np
 import spotpy
 
-
 __all__ = ["TypeCurve", "fast_rep"]
 
 
-# functions for fitting
+def _quad(x):
+    return np.power(x, 2)
+
+
+def _inv(x):
+    return 1.0 / x
+
+
+def _lin(x):
+    return x
+
+
 FIT = {
-    "linear": lambda x: x,
-    "lin": lambda x: x,
-    "logarithmic": np.exp,
-    "log": np.exp,
-    "exponential": np.log,
-    "exp": np.log,
-    "squareroot": lambda x: np.power(x, 2),
-    "sqrt": lambda x: np.power(x, 2),
-    "quadratic": np.sqrt,
-    "quad": np.sqrt,
-    "inverse": lambda x: 1.0 / x,
-    "inv": lambda x: 1.0 / x,
+    "lin": (_lin, _lin),
+    "log": (np.log, np.exp),
+    "exp": (np.exp, np.log),
+    "sqrt": (np.sqrt, _quad),
+    "quad": (_quad, np.sqrt),
+    "inv": (_inv, _inv),
 }
+"""dict: all predefined fitting transformations and their inverse."""
+
+
+def _is_callable_tuple(input):
+    result = False
+    length = 0
+    try:
+        length = len(input)
+    except TypeError:
+        length = -1
+    finally:
+        if length == 2:
+            result = all(map(callable, input))
+    return result
 
 
 def fast_rep(para_no, infer_fac=4, freq_step=2):
     """Get number of iterations needed for the FAST algorithm.
 
     Parameters
     ----------
     para_no : :class:`int`
         Number of parameters in the model.
     infer_fac : :class:`int`, optional
-        The inference fractor. Default: 4
+        The inference factor. Default: 4
     freq_step : :class:`int`, optional
         The frequency step. Default: 2
     """
     return 2 * int(
-        para_no * (1 + 4 * infer_fac ** 2 * (1 + (para_no - 2) * freq_step))
+        para_no * (1 + 4 * infer_fac**2 * (1 + (para_no - 2) * freq_step))
     )
 
 
 class TypeCurve:
     r"""Spotpy class for an estimation of subsurface parameters.
 
     This class fits a given Type Curve to given data.
-    Values will be sampled uniformly in given ranges.
-
-    Fitting values will be done linear, logarithmic or by user specified
-    function.
+    Values will be sampled uniformly in given ranges and with given transformation.
 
     Parameters
     ----------
     type_curve : :any:`callable`
         The given type-curve. Output will be reshaped to flat array.
     data : :class:`numpy.ndarray`
         Observed data as array. Will be reshaped to flat array.
     val_ranges : :class:`dict`
         Dictionary containing the fit-ranges for each value in the type-curve.
-        Names should be as in the type-curve signiture
-        or replaced in val_kw_names.
-        Ranges should be a tuple containing min and max value.
+        Names should be as in the type-curve signature.
+        All values to be estimated should be present here.
+        Ranges should be a tuple containing min and max value: ``(min, max)``.
     val_fix : :class:`dict` or :any:`None`
         Dictionary containing fixed values for the type-curve.
-        Names should be as in the type-curve signiture
-        or replaced in val_kw_names.
+        Names should be as in the type-curve signature.
         Default: None
-    fit_type : :class:`dict` or :any:`None`
-        Dictionary containing fitting type for each value in the type-curve.
-        Names should be as in the type-curve signiture
-        or replaced in val_kw_names.
-        fit_type can be "lin", "log" (np.exp(val) will be used)
-        or a callable function.
-        By default, values will be fit linearly.
+    val_fit_type : :class:`dict` or :any:`None`
+        Dictionary containing fitting transformation type for each value.
+        Names should be as in the type-curve signature.
+        val_fit_type can be "lin", "log", "exp", "sqrt", "quad", "inv"
+        or a tuple of two callable functions where the
+        first is the transformation and the second is its inverse.
+        "log" is for example equivalent to ``(np.log, np.exp)``.
+        By default, values will be fitted linear.
         Default: None
-    val_kw_names : :class:`dict` or :any:`None`
-        Dictionary containing keyword names in the type-curve for each value.
-
-            {value-name: kwargs-name in type_curve}
-
-        This is usefull if fitting is not done by linear values.
-        By default, parameter names will be value names.
+    val_fit_name : :class:`dict` or :any:`None`
+        Display name of the fitting transformation.
+        Will be the val_fit_type string if it is a predefined one,
+        or ``f`` if it is a given callable as default for each value.
         Default: None
     val_plot_names : :class:`dict` or :any:`None`
         Dictionary containing plotable strings for the parameters.
 
             {value-name: plotting-string}
 
         Default: None
@@ -108,78 +119,82 @@
 
     def __init__(
         self,
         type_curve,
         data,
         val_ranges,
         val_fix=None,
-        fit_type=None,
-        val_kw_names=None,
+        val_fit_type=None,
+        val_fit_name=None,
         val_plot_names=None,
         dummy=False,
     ):
         self.func = type_curve
-        assert callable(self.func), "type_curve not callable"
-        self.fit_type = {} if fit_type is None else fit_type
-        self.val_kw_names = {} if val_kw_names is None else val_kw_names
-        self.val_plot_names = {} if val_plot_names is None else val_plot_names
-        self.val_ranges = val_ranges
-        assert self.val_ranges, "No ranges given"
-        self.val_fix = {} if val_fix is None else val_fix
-        self.val_fix_kw = {}
-        for fix in self.val_fix:
-            name = self.val_kw_names.get(fix, fix)
-            fit_fix = self.fit_type.get(fix, "lin")
-            fit_fix = fit_fix if callable(fit_fix) else FIT[fit_fix]
-            self.val_fix_kw[name] = fit_fix(self.val_fix[fix])
+        if not callable(self.func):
+            raise ValueError("type_curve not callable")
+        self.val_fit_type = val_fit_type or {}
+        self.val_plot_names = val_plot_names or {}
+        if not isinstance(val_ranges, dict) or not val_ranges:
+            raise ValueError("No ranges given")
+        self.val_ranges = val_ranges.copy()
+        self.val_fix = val_fix or {}
         # if values haven given ranges but should be fixed, remove ranges
         for inter in set(self.val_ranges) & set(self.val_fix):
             del self.val_ranges[inter]
 
-        self.para_names = list(val_ranges)
+        self.para_names = list(self.val_ranges)
         self.para_dist = []
         self.data = np.array(data, dtype=float).reshape(-1)
         self.sim_kwargs = {}
         self.fit_func = {}
-
+        self.val_fit_name = val_fit_name or {}
         for val in self.para_names:
+            # linear fitting by default
+            fit_t = self.val_fit_type.get(val, "lin")
+            fit_n = fit_t if fit_t in FIT else "f"
+            self.val_fit_name.setdefault(
+                val, fit_n if fit_n != "lin" else None
+            )
+            self.fit_func[val] = (
+                fit_t if _is_callable_tuple(fit_t) else FIT.get(fit_t, None)
+            )
+            if not self.fit_func[val]:
+                raise ValueError(f"Fitting transformation for '{val}' missing")
+            # apply fitting transformation to ranges
             self.para_dist.append(
-                spotpy.parameter.Uniform(val, *self.val_ranges[val])
+                spotpy.parameter.Uniform(
+                    val, *map(self.fit_func[val][0], self.val_ranges[val])
+                )
             )
-            fit_t = self.fit_type.get(val, "lin")
-            self.fit_func[val] = fit_t if callable(fit_t) else FIT[fit_t]
-            self.val_kw_names.setdefault(val, val)
             self.val_plot_names.setdefault(val, val)
 
         self.dummy = dummy
         if self.dummy:
             self.para_dist.append(spotpy.parameter.Uniform("dummy", 0, 1))
 
-        self.sim = ft.partial(self.func, **self.val_fix_kw)
+        self.sim = ft.partial(self.func, **self.val_fix)
 
     def get_sim_kwargs(self, vector):
         """Generate keyword-args for simulation."""
         # if there is a dummy parameter it will be skipped automatically
         for i, para in enumerate(self.para_names):
-            self.sim_kwargs[self.val_kw_names[para]] = self.fit_func[para](
-                vector[i]
-            )
+            self.sim_kwargs[para] = self.fit_func[para][1](vector[i])
         return self.sim_kwargs
 
     def parameters(self):
         """Generate a set of parameters."""
         return spotpy.parameter.generate(self.para_dist)
 
     def simulation(self, vector):
         """Run a simulation with the given parameters."""
         self.get_sim_kwargs(vector)
         return self.sim(**self.sim_kwargs).reshape(-1)
 
     def evaluation(self):
-        """Accesss the observation data."""
+        """Access the observation data."""
         return self.data
 
     def objectivefunction(self, simulation, evaluation):
         """Calculate RMSE between observation and simulation."""
         return spotpy.objectivefunctions.rmse(
             evaluation=evaluation, simulation=simulation
         )
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/estimate/steady_lib.py` & `welltestpy-1.2.0/src/welltestpy/estimate/steady_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,19 @@
-# -*- coding: utf-8 -*-
-"""
-welltestpy subpackage providing base classe for steady state estimations.
-
-.. currentmodule:: welltestpy.estimate.steady_lib
-
-The following classes are provided
-
-.. autosummary::
-   SteadyPumping
-"""
-from copy import deepcopy as dcopy
+"""welltestpy subpackage providing base classes for steady state estimations."""
 import os
 import time as timemodule
+from copy import deepcopy as dcopy
 
 import numpy as np
 import spotpy
 
 from ..data import testslib
 from ..process import processlib
-from . import spotpylib
 from ..tools import plotter
+from . import spotpylib
 
 __all__ = [
     "SteadyPumping",
 ]
 
 
 class SteadyPumping:
@@ -31,57 +21,53 @@
 
     Parameters
     ----------
     name : :class:`str`
         Name of the Estimation.
     campaign : :class:`welltestpy.data.Campaign`
         The pumping test campaign which should be used to estimate the
-        paramters
+        parameters
     type_curve : :any:`callable`
         The given type-curve. Output will be reshaped to flat array.
     val_ranges : :class:`dict`
         Dictionary containing the fit-ranges for each value in the type-curve.
-        Names should be as in the type-curve signiture
-        or replaced in val_kw_names.
+        Names should be as in the type-curve signature.
         Ranges should be a tuple containing min and max value.
     make_steady : :class:`bool`, optional
         State if the tests should be converted to steady observations.
         See: :any:`PumpingTest.make_steady`.
         Default: True
     val_fix : :class:`dict` or :any:`None`
         Dictionary containing fixed values for the type-curve.
-        Names should be as in the type-curve signiture
-        or replaced in val_kw_names.
+        Names should be as in the type-curve signature.
         Default: None
-    fit_type : :class:`dict` or :any:`None`
-        Dictionary containing fitting type for each value in the type-curve.
-        Names should be as in the type-curve signiture
-        or replaced in val_kw_names.
-        fit_type can be "lin", "log" (np.exp(val) will be used)
-        or a callable function.
-        By default, values will be fit linearly.
+    val_fit_type : :class:`dict` or :any:`None`
+        Dictionary containing fitting transformation type for each value.
+        Names should be as in the type-curve signature.
+        val_fit_type can be "lin", "log", "exp", "sqrt", "quad", "inv"
+        or a tuple of two callable functions where the
+        first is the transformation and the second is its inverse.
+        "log" is for example equivalent to ``(np.log, np.exp)``.
+        By default, values will be fitted linear.
         Default: None
-    val_kw_names : :class:`dict` or :any:`None`
-        Dictionary containing keyword names in the type-curve for each value.
-
-            {value-name: kwargs-name in type_curve}
-
-        This is usefull if fitting is not done by linear values.
-        By default, parameter names will be value names.
+    val_fit_name : :class:`dict` or :any:`None`
+        Display name of the fitting transformation.
+        Will be the val_fit_type string if it is a predefined one,
+        or ``f`` if it is a given callable as default for each value.
         Default: None
     val_plot_names : :class:`dict` or :any:`None`
         Dictionary containing keyword names in the type-curve for each value.
 
             {value-name: string for plot legend}
 
-        This is usefull to get better plots.
+        This is useful to get better plots.
         By default, parameter names will be value names.
         Default: None
     testinclude : :class:`dict`, optional
-        dictonary of which tests should be included. If ``None`` is given,
+        Dictionary of which tests should be included. If ``None`` is given,
         all available tests are included.
         Default: ``None``
     generate : :class:`bool`, optional
         State if time stepping, processed observation data and estimation
         setup should be generated with default values.
         Default: ``False``
     """
@@ -90,30 +76,27 @@
         self,
         name,
         campaign,
         type_curve,
         val_ranges,
         make_steady=True,
         val_fix=None,
-        fit_type=None,
-        val_kw_names=None,
+        val_fit_type=None,
+        val_fit_name=None,
         val_plot_names=None,
         testinclude=None,
         generate=False,
     ):
         val_fix = {} if val_fix is None else val_fix
-        fit_type = {} if fit_type is None else fit_type
-        val_kw_names = {} if val_kw_names is None else val_kw_names
-        val_plot_names = {} if val_plot_names is None else val_plot_names
         self.setup_kw = {
             "type_curve": type_curve,
             "val_ranges": val_ranges,
             "val_fix": val_fix,
-            "fit_type": fit_type,
-            "val_kw_names": val_kw_names,
+            "val_fit_type": val_fit_type,
+            "val_fit_name": val_fit_name,
             "val_plot_names": val_plot_names,
         }
         """:class:`dict`: TypeCurve Spotpy Setup definition"""
         self.name = name
         """:class:`str`: Name of the Estimation"""
         self.campaign_raw = dcopy(campaign)
         """:class:`welltestpy.data.Campaign`:\
@@ -139,15 +122,15 @@
         self.estimated_para = {}
         """:class:`dict`: estimated parameters by name"""
         self.result = None
         """:class:`list`: result of the spotpy estimation"""
         self.sens = None
         """:class:`dict`: result of the spotpy sensitivity analysis"""
         self.testinclude = {}
-        """:class:`dict`: dictonary of which tests should be included"""
+        """:class:`dict`: dictionary of which tests should be included"""
 
         if testinclude is None:
             tests = list(self.campaign.tests.keys())
             self.testinclude = {}
             for test in tests:
                 self.testinclude[test] = self.campaign.tests[
                     test
@@ -271,27 +254,23 @@
             Keyword name for the reference head in the used type curve.
             Default: "h_ref"
         dummy : :class:`bool`, optional
             Add a dummy parameter to the model. This could be used to equalize
             sensitivity analysis.
             Default: False
         """
-        self.extra_kw_names = {
-            "Qw": prate_kw,
-            "rad": rad_kw,
-            "r_ref": r_ref_kw,
-            "h_ref": h_ref_kw,
-        }
-        self.setup_kw["val_fix"].setdefault(prate_kw, self.prate)
-        self.setup_kw["val_fix"].setdefault(rad_kw, self.rad)
-        self.setup_kw["val_fix"].setdefault(r_ref_kw, self.r_ref)
-        self.setup_kw["val_fix"].setdefault(h_ref_kw, self.h_ref)
-        self.setup_kw.setdefault("data", self.data)
-        self.setup_kw["dummy"] = dummy
-        self.setup = spotpylib.TypeCurve(**self.setup_kw)
+        self.extra_kw_names = {"rad": rad_kw}
+        setup_kw = dcopy(self.setup_kw)  # create a copy here
+        setup_kw["val_fix"].setdefault(prate_kw, self.prate)
+        setup_kw["val_fix"].setdefault(rad_kw, self.rad)
+        setup_kw["val_fix"].setdefault(r_ref_kw, self.r_ref)
+        setup_kw["val_fix"].setdefault(h_ref_kw, self.h_ref)
+        setup_kw.setdefault("data", self.data)
+        setup_kw["dummy"] = dummy
+        self.setup = spotpylib.TypeCurve(**setup_kw)
 
     def run(
         self,
         rep=5000,
         parallel="seq",
         run=True,
         folder=None,
@@ -346,20 +325,20 @@
             Default: ``None``
         estname : :class:`str`, optional
             File-name of the results of the spotpy estimation.
             If ``None``, it will be the current time +
             ``"_estimate"``.
             Default: ``None``
         plot_style : str, optional
-            Plot stlye. The default is "WTP".
+            Plot style. The default is "WTP".
         """
         if self.setup.dummy:
             raise ValueError(
                 "Estimate: for parameter estimation"
-                " you can't use a dummy paramter."
+                " you can't use a dummy parameter."
             )
         act_time = timemodule.strftime("%Y-%m-%d_%H-%M-%S")
 
         # generate the filenames
         if folder is None:
             folder = os.path.join(os.getcwd(), self.name)
         folder = os.path.abspath(folder)
@@ -385,15 +364,19 @@
         if estname is None:
             paraname = os.path.join(folder, act_time + "_estimate.txt")
         elif not os.path.isabs(estname):
             paraname = os.path.join(folder, estname)
 
         # generate the parameter-names for plotting
         paranames = dcopy(self.setup.para_names)
-        paralabels = [self.setup.val_plot_names[name] for name in paranames]
+        paralabels = []
+        for name in paranames:
+            p_label = self.setup.val_plot_names[name]
+            fit_n = self.setup.val_fit_name[name]
+            paralabels.append(f"{fit_n}({p_label})" if fit_n else p_label)
 
         if parallel == "mpi":
             # send the dbname of rank0
             from mpi4py import MPI
 
             comm = MPI.COMM_WORLD
             rank = comm.Get_rank()
@@ -432,16 +415,17 @@
                 self.result, maximize=False
             )
             void_names = para_opt.dtype.names
             para = []
             header = []
             for name in void_names:
                 para.append(para_opt[0][name])
-                header.append(name[3:])
-                self.estimated_para[header[-1]] = para[-1]
+                fit_n = self.setup.val_fit_name[name[3:]]
+                header.append(f"{fit_n}-{name[3:]}" if fit_n else name[3:])
+                self.estimated_para[name[3:]] = para[-1]
             np.savetxt(paraname, para, header=" ".join(header))
             # plot the estimation-results
             plotter.plotparatrace(
                 result=self.result,
                 parameternames=paranames,
                 parameterlabels=paralabels,
                 stdvalues=self.estimated_para,
@@ -508,20 +492,20 @@
             Default: ``None``
         sensname : :class:`str`, optional
             File-name of the results of the FAST estimation.
             If ``None``, it will be the current time +
             ``"_estimate"``.
             Default: ``None``
         plot_style : str, optional
-            Plot stlye. The default is "WTP".
+            Plot style. The default is "WTP".
         """
         if len(self.setup.para_names) == 1 and not self.setup.dummy:
             raise ValueError(
                 "Sensitivity: for estimation with only one parameter"
-                " you have to use a dummy paramter."
+                " you have to use a dummy parameter."
             )
         if rep is None:
             rep = spotpylib.fast_rep(
                 len(self.setup.para_names) + int(self.setup.dummy)
             )
 
         act_time = timemodule.strftime("%Y-%m-%d_%H-%M-%S")
@@ -550,15 +534,19 @@
             sensname = os.path.join(folder, sensname)
 
         sens_base, sens_ext = os.path.splitext(sensname)
         sensname1 = sens_base + "_S1" + sens_ext
 
         # generate the parameter-names for plotting
         paranames = dcopy(self.setup.para_names)
-        paralabels = [self.setup.val_plot_names[name] for name in paranames]
+        paralabels = []
+        for name in paranames:
+            p_label = self.setup.val_plot_names[name]
+            fit_n = self.setup.val_fit_name[name]
+            paralabels.append(f"{fit_n}({p_label})" if fit_n else p_label)
 
         if self.setup.dummy:
             paranames.append("dummy")
             paralabels.append("dummy")
 
         if parallel == "mpi":
             # send the dbname of rank0
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/estimate/transient_lib.py` & `welltestpy-1.2.0/src/welltestpy/estimate/transient_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,20 @@
-# -*- coding: utf-8 -*-
-"""
-welltestpy subpackage providing base classe for transient estimations.
-
-.. currentmodule:: welltestpy.estimate.transient_lib
-
-The following classes are provided
-
-.. autosummary::
-   TransientPumping
-"""
-from copy import deepcopy as dcopy
+"""welltestpy subpackage providing base classes for transient estimations."""
 import os
 import time as timemodule
+from copy import deepcopy as dcopy
 
+import anaflow as ana
 import numpy as np
 import spotpy
-import anaflow as ana
 
 from ..data import testslib
 from ..process import processlib
-from . import spotpylib
 from ..tools import plotter
+from . import spotpylib
 
 __all__ = [
     "TransientPumping",
 ]
 
 
 class TransientPumping:
@@ -32,53 +22,49 @@
 
     Parameters
     ----------
     name : :class:`str`
         Name of the Estimation.
     campaign : :class:`welltestpy.data.Campaign`
         The pumping test campaign which should be used to estimate the
-        paramters
+        parameters
     type_curve : :any:`callable`
         The given type-curve. Output will be reshaped to flat array.
     val_ranges : :class:`dict`
         Dictionary containing the fit-ranges for each value in the type-curve.
-        Names should be as in the type-curve signiture
-        or replaced in val_kw_names.
+        Names should be as in the type-curve signature.
         Ranges should be a tuple containing min and max value.
     val_fix : :class:`dict` or :any:`None`
         Dictionary containing fixed values for the type-curve.
-        Names should be as in the type-curve signiture
-        or replaced in val_kw_names.
+        Names should be as in the type-curve signature.
         Default: None
-    fit_type : :class:`dict` or :any:`None`
-        Dictionary containing fitting type for each value in the type-curve.
-        Names should be as in the type-curve signiture
-        or replaced in val_kw_names.
-        fit_type can be "lin", "log" (np.exp(val) will be used)
-        or a callable function.
-        By default, values will be fit linearly.
+    val_fit_type : :class:`dict` or :any:`None`
+        Dictionary containing fitting transformation type for each value.
+        Names should be as in the type-curve signature.
+        val_fit_type can be "lin", "log", "exp", "sqrt", "quad", "inv"
+        or a tuple of two callable functions where the
+        first is the transformation and the second is its inverse.
+        "log" is for example equivalent to ``(np.log, np.exp)``.
+        By default, values will be fitted linear.
         Default: None
-    val_kw_names : :class:`dict` or :any:`None`
-        Dictionary containing keyword names in the type-curve for each value.
-
-            {value-name: kwargs-name in type_curve}
-
-        This is usefull if fitting is not done by linear values.
-        By default, parameter names will be value names.
+    val_fit_name : :class:`dict` or :any:`None`
+        Display name of the fitting transformation.
+        Will be the val_fit_type string if it is a predefined one,
+        or ``f`` if it is a given callable as default for each value.
         Default: None
     val_plot_names : :class:`dict` or :any:`None`
         Dictionary containing keyword names in the type-curve for each value.
 
             {value-name: string for plot legend}
 
-        This is usefull to get better plots.
+        This is useful to get better plots.
         By default, parameter names will be value names.
         Default: None
     testinclude : :class:`dict`, optional
-        dictonary of which tests should be included. If ``None`` is given,
+        Dictionary of which tests should be included. If ``None`` is given,
         all available tests are included.
         Default: ``None``
     generate : :class:`bool`, optional
         State if time stepping, processed observation data and estimation
         setup should be generated with default values.
         Default: ``False``
     """
@@ -86,30 +72,27 @@
     def __init__(
         self,
         name,
         campaign,
         type_curve,
         val_ranges,
         val_fix=None,
-        fit_type=None,
-        val_kw_names=None,
+        val_fit_type=None,
+        val_fit_name=None,
         val_plot_names=None,
         testinclude=None,
         generate=False,
     ):
-        val_fix = {} if val_fix is None else val_fix
-        fit_type = {} if fit_type is None else fit_type
-        val_kw_names = {} if val_kw_names is None else val_kw_names
-        val_plot_names = {} if val_plot_names is None else val_plot_names
+        val_fix = val_fix or {}
         self.setup_kw = {
             "type_curve": type_curve,
             "val_ranges": val_ranges,
             "val_fix": val_fix,
-            "fit_type": fit_type,
-            "val_kw_names": val_kw_names,
+            "val_fit_type": val_fit_type,
+            "val_fit_name": val_fit_name,
             "val_plot_names": val_plot_names,
         }
         """:class:`dict`: TypeCurve Spotpy Setup definition"""
         self.name = name
         """:class:`str`: Name of the Estimation"""
         self.campaign_raw = dcopy(campaign)
         """:class:`welltestpy.data.Campaign`:\
@@ -133,15 +116,15 @@
         self.estimated_para = {}
         """:class:`dict`: estimated parameters by name"""
         self.result = None
         """:class:`list`: result of the spotpy estimation"""
         self.sens = None
         """:class:`dict`: result of the spotpy sensitivity analysis"""
         self.testinclude = {}
-        """:class:`dict`: dictonary of which tests should be included"""
+        """:class:`dict`: dictionary of which tests should be included"""
 
         if testinclude is None:
             tests = list(self.campaign.tests.keys())
             self.testinclude = {}
             for test in tests:
                 self.testinclude[test] = self.campaign.tests[
                     test
@@ -204,15 +187,15 @@
     def settime(self, time=None, tmin=10.0, tmax=np.inf, typ="quad", steps=10):
         """Set uniform time points for the observations.
 
         Parameters
         ----------
         time : :class:`numpy.ndarray`, optional
             Array of specified time points. If ``None`` is given, they will
-            be determind by the observation data.
+            be determined by the observation data.
             Default: ``None``
         tmin : :class:`float`, optional
             Minimal time value. It will set a minimal value of 10s.
             Default: ``10``
         tmax : :class:`float`, optional
             Maximal time value.
             Default: ``inf``
@@ -307,21 +290,22 @@
             Keyword name for the time in the used type curve.
             Default: "time"
         dummy : :class:`bool`, optional
             Add a dummy parameter to the model. This could be used to equalize
             sensitivity analysis.
             Default: False
         """
-        self.extra_kw_names = {"Qw": prate_kw, "rad": rad_kw, "time": time_kw}
-        self.setup_kw["val_fix"].setdefault(prate_kw, self.prate)
-        self.setup_kw["val_fix"].setdefault(rad_kw, self.rad)
-        self.setup_kw["val_fix"].setdefault(time_kw, self.time)
-        self.setup_kw.setdefault("data", self.data)
-        self.setup_kw["dummy"] = dummy
-        self.setup = spotpylib.TypeCurve(**self.setup_kw)
+        self.extra_kw_names = {"rad": rad_kw, "time": time_kw}
+        setup_kw = dcopy(self.setup_kw)
+        setup_kw["val_fix"].setdefault(prate_kw, self.prate)
+        setup_kw["val_fix"].setdefault(rad_kw, self.rad)
+        setup_kw["val_fix"].setdefault(time_kw, self.time)
+        setup_kw.setdefault("data", self.data)
+        setup_kw["dummy"] = dummy
+        self.setup = spotpylib.TypeCurve(**setup_kw)
 
     def run(
         self,
         rep=5000,
         parallel="seq",
         run=True,
         folder=None,
@@ -376,15 +360,15 @@
             Default: ``None``
         estname : :class:`str`, optional
             File-name of the results of the spotpy estimation.
             If ``None``, it will be the current time +
             ``"_estimate"``.
             Default: ``None``
         plot_style : str, optional
-            Plot stlye. The default is "WTP".
+            Plot style. The default is "WTP".
         """
         if self.setup.dummy:
             raise ValueError(
                 "Estimate: for parameter estimation"
                 " you can't use a dummy paramter."
             )
         act_time = timemodule.strftime("%Y-%m-%d_%H-%M-%S")
@@ -415,15 +399,19 @@
         if estname is None:
             paraname = os.path.join(folder, act_time + "_estimate.txt")
         elif not os.path.isabs(estname):
             paraname = os.path.join(folder, estname)
 
         # generate the parameter-names for plotting
         paranames = dcopy(self.setup.para_names)
-        paralabels = [self.setup.val_plot_names[name] for name in paranames]
+        paralabels = []
+        for name in paranames:
+            p_label = self.setup.val_plot_names[name]
+            fit_n = self.setup.val_fit_name[name]
+            paralabels.append(f"{fit_n}({p_label})" if fit_n else p_label)
 
         if parallel == "mpi":
             # send the dbname of rank0
             from mpi4py import MPI
 
             comm = MPI.COMM_WORLD
             rank = comm.Get_rank()
@@ -463,16 +451,17 @@
                 self.result, maximize=False
             )
             void_names = para_opt.dtype.names
             para = []
             header = []
             for name in void_names:
                 para.append(para_opt[0][name])
-                header.append(name[3:])
-                self.estimated_para[header[-1]] = para[-1]
+                fit_n = self.setup.val_fit_name[name[3:]]
+                header.append(f"{fit_n}-{name[3:]}" if fit_n else name[3:])
+                self.estimated_para[name[3:]] = para[-1]
             np.savetxt(paraname, para, header=" ".join(header))
             # plot the estimation-results
             plotter.plotparatrace(
                 self.result,
                 parameternames=paranames,
                 parameterlabels=paralabels,
                 stdvalues=self.estimated_para,
@@ -540,20 +529,20 @@
             Default: ``None``
         sensname : :class:`str`, optional
             File-name of the results of the FAST estimation.
             If ``None``, it will be the current time +
             ``"_estimate"``.
             Default: ``None``
         plot_style : str, optional
-            Plot stlye. The default is "WTP".
+            Plot style. The default is "WTP".
         """
         if len(self.setup.para_names) == 1 and not self.setup.dummy:
             raise ValueError(
                 "Sensitivity: for estimation with only one parameter"
-                " you have to use a dummy paramter."
+                " you have to use a dummy parameter."
             )
         if rep is None:
             rep = spotpylib.fast_rep(
                 len(self.setup.para_names) + int(self.setup.dummy)
             )
 
         act_time = timemodule.strftime("%Y-%m-%d_%H-%M-%S")
@@ -582,15 +571,19 @@
             sensname = os.path.join(folder, sensname)
 
         sens_base, sens_ext = os.path.splitext(sensname)
         sensname1 = sens_base + "_S1" + sens_ext
 
         # generate the parameter-names for plotting
         paranames = dcopy(self.setup.para_names)
-        paralabels = [self.setup.val_plot_names[name] for name in paranames]
+        paralabels = []
+        for name in paranames:
+            p_label = self.setup.val_plot_names[name]
+            fit_n = self.setup.val_fit_name[name]
+            paralabels.append(f"{fit_n}({p_label})" if fit_n else p_label)
 
         if self.setup.dummy:
             paranames.append("dummy")
             paralabels.append("dummy")
 
         if parallel == "mpi":
             # send the dbname of rank0
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/process/__init__.py` & `welltestpy-1.2.0/src/welltestpy/process/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-# -*- coding: utf-8 -*-
 """
 welltestpy subpackage providing routines to pre process test data.
 
 .. currentmodule:: welltestpy.process
 
 Included functions
 ^^^^^^^^^^^^^^^^^^
 
 The following classes and functions are provided
 
 .. autosummary::
-    normpumptest
-    combinepumptest
-    filterdrawdown
-    cooper_jacob_correction
-    smoothing_derivative
+   :toctree:
+
+   normpumptest
+   combinepumptest
+   filterdrawdown
+   cooper_jacob_correction
+   smoothing_derivative
 """
 from .processlib import (
-    normpumptest,
     combinepumptest,
-    filterdrawdown,
     cooper_jacob_correction,
+    filterdrawdown,
+    normpumptest,
     smoothing_derivative,
 )
 
 __all__ = [
     "normpumptest",
     "combinepumptest",
     "filterdrawdown",
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/process/processlib.py` & `welltestpy-1.2.0/src/welltestpy/process/processlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,10 @@
-# -*- coding: utf-8 -*-
-"""
-welltestpy subpackage providing functions to pre process data.
-
-.. currentmodule:: welltestpy.process.processlib
-
-The following classes are provided
-
-.. autosummary::
-   normpumptest
-   combinepumptest
-   filterdrawdown
-   cooper_jacob_correction
-   smoothing_derivative
-"""
+"""welltestpy subpackage providing functions to pre process data."""
 from copy import deepcopy as dcopy
+
 import numpy as np
 from scipy import signal
 
 from ..data import testslib
 
 __all__ = [
     "normpumptest",
@@ -247,33 +234,34 @@
     except ValueError:  # in this case there are to few data points
         hout = np.interp(tout, time, head)
 
     return observation(time=tout, observation=hout)
 
 
 def cooper_jacob_correction(observation, sat_thickness):
-    """correction method for observed drawdown for unconfined aquifers.
+    """
+    Correction method for observed drawdown for unconfined aquifers.
 
     Parameters
     ----------
     observation : :class:`welltestpy.data.Observation`
         The observation to be corrected.
     sat_thickness : :class:`float`
-        vertical length of the aquifer in which its pores are filled with water.
+        Vertical length of the aquifer in which its pores are filled with water.
 
     Returns
     -------
     The corrected drawdown
 
     """
     # split the observations into array for head.
     head = observation.observation
 
     # cooper and jacob correction
-    head = head - (head ** 2) / (2 * sat_thickness)
+    head = head - (head**2) / (2 * sat_thickness)
 
     # return new observation
     observation(observation=head)
 
     return observation
 
 
@@ -287,16 +275,16 @@
     time: :class: 'array'
         An array with the time values for the observed head values.
     method : :class:`str`, optional
         Method to calculate the time derivative.
         Default: "bourdet"
 
     Returns
-    ---------
-    the derivative of the observed heads.
+    -------
+    The derivative of the observed heads.
 
     """
     # create arrays for the input of head and time.
     derhead = np.zeros(len(head))
     t = np.arange(len(time))
     if method == "bourdet":
         for i in t[1:-1]:
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/tools/__init__.py` & `welltestpy-1.2.0/src/welltestpy/tools/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-# -*- coding: utf-8 -*-
 """
 welltestpy subpackage providing miscellaneous tools.
 
 .. currentmodule:: welltestpy.tools
 
 Included functions
 ^^^^^^^^^^^^^^^^^^
 
 The following functions are provided for point triangulation
 
 .. autosummary::
+   :toctree:
+
    triangulate
    sym
 
 The following plotting routines are provided
 
 .. autosummary::
+   :toctree:
+
    campaign_plot
    fadeline
    plot_well_pos
    campaign_well_plot
    plotfit_transient
    plotfit_steady
    plotparainteract
    plotparatrace
    plotsensitivity
    diagnostic_plot_pump_test
 """
-from . import plotter, trilib, diagnostic_plots
-
-from .trilib import triangulate, sym
-
+from . import diagnostic_plots, plotter, trilib
+from .diagnostic_plots import diagnostic_plot_pump_test
 from .plotter import (
     campaign_plot,
+    campaign_well_plot,
     fadeline,
     plot_well_pos,
-    campaign_well_plot,
-    plotfit_transient,
     plotfit_steady,
+    plotfit_transient,
     plotparainteract,
     plotparatrace,
     plotsensitivity,
 )
-
-from .diagnostic_plots import diagnostic_plot_pump_test
+from .trilib import sym, triangulate
 
 __all__ = [
     "triangulate",
     "sym",
     "campaign_plot",
     "fadeline",
     "plot_well_pos",
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/tools/diagnostic_plots.py` & `welltestpy-1.2.0/src/welltestpy/tools/diagnostic_plots.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,34 @@
-"""
-welltestpy subpackage to make diagnostic plots.
-
-.. currentmodule:: welltestpy.tools.diagnostic_plots
-
-The following classes and functions are provided
-
-.. autosummary::
-   diagnostic_plot_pump_test
-
-"""
+"""welltestpy subpackage to make diagnostic plots."""
 # pylint: disable=C0103
-
-
+import matplotlib.pyplot as plt
 import numpy as np
 
 from ..process import processlib
 from . import plotter
 
-import matplotlib.pyplot as plt
-
 
 def diagnostic_plot_pump_test(
     observation,
     rate,
     method="bourdet",
     linthresh_time=1.0,
     linthresh_head=1e-5,
     fig=None,
     ax=None,
     plotname=None,
     style="WTP",
 ):
-    """plot the derivative with the original data.
+    """
+    Plot the derivative with the original data.
 
     Parameters
     ----------
     observation : :class:`welltestpy.data.Observation`
-         The observation to calculate the derivative.
+        The observation to calculate the derivative.
     rate : :class:`float`
         Pumping rate.
     method : :class:`str`, optional
         Method to calculate the time derivative.
         Default: "bourdet"
     linthresh_time : :class: 'float'
         Range of time around 0 that behaves linear.
@@ -57,61 +45,55 @@
     plotname : str, optional
         Plot name if the result should be saved.
         Default: None.
     style : str, optional
         Plot style.
         Default: "WTP".
 
-     Returns
-     ---------
-     Diagnostic plot
+    Returns
+    -------
+    Diagnostic plot
     """
     head, time = observation()
     head = np.array(head, dtype=float).reshape(-1)
     time = np.array(time, dtype=float).reshape(-1)
     if rate < 0:
         head = head * -1
     derivative = processlib.smoothing_derivative(
         head=head, time=time, method=method
     )
     # setting variables
-    x = time
-    y = head
-    sx = time
-    sy = head
     dx = time[1:-1]
     dy = derivative[1:-1]
 
     # plotting
     if style == "WTP":
         style = "ggplot"
         font_size = plt.rcParams.get("font.size", 10.0)
         keep_fs = True
     with plt.style.context(style):
         if keep_fs:
             plt.rcParams.update({"font.size": font_size})
         fig, ax = plotter._get_fig_ax(fig, ax)
-        ax.scatter(x, y, color="red", label="drawdown")
-        ax.plot(sx, sy, c="red")
-        ax.plot(dx, dy, c="black", linestyle="dashed")
-        ax.scatter(dx, dy, c="black", marker="+", label="time derivative")
+        ax.scatter(time, head, color="C0", label="drawdown")
+        ax.plot(dx, dy, color="C1", label="time derivative")
         ax.set_xscale("symlog", linthresh=linthresh_time)
         ax.set_yscale("symlog", linthresh=linthresh_head)
         ax.set_xlabel("$t$ in [s]", fontsize=16)
         ax.set_ylabel("$h$ and $dh/dx$ in [m]", fontsize=16)
         lgd = ax.legend(loc="upper left", facecolor="w")
         min_v = min(np.min(head), np.min(dy))
         max_v = max(np.max(head), np.max(dy))
         max_e = int(np.ceil(np.log10(max_v)))
         if min_v < linthresh_head:
             min_e = -np.inf
         else:
             min_e = int(np.floor(np.log10(min_v)))
-        ax.set_ylim(10.0 ** min_e, 10.0 ** max_e)
-        yticks = [0 if min_v < linthresh_head else 10.0 ** min_e]
+        ax.set_ylim(10.0**min_e, 10.0**max_e)
+        yticks = [0 if min_v < linthresh_head else 10.0**min_e]
         thresh_e = int(np.floor(np.log10(linthresh_head)))
         first_e = thresh_e if min_v < linthresh_head else (min_e + 1)
         yticks += list(10.0 ** np.arange(first_e, max_e + 1))
         ax.set_yticks(yticks)
         fig.tight_layout()
         if plotname is not None:
             fig.savefig(
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/tools/plotter.py` & `welltestpy-1.2.0/src/welltestpy/tools/plotter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,18 @@
-# -*- coding: utf-8 -*-
-"""
-welltestpy subpackage providing plotting routines.
-
-.. currentmodule:: welltestpy.tools.plotter
-
-The following classes and functions are provided
-
-.. autosummary::
-   campaign_plot
-   campaign_well_plot
-   plot_pump_test
-   plot_well_pos
-   fadeline
-   plotfit_transient
-   plotfit_steady
-   plotparainteract
-   plotparatrace
-   plotsensitivity
-"""
+"""welltestpy subpackage providing plotting routines."""
 # pylint: disable=C0103
 import copy
-import warnings
 import functools as ft
+import warnings
 
-import numpy as np
-
-from mpl_toolkits.mplot3d import Axes3D
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
+import numpy as np
+from mpl_toolkits.mplot3d import Axes3D
+from scipy.stats import gaussian_kde
 
 
 def _get_fig_ax(
     fig=None,
     ax=None,
     ax_name="rectilinear",
     sub_args=None,
@@ -191,15 +172,15 @@
     plot_tests : bool, optional
         DESCRIPTION. The default is True.
     plot_well_names : TYPE, optional
         DESCRIPTION. The default is True.
     fig : Figure, optional
         Matplotlib figure to plot on. The default is None.
     style : str, optional
-        Plot stlye. The default is "WTP".
+        Plot style. The default is "WTP".
 
     Returns
     -------
     ax : Axes
         The created matplotlib axes.
 
     """
@@ -269,24 +250,24 @@
     """Plot a pumping test.
 
     Parameters
     ----------
     pump_test: :class:`PumpingTest`
         Pumping test class that should be plotted.
     wells : :class:`dict`
-        Dictonary containing the well classes sorted by name.
+        Dictionary containing the well classes sorted by name.
     exclude: :class:`list`, optional
         List of wells that should be excluded from the plot.
         Default: ``None``
     fig : Figure, optional
         Matplotlib figure to plot on. The default is None.
     ax : :class:`Axes`
         Matplotlib axes to plot on. The default is None.
     style : str, optional
-        Plot stlye. The default is "WTP".
+        Plot style. The default is "WTP".
 
     Returns
     -------
     ax : Axes
         The created matplotlib axes.
 
     Notes
@@ -322,15 +303,15 @@
         elif state == "transient":
             ax1 = ax
             ax2 = None
         elif state == "steady":
             ax1 = None
             ax2 = ax
         else:
-            raise ValueError("plot_pump_test: unknow state of pumping test.")
+            raise ValueError("plot_pump_test: unknown state of pumping test.")
         for i, k in enumerate(plot_wells):
             if k != pump_test.pumpingwell:
                 dist = wells[k] - wells[pump_test.pumpingwell]
             else:
                 dist = wells[pump_test.pumpingwell].radius
             if pump_test.observations[k].state == "transient":
                 if abslab:
@@ -422,38 +403,38 @@
     plot_well_names : bool, optional
         Whether to plot the well-names. The default is True.
     ticks_set : int or str, optional
         Tick spacing in the plot. The default is "auto".
     fig : Figure, optional
         Matplotlib figure to plot on. The default is None.
     style : str, optional
-        Plot stlye. The default is "WTP".
+        Plot style. The default is "WTP".
 
     Returns
     -------
     fig : Figure
         The created matplotlib figure.
     """
     # calculate Column- and Row-count for quadratic shape of the plot
     # total number of plots
     total_n = len(well_const)
     # columns near the square-root but tendentially wider than tall
     col_n = int(np.ceil(np.sqrt(total_n)))
     # enough rows to catch all plots
     row_n = int(np.ceil(total_n / col_n))
-    # Possition numbers as array
+    # Position numbers as array
     pos_tuple = np.arange(total_n) + 1
 
     # generate names for points if undefined
     if names is None:
         names = []
         for i in range(len(well_const[0])):
             names.append("p" + str(i))
 
-    # genearte commen borders for all plots
+    # generate common borders for all plots
     xmax = -np.inf
     xmin = np.inf
     ymax = -np.inf
     ymin = np.inf
 
     for i in well_const:
         for j in i:
@@ -553,15 +534,15 @@
     else:
         style1 = style2 = style
     with plt.style.context(style1):
         clrs = plt.rcParams["axes.prop_cycle"].by_key()["color"]
         clr_n = len(clrs)
     with plt.style.context(style2):
         if keep_fs:
-            # font type fix (resetted in default)
+            # font type fix (reset in default)
             plt.rcParams.update({"pdf.fonttype": pdf_ft, "ps.fonttype": ps_ft})
             plt.rcParams.update({"font.size": font_size})
         fig, ax = _get_fig_ax(fig, ax, ax_name=Axes3D.name, figsize=(7.5, 7))
         val_fix = setup.val_fix
         for kwarg in ["time", "rad"]:
             val_fix.pop(extra[kwarg], None)
 
@@ -720,16 +701,16 @@
                 "log-radius plot",
                 ha="right",
                 va="bottom",
                 bbox=dict(boxstyle="round", ec="k", fc="w"),
                 transform=axins.transAxes,
             )
         for ri, re in enumerate(rad):
-            h = plot_f(**{extra["rad"]: re}).reshape(-1)
-            h1 = data[ri]
+            h = np.asarray(plot_f(**{extra["rad"]: re})).reshape(-1)
+            h1 = np.asarray(data[ri]).reshape(-1)
             color = clrs[(test_name.index(radnames[ri, 0]) + 2) % clr_n]
             if radnames[ri, 0] == radnames[ri, 1]:
                 label = "test at '{}'".format(radnames[ri, 0])
             else:
                 label = None
             ax.plot([re, re], [h, h1], alpha=0.6, color=color, zorder=100)
             ax.scatter(re, data[ri], color=color, label=label, zorder=300)
@@ -755,45 +736,31 @@
             fig.savefig(plotname, format="pdf")
 
     return ax
 
 
 def plotparainteract(result, paranames, plotname=None, fig=None, style="WTP"):
     """Plot of parameter interaction."""
-    import pandas as pd
-
     style = copy.deepcopy(plt.rcParams) if style is None else style
     keep_fs = False
     if style == "WTP":
         style = "default"
         font_size = plt.rcParams.get("font.size", 10.0)
         # font type fix
         pdf_ft = plt.rcParams.get("pdf.fonttype", 42)
         ps_ft = plt.rcParams.get("ps.fonttype", 42)
         keep_fs = True
     with plt.style.context(style):
         if keep_fs:
             # font type fix (resetted in default)
             plt.rcParams.update({"pdf.fonttype": pdf_ft, "ps.fonttype": ps_ft})
             plt.rcParams.update({"font.size": font_size})
-        fig, ax = _get_fig_ax(fig, ax=None, figsize=(12, 12))
         fields = [par for par in result.dtype.names if par.startswith("par")]
-        parameterdistribtion = result[fields]
-        df = pd.DataFrame(
-            np.asarray(parameterdistribtion).T.tolist(), columns=paranames
-        )
-        with warnings.catch_warnings():
-            # We know that fig is resetted, but we need to give ax to set fig
-            warnings.simplefilter("ignore", UserWarning)
-            if len(paranames) > 1:
-                pd.plotting.scatter_matrix(
-                    df, alpha=0.2, ax=ax, diagonal="kde"
-                )
-            else:
-                df.plot.kde(ax=ax)
+        para = [result[:][name] for name in fields]
+        fig = _scatter_matrix(para, paranames, fig)
         fig.tight_layout()
         fig.subplots_adjust(hspace=0, wspace=0, bottom=0.1)
         if plotname is not None:
             fig.savefig(plotname, format="pdf")
     return fig
 
 
@@ -817,17 +784,18 @@
         font_size = plt.rcParams.get("font.size", 10.0)
         keep_fs = True
     with plt.style.context(style):
         if keep_fs:
             plt.rcParams.update({"font.size": font_size})
         clrs = plt.rcParams["axes.prop_cycle"].by_key()["color"]
         fig = _get_fig_ax(fig, ax=False, figsize=(15, 3 * rows))
-
+        axes = []
         for j in range(rows):
             ax = fig.add_subplot(rows, 1, 1 + j)
+            axes.append(ax)
             data = result["par" + parameternames[j]]
 
             ax.plot(data, "-", color=clrs[0])
 
             if stdvalues is not None:
                 ax.plot(
                     [stdvalues[parameternames[j]]] * rep,
@@ -840,23 +808,19 @@
                 )
                 ax.legend()
 
             if xticks is None:
                 xticks = np.linspace(0, 1, 11) * len(data)
 
             ax.set_xlim(0, rep)
-            ax.set_ylim(
-                np.min(data) - 0.1 * np.max(abs(data)),
-                np.max(data) + 0.1 * np.max(abs(data)),
-            )
+            ax.margins(y=0.2)
             ax.xaxis.set_ticks(xticks)
-            ax.set_ylabel(
-                parameterlabels[j], rotation=0, fontsize="large", labelpad=10
-            )
-
+            ax.set_ylabel(parameterlabels[j], fontsize="large")
+        ax.set_xlabel("Iterations", fontsize="large")
+        fig.align_ylabels(axes)
         fig.tight_layout()
         if plotname is not None:
             fig.savefig(plotname, format="pdf", bbox_inches="tight")
     return fig
 
 
 def plotsensitivity(
@@ -891,7 +855,59 @@
             fig.savefig(
                 plotname,
                 format="pdf",
                 bbox_extra_artists=(lgd,),
                 bbox_inches="tight",
             )
     return ax
+
+
+def _scatter_matrix(data, label, fig=None):
+    data = np.array(data, ndmin=2, dtype=float)
+    n = len(data)
+    axes = np.empty(n**2, dtype=object)
+    for i in range(n**2):
+        fig, axes[i] = _get_fig_ax(fig, figsize=(8, 8), sub_args=(n, n, i + 1))
+    axes = axes.reshape(n, n)
+
+    boundaries_list = []
+    for dat in data:
+        rmin, rmax = np.min(dat), np.max(dat)
+        rdelta = (rmax - rmin) * 0.025
+        boundaries_list.append((rmin - rdelta, rmax + rdelta))
+
+    for i, a in enumerate(data):
+        for j, b in enumerate(data):
+            ax = axes[i, j]
+            if i == j:
+                ind = np.linspace(a.min(), a.max(), 1000)
+                ax.plot(ind, gaussian_kde(a).evaluate(ind))
+            else:
+                ax.scatter(b, a, marker=".", alpha=0.2, edgecolors="none")
+                ax.set_ylim(boundaries_list[i])
+            ax.set_xlim(boundaries_list[j])
+            ax.set_xlabel(label[j])
+            ax.set_ylabel(label[i])
+            if j != 0:
+                ax.yaxis.set_visible(False)
+            if i != n - 1:
+                ax.xaxis.set_visible(False)
+
+    # reset labels of first kde plot to match scatter plots
+    if n > 1:
+        lim1 = boundaries_list[0]
+        locs = axes[0, 1].yaxis.get_majorticklocs()
+        locs = locs[(lim1[0] <= locs) & (locs <= lim1[1])]
+        adj = (locs - lim1[0]) / (lim1[1] - lim1[0])
+
+        lim0 = axes[0, 0].get_ylim()
+        adj = adj * (lim0[1] - lim0[0]) + lim0[0]
+        axes[0, 0].yaxis.set_ticks(adj)
+        locs = locs.astype(int) if np.all(locs == locs.astype(int)) else locs
+        axes[0, 0].yaxis.set_ticklabels(locs)
+        fig.align_ylabels(axes[:, 0])
+        fig.align_xlabels(axes[-1, :])
+
+    for ax in axes[-1, :]:
+        plt.setp(ax.get_xticklabels(), rotation=90)
+
+    return fig
```

### Comparing `welltestpy-1.1.0rc1/welltestpy/tools/trilib.py` & `welltestpy-1.2.0/src/welltestpy/tools/trilib.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,12 @@
-# -*- coding: utf-8 -*-
-"""
-welltestpy subpackage providing routines for triangulation.
-
-.. currentmodule:: welltestpy.tools.trilib
-
-The following functions are provided
-
-.. autosummary::
-   triangulate
-   sym
-"""
+"""welltestpy subpackage providing routines for triangulation."""
 # pylint: disable=C0103
 from copy import deepcopy as dcopy
-import numpy as np
 
+import numpy as np
 
 __all__ = ["triangulate", "sym"]
 
 
 def triangulate(distances, prec, all_pos=False):
     """Triangulate points by given distances.
 
@@ -34,15 +23,15 @@
         It hat to be a symmetric matrix with a vanishing diagonal and
 
             ``distances[i,j] = |pi-pj|``
 
         If a distance is unknown, you can set it to ``-1``.
     prec : :class:`float`
         Given Precision to be used within the algorithm. This can be used to
-        smooth away messure errors
+        smooth away measure errors
     all_pos : :class:`bool`, optional
         If `True` all possible constellations will be calculated. Otherwise,
         the first possibility will be returned.
         Default: False
     """
     if not _distvalid(distances, prec / 3.0):
         raise ValueError("Given distances are not valid")
@@ -85,15 +74,15 @@
     return sol
 
 
 def _triangulatesgl(distances, sp1, sp2, prec):
     """
     Try to triangulate points.
 
-    With startingpoints sp1 and sp2 and a given precicion.
+    With starting points sp1 and sp2 and a given precision.
     Thereby sp1 will be at the origin (0,0) and sp2 will be at (|sp2-sp1|,0).
     """
     res = []
 
     if distances[sp1, sp2] < -0.5:
         return res
 
@@ -125,15 +114,15 @@
     return res
 
 
 def _addpoints(sol, distances, prec):
     """
     Try for each point to add it to a given solution-approach.
 
-    gives all possibilties and a status about the solution:
+    gives all possibilities and a status about the solution:
         state = 0: possibilities found
         state = 1: no possibilities
         state = 2: solution-approach has a contradiction with a point
     """
     res = []
 
     posfound = False
@@ -164,15 +153,15 @@
     return res, 1
 
 
 def _addpoint(sol, i, distances, prec):
     """
     Try to add point i to a given solution-approach.
 
-    gives all possibilties and a status about the solution:
+    gives all possibilities and a status about the solution:
         state = 0: possibilities found
         state = 1: no possibilities but no contradiction
         state = 2: solution-approach has a contradiction with point i
     """
     res = []
 
     # if i is already part of the solution return it
@@ -221,27 +210,27 @@
 
     pntscount = len(sol)
 
     # if no distances known, return empty result and the unknown-state
     if distances[i, n] < -0.5 or distances[i, m] < -0.5:
         return tmppnt, state
 
-    # if the Triangle inequality is not fullfilled give a contradiction
+    # if the Triangle inequality is not fulfilled give a contradiction
     if distances[i, n] + distances[i, m] < _dist(sol[n], sol[m]):
         state = 2
         return tmppnt, state
 
     # generate the affine rotation to bring the points in the right place
     g = _affinef(*_invtranmat(*_tranmat(sol[n], sol[m])))
 
     # generate the coordinates
     x = _xvalue(distances[i, n], distances[i, m], _dist(sol[n], sol[m]))
     y1, y2 = _yvalue(distances[i, n], distances[i, m], _dist(sol[n], sol[m]))
 
-    # generate the possible positons
+    # generate the possible positions
     pos1 = g(np.array([x, y1]))
     pos2 = g(np.array([x, y2]))
 
     valid1 = True
     valid2 = True
 
     # check if the possible positions are valid
@@ -263,15 +252,15 @@
         state = 2
 
     return tmppnt, state
 
 
 def _solequal(sol1, sol2, prec):
     """
-    Compare two different solutions with a given precicion.
+    Compare two different solutions with a given precision.
 
     Return True if they equal.
     """
     res = True
 
     for sol_1, sol_2 in zip(sol1, sol2):
         if np.ndim(sol_1) != 0 and np.ndim(sol_2) != 0:
@@ -284,15 +273,15 @@
     return res
 
 
 def _distvalid(dis, err=0.0, verbose=True):
     """
     Check if the given distances between the points are valid.
 
-    I.e. if they fullfill the triangle-equation.
+    I.e. if they fulfill the triangle-equation.
     """
     valid = True
     valid &= np.all(dis == dis.T)
     valid &= np.all(dis.diagonal() == 0.0)
 
     pntscount = np.shape(dis)[0]
 
@@ -318,32 +307,32 @@
     """
     Get the x-value for the upper point of a triangle.
 
     where c is the length of the down side starting in the origin and
     lying on the x-axes, a is the distance of the unknown point to the origen
     and b is the distance of the unknown point to the righter given point
     """
-    return (a ** 2 + c ** 2 - b ** 2) / (2 * c)
+    return (a**2 + c**2 - b**2) / (2 * c)
 
 
 def _yvalue(b, a, c):
     """
     Get the two possible y-values for the upper point of a triangle.
 
     where c is the length of the down side starting in the origin and
     lying on the x-axes, a is the distance of the unknown point to the origen
     and b is the distance of the unknown point to the righter given point
     """
-    # ckeck flatness to eliminate numerical errors when the triangle is flat
+    # check flatness to eliminate numerical errors when the triangle is flat
     if a + b <= c or a + c <= b or b + c <= a:
         return 0.0, -0.0
 
     res = 2 * ((a * b) ** 2 + (a * c) ** 2 + (b * c) ** 2)
-    res -= a ** 4 + b ** 4 + c ** 4
-    # in case of numerical errors set res to 0 (hope you check validty before)
+    res -= a**4 + b**4 + c**4
+    # in case of numerical errors set res to 0 (hope you check validity before)
     res = max(res, 0.0)
     res = np.sqrt(res)
     res /= 2 * c
     return res, -res
 
 
 def _rotate(res):
@@ -360,32 +349,32 @@
             rotres[rot_i][rot_e_j] = g(rot_e_e)
 
     return rotres
 
 
 def _tranmat(a, b):
     """
-    Get the coefficents for the affine-linear function f(x)=Ax+s.
+    Get the coefficients for the affine-linear function f(x)=Ax+s.
 
-    Which fullfills that A is a rotation-matrix,
+    Which fulfills that A is a rotation-matrix,
     f(a) = [0,0] and f(b) = [|b-a|,0].
     """
     A = np.zeros((2, 2))
     A[0, 0] = b[0] - a[0]
     A[1, 1] = b[0] - a[0]
     A[1, 0] = -(b[1] - a[1])
     A[0, 1] = +(b[1] - a[1])
     A /= _dist(a, b)
     s = -np.dot(A, a)
     return A, s
 
 
 def _invtranmat(A, s):
     """
-    Get the coefficents for the affine-linear function g(x)=Bx+t.
+    Get the coefficients for the affine-linear function g(x)=Bx+t.
 
     which is inverse to f(x)=Ax+s
     """
     B = np.linalg.inv(A)
     t = -np.dot(B, s)
     return B, t
```

