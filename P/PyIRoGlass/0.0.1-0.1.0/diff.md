# Comparing `tmp/PyIRoGlass-0.0.1.tar.gz` & `tmp/PyIRoGlass-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyIRoGlass-0.0.1.tar", last modified: Fri Mar 24 20:46:34 2023, max compression
+gzip compressed data, was "PyIRoGlass-0.1.0.tar", last modified: Tue Apr 18 15:17:41 2023, max compression
```

## Comparing `PyIRoGlass-0.0.1.tar` & `PyIRoGlass-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:46:34.206893 PyIRoGlass-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-03-24 20:46:34.206893 PyIRoGlass-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-03-24 20:46:21.000000 PyIRoGlass-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-24 20:46:34.206893 PyIRoGlass-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-24 20:46:22.000000 PyIRoGlass-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:46:34.206893 PyIRoGlass-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:46:34.206893 PyIRoGlass-0.0.1/src/PyIRoGlass/
--rw-r--r--   0 runner    (1001) docker     (123)    29500 2023-03-24 20:46:22.000000 PyIRoGlass-0.0.1/src/PyIRoGlass/BaselineAvgPCA.npz
--rw-r--r--   0 runner    (1001) docker     (123)    19852 2023-03-24 20:46:22.000000 PyIRoGlass-0.0.1/src/PyIRoGlass/H2Om1635PCA.npz
--rw-r--r--   0 runner    (1001) docker     (123)   117085 2023-03-24 20:46:22.000000 PyIRoGlass-0.0.1/src/PyIRoGlass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-24 20:46:22.000000 PyIRoGlass-0.0.1/src/PyIRoGlass/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 20:46:34.206893 PyIRoGlass-0.0.1/src/PyIRoGlass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-03-24 20:46:34.000000 PyIRoGlass-0.0.1/src/PyIRoGlass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-24 20:46:34.000000 PyIRoGlass-0.0.1/src/PyIRoGlass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 20:46:34.000000 PyIRoGlass-0.0.1/src/PyIRoGlass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-24 20:46:34.000000 PyIRoGlass-0.0.1/src/PyIRoGlass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-24 20:46:34.000000 PyIRoGlass-0.0.1/src/PyIRoGlass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:17:41.581746 PyIRoGlass-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-18 15:17:41.581746 PyIRoGlass-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-18 15:17:28.000000 PyIRoGlass-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 15:17:41.581746 PyIRoGlass-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-18 15:17:29.000000 PyIRoGlass-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:17:41.577746 PyIRoGlass-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:17:41.577746 PyIRoGlass-0.1.0/src/PyIRoGlass/
+-rw-r--r--   0 runner    (1001) docker     (123)    29500 2023-04-18 15:17:29.000000 PyIRoGlass-0.1.0/src/PyIRoGlass/BaselineAvgPCA.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    19852 2023-04-18 15:17:29.000000 PyIRoGlass-0.1.0/src/PyIRoGlass/H2Om1635PCA.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   117683 2023-04-18 15:17:29.000000 PyIRoGlass-0.1.0/src/PyIRoGlass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-18 15:17:29.000000 PyIRoGlass-0.1.0/src/PyIRoGlass/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:17:41.577746 PyIRoGlass-0.1.0/src/PyIRoGlass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-18 15:17:41.000000 PyIRoGlass-0.1.0/src/PyIRoGlass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-18 15:17:41.000000 PyIRoGlass-0.1.0/src/PyIRoGlass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:17:41.000000 PyIRoGlass-0.1.0/src/PyIRoGlass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-18 15:17:41.000000 PyIRoGlass-0.1.0/src/PyIRoGlass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 15:17:41.000000 PyIRoGlass-0.1.0/src/PyIRoGlass.egg-info/top_level.txt
```

### Comparing `PyIRoGlass-0.0.1/PKG-INFO` & `PyIRoGlass-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: PyIRoGlass
-Version: 0.0.1
+Version: 0.1.0
 Summary: PyIRoGlass
 Home-page: https://github.com/sarahshi/PyIRoGlass
 Author: Sarah C. Shi
 Author-email: sarah.c.shi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # PyIRoGlass
 [![PyPI](https://badgen.net/pypi/v/PyIRoGlass)](https://pypi.org/project/PyIRoGlass/)
 [![Build Status](https://github.com/SarahShi/PyIRoGlass/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/SarahShi/PyIRoGlass/actions/workflows/main.yml)
+[![Documentation Status](https://readthedocs.org/projects/pyiroglass/badge/?version=latest)](https://pyiroglass.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/SarahShi/PyIRoGlass/branch/main/graph/badge.svg)](https://codecov.io/gh/SarahShi/PyIRoGlass/branch/main)
 
 PyIRoGlass is a Bayesian MCMC-founded Python algorithm for determining volatile concentrations and speciation for $\mathrm{H_2O_{t, 3550}}$, $\mathrm{H_2O_{m, 1635}}$, $\mathrm{CO_{3, 1515}^{2-}}$, $\mathrm{CO_{3, 1430}^{2-}}$, $\mathrm{H_2O_{m, 5200}}$, and $\mathrm{OH_{4500}}$ from basaltic to andesitic transmission FTIR spectra. PyIRoGlass is written in the open-source language Python3 with the $\mathrm{MC^3}$ package, allowing for the proper sampling of parameter space and the determination of volatile concentrations with uncertainties. 
 
 
 Quantifying concentrations of volatiles in magmas is critical for estimating the conditions of magma storage, assessing phase equilibria, and understanding eruption. We develop and present PyIRoGlass, a new open-source Python package implementing a Bayesian method with Markov Chain Monte Carlo sampling, to process the transmission FTIR spectra of basaltic to andesitic glasses and to quantify volatile concentrations with uncertainties for all $\mathrm{H_2O}$ and $\mathrm{CO_2}$ species in basaltic to andesitic glasses, when devolatilized baselines are not readily available. We utilize spectra of natural, devolatilized melt inclusions from the Aleutians to determine the fundamental shapes and variability of the baseline in the mid-IR region, in which the $\mathrm{CO_3^{2-}}$ doublets and $\mathrm{H_2O_{m, 1635}}$ peaks are found. The shape of the baseline and that of the peaks varies across samples, dependent on the chemistry of samples and concentration of volatiles. All parameters within the Beer-Lambert Law — including the baseline, molar absorptivity, thickness, and density — are closely examined to quantify the associated uncertainties. Molar absorptivity is recalibrated as a function of compositional parameters by applying a Newtonian inversion, allowing for the quantification of the uncertainty of the inversion and of the uncertainty in composition. PyIRoGlass further provides functions for processing reflectance FTIR spectra to determine sample wafer thickness. Development of this Bayesian method with MCMC sampling allows for the sampling of all possible baselines and peaks to iteratively solve for the best-fit parameters, presenting a promising method forward for robustly estimating uncertainty and accounting for covariance within fit parameters within a unified framework to confidently process transmission FTIR spectra to determine volatile concentrations with uncertainties. The open-source nature of the Python package allows for continuous evolution as more data become available.
```

#### html2text {}

```diff
@@ -1,46 +1,48 @@
-Metadata-Version: 2.1 Name: PyIRoGlass Version: 0.0.1 Summary: PyIRoGlass Home-
+Metadata-Version: 2.1 Name: PyIRoGlass Version: 0.1.0 Summary: PyIRoGlass Home-
 page: https://github.com/sarahshi/PyIRoGlass Author: Sarah C. Shi Author-email:
 sarah.c.shi@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown #
 PyIRoGlass [![PyPI](https://badgen.net/pypi/v/PyIRoGlass)](https://pypi.org/
 project/PyIRoGlass/) [![Build Status](https://github.com/SarahShi/PyIRoGlass/
 actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/SarahShi/
-PyIRoGlass/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/
-SarahShi/PyIRoGlass/branch/main/graph/badge.svg)](https://codecov.io/gh/
-SarahShi/PyIRoGlass/branch/main) PyIRoGlass is a Bayesian MCMC-founded Python
-algorithm for determining volatile concentrations and speciation for $\mathrm
-{H_2O_{t, 3550}}$, $\mathrm{H_2O_{m, 1635}}$, $\mathrm{CO_{3, 1515}^{2-}}$,
-$\mathrm{CO_{3, 1430}^{2-}}$, $\mathrm{H_2O_{m, 5200}}$, and $\mathrm{OH_
-{4500}}$ from basaltic to andesitic transmission FTIR spectra. PyIRoGlass is
-written in the open-source language Python3 with the $\mathrm{MC^3}$ package,
-allowing for the proper sampling of parameter space and the determination of
-volatile concentrations with uncertainties. Quantifying concentrations of
-volatiles in magmas is critical for estimating the conditions of magma storage,
-assessing phase equilibria, and understanding eruption. We develop and present
-PyIRoGlass, a new open-source Python package implementing a Bayesian method
-with Markov Chain Monte Carlo sampling, to process the transmission FTIR
-spectra of basaltic to andesitic glasses and to quantify volatile
-concentrations with uncertainties for all $\mathrm{H_2O}$ and $\mathrm{CO_2}$
-species in basaltic to andesitic glasses, when devolatilized baselines are not
-readily available. We utilize spectra of natural, devolatilized melt inclusions
-from the Aleutians to determine the fundamental shapes and variability of the
-baseline in the mid-IR region, in which the $\mathrm{CO_3^{2-}}$ doublets and
-$\mathrm{H_2O_{m, 1635}}$ peaks are found. The shape of the baseline and that
-of the peaks varies across samples, dependent on the chemistry of samples and
-concentration of volatiles. All parameters within the Beer-Lambert Law â
-including the baseline, molar absorptivity, thickness, and density â are
-closely examined to quantify the associated uncertainties. Molar absorptivity
-is recalibrated as a function of compositional parameters by applying a
-Newtonian inversion, allowing for the quantification of the uncertainty of the
-inversion and of the uncertainty in composition. PyIRoGlass further provides
-functions for processing reflectance FTIR spectra to determine sample wafer
-thickness. Development of this Bayesian method with MCMC sampling allows for
-the sampling of all possible baselines and peaks to iteratively solve for the
-best-fit parameters, presenting a promising method forward for robustly
-estimating uncertainty and accounting for covariance within fit parameters
-within a unified framework to confidently process transmission FTIR spectra to
-determine volatile concentrations with uncertainties. The open-source nature of
-the Python package allows for continuous evolution as more data become
-available. [Open_In_Colab] [![Binder](https://mybinder.org/badge_logo.svg)]
-(https://mybinder.org/v2/gh/SarahShi/PyIRoGlass/HEAD)
+PyIRoGlass/actions/workflows/main.yml) [![Documentation Status](https://
+readthedocs.org/projects/pyiroglass/badge/?version=latest)](https://
+pyiroglass.readthedocs.io/en/latest/?badge=latest) [![codecov](https://
+codecov.io/gh/SarahShi/PyIRoGlass/branch/main/graph/badge.svg)](https://
+codecov.io/gh/SarahShi/PyIRoGlass/branch/main) PyIRoGlass is a Bayesian MCMC-
+founded Python algorithm for determining volatile concentrations and speciation
+for $\mathrm{H_2O_{t, 3550}}$, $\mathrm{H_2O_{m, 1635}}$, $\mathrm{CO_{3,
+1515}^{2-}}$, $\mathrm{CO_{3, 1430}^{2-}}$, $\mathrm{H_2O_{m, 5200}}$, and
+$\mathrm{OH_{4500}}$ from basaltic to andesitic transmission FTIR spectra.
+PyIRoGlass is written in the open-source language Python3 with the $\mathrm
+{MC^3}$ package, allowing for the proper sampling of parameter space and the
+determination of volatile concentrations with uncertainties. Quantifying
+concentrations of volatiles in magmas is critical for estimating the conditions
+of magma storage, assessing phase equilibria, and understanding eruption. We
+develop and present PyIRoGlass, a new open-source Python package implementing a
+Bayesian method with Markov Chain Monte Carlo sampling, to process the
+transmission FTIR spectra of basaltic to andesitic glasses and to quantify
+volatile concentrations with uncertainties for all $\mathrm{H_2O}$ and $\mathrm
+{CO_2}$ species in basaltic to andesitic glasses, when devolatilized baselines
+are not readily available. We utilize spectra of natural, devolatilized melt
+inclusions from the Aleutians to determine the fundamental shapes and
+variability of the baseline in the mid-IR region, in which the $\mathrm{CO_3^
+{2-}}$ doublets and $\mathrm{H_2O_{m, 1635}}$ peaks are found. The shape of the
+baseline and that of the peaks varies across samples, dependent on the
+chemistry of samples and concentration of volatiles. All parameters within the
+Beer-Lambert Law â including the baseline, molar absorptivity, thickness, and
+density â are closely examined to quantify the associated uncertainties.
+Molar absorptivity is recalibrated as a function of compositional parameters by
+applying a Newtonian inversion, allowing for the quantification of the
+uncertainty of the inversion and of the uncertainty in composition. PyIRoGlass
+further provides functions for processing reflectance FTIR spectra to determine
+sample wafer thickness. Development of this Bayesian method with MCMC sampling
+allows for the sampling of all possible baselines and peaks to iteratively
+solve for the best-fit parameters, presenting a promising method forward for
+robustly estimating uncertainty and accounting for covariance within fit
+parameters within a unified framework to confidently process transmission FTIR
+spectra to determine volatile concentrations with uncertainties. The open-
+source nature of the Python package allows for continuous evolution as more
+data become available. [Open_In_Colab] [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/SarahShi/PyIRoGlass/HEAD)
```

### Comparing `PyIRoGlass-0.0.1/README.md` & `PyIRoGlass-0.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # PyIRoGlass
 [![PyPI](https://badgen.net/pypi/v/PyIRoGlass)](https://pypi.org/project/PyIRoGlass/)
 [![Build Status](https://github.com/SarahShi/PyIRoGlass/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/SarahShi/PyIRoGlass/actions/workflows/main.yml)
+[![Documentation Status](https://readthedocs.org/projects/pyiroglass/badge/?version=latest)](https://pyiroglass.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/SarahShi/PyIRoGlass/branch/main/graph/badge.svg)](https://codecov.io/gh/SarahShi/PyIRoGlass/branch/main)
 
 PyIRoGlass is a Bayesian MCMC-founded Python algorithm for determining volatile concentrations and speciation for $\mathrm{H_2O_{t, 3550}}$, $\mathrm{H_2O_{m, 1635}}$, $\mathrm{CO_{3, 1515}^{2-}}$, $\mathrm{CO_{3, 1430}^{2-}}$, $\mathrm{H_2O_{m, 5200}}$, and $\mathrm{OH_{4500}}$ from basaltic to andesitic transmission FTIR spectra. PyIRoGlass is written in the open-source language Python3 with the $\mathrm{MC^3}$ package, allowing for the proper sampling of parameter space and the determination of volatile concentrations with uncertainties. 
 
 
 Quantifying concentrations of volatiles in magmas is critical for estimating the conditions of magma storage, assessing phase equilibria, and understanding eruption. We develop and present PyIRoGlass, a new open-source Python package implementing a Bayesian method with Markov Chain Monte Carlo sampling, to process the transmission FTIR spectra of basaltic to andesitic glasses and to quantify volatile concentrations with uncertainties for all $\mathrm{H_2O}$ and $\mathrm{CO_2}$ species in basaltic to andesitic glasses, when devolatilized baselines are not readily available. We utilize spectra of natural, devolatilized melt inclusions from the Aleutians to determine the fundamental shapes and variability of the baseline in the mid-IR region, in which the $\mathrm{CO_3^{2-}}$ doublets and $\mathrm{H_2O_{m, 1635}}$ peaks are found. The shape of the baseline and that of the peaks varies across samples, dependent on the chemistry of samples and concentration of volatiles. All parameters within the Beer-Lambert Law — including the baseline, molar absorptivity, thickness, and density — are closely examined to quantify the associated uncertainties. Molar absorptivity is recalibrated as a function of compositional parameters by applying a Newtonian inversion, allowing for the quantification of the uncertainty of the inversion and of the uncertainty in composition. PyIRoGlass further provides functions for processing reflectance FTIR spectra to determine sample wafer thickness. Development of this Bayesian method with MCMC sampling allows for the sampling of all possible baselines and peaks to iteratively solve for the best-fit parameters, presenting a promising method forward for robustly estimating uncertainty and accounting for covariance within fit parameters within a unified framework to confidently process transmission FTIR spectra to determine volatile concentrations with uncertainties. The open-source nature of the Python package allows for continuous evolution as more data become available.
```

#### html2text {}

```diff
@@ -1,41 +1,43 @@
 # PyIRoGlass [![PyPI](https://badgen.net/pypi/v/PyIRoGlass)](https://pypi.org/
 project/PyIRoGlass/) [![Build Status](https://github.com/SarahShi/PyIRoGlass/
 actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/SarahShi/
-PyIRoGlass/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/
-SarahShi/PyIRoGlass/branch/main/graph/badge.svg)](https://codecov.io/gh/
-SarahShi/PyIRoGlass/branch/main) PyIRoGlass is a Bayesian MCMC-founded Python
-algorithm for determining volatile concentrations and speciation for $\mathrm
-{H_2O_{t, 3550}}$, $\mathrm{H_2O_{m, 1635}}$, $\mathrm{CO_{3, 1515}^{2-}}$,
-$\mathrm{CO_{3, 1430}^{2-}}$, $\mathrm{H_2O_{m, 5200}}$, and $\mathrm{OH_
-{4500}}$ from basaltic to andesitic transmission FTIR spectra. PyIRoGlass is
-written in the open-source language Python3 with the $\mathrm{MC^3}$ package,
-allowing for the proper sampling of parameter space and the determination of
-volatile concentrations with uncertainties. Quantifying concentrations of
-volatiles in magmas is critical for estimating the conditions of magma storage,
-assessing phase equilibria, and understanding eruption. We develop and present
-PyIRoGlass, a new open-source Python package implementing a Bayesian method
-with Markov Chain Monte Carlo sampling, to process the transmission FTIR
-spectra of basaltic to andesitic glasses and to quantify volatile
-concentrations with uncertainties for all $\mathrm{H_2O}$ and $\mathrm{CO_2}$
-species in basaltic to andesitic glasses, when devolatilized baselines are not
-readily available. We utilize spectra of natural, devolatilized melt inclusions
-from the Aleutians to determine the fundamental shapes and variability of the
-baseline in the mid-IR region, in which the $\mathrm{CO_3^{2-}}$ doublets and
-$\mathrm{H_2O_{m, 1635}}$ peaks are found. The shape of the baseline and that
-of the peaks varies across samples, dependent on the chemistry of samples and
-concentration of volatiles. All parameters within the Beer-Lambert Law â
-including the baseline, molar absorptivity, thickness, and density â are
-closely examined to quantify the associated uncertainties. Molar absorptivity
-is recalibrated as a function of compositional parameters by applying a
-Newtonian inversion, allowing for the quantification of the uncertainty of the
-inversion and of the uncertainty in composition. PyIRoGlass further provides
-functions for processing reflectance FTIR spectra to determine sample wafer
-thickness. Development of this Bayesian method with MCMC sampling allows for
-the sampling of all possible baselines and peaks to iteratively solve for the
-best-fit parameters, presenting a promising method forward for robustly
-estimating uncertainty and accounting for covariance within fit parameters
-within a unified framework to confidently process transmission FTIR spectra to
-determine volatile concentrations with uncertainties. The open-source nature of
-the Python package allows for continuous evolution as more data become
-available. [Open_In_Colab] [![Binder](https://mybinder.org/badge_logo.svg)]
-(https://mybinder.org/v2/gh/SarahShi/PyIRoGlass/HEAD)
+PyIRoGlass/actions/workflows/main.yml) [![Documentation Status](https://
+readthedocs.org/projects/pyiroglass/badge/?version=latest)](https://
+pyiroglass.readthedocs.io/en/latest/?badge=latest) [![codecov](https://
+codecov.io/gh/SarahShi/PyIRoGlass/branch/main/graph/badge.svg)](https://
+codecov.io/gh/SarahShi/PyIRoGlass/branch/main) PyIRoGlass is a Bayesian MCMC-
+founded Python algorithm for determining volatile concentrations and speciation
+for $\mathrm{H_2O_{t, 3550}}$, $\mathrm{H_2O_{m, 1635}}$, $\mathrm{CO_{3,
+1515}^{2-}}$, $\mathrm{CO_{3, 1430}^{2-}}$, $\mathrm{H_2O_{m, 5200}}$, and
+$\mathrm{OH_{4500}}$ from basaltic to andesitic transmission FTIR spectra.
+PyIRoGlass is written in the open-source language Python3 with the $\mathrm
+{MC^3}$ package, allowing for the proper sampling of parameter space and the
+determination of volatile concentrations with uncertainties. Quantifying
+concentrations of volatiles in magmas is critical for estimating the conditions
+of magma storage, assessing phase equilibria, and understanding eruption. We
+develop and present PyIRoGlass, a new open-source Python package implementing a
+Bayesian method with Markov Chain Monte Carlo sampling, to process the
+transmission FTIR spectra of basaltic to andesitic glasses and to quantify
+volatile concentrations with uncertainties for all $\mathrm{H_2O}$ and $\mathrm
+{CO_2}$ species in basaltic to andesitic glasses, when devolatilized baselines
+are not readily available. We utilize spectra of natural, devolatilized melt
+inclusions from the Aleutians to determine the fundamental shapes and
+variability of the baseline in the mid-IR region, in which the $\mathrm{CO_3^
+{2-}}$ doublets and $\mathrm{H_2O_{m, 1635}}$ peaks are found. The shape of the
+baseline and that of the peaks varies across samples, dependent on the
+chemistry of samples and concentration of volatiles. All parameters within the
+Beer-Lambert Law â including the baseline, molar absorptivity, thickness, and
+density â are closely examined to quantify the associated uncertainties.
+Molar absorptivity is recalibrated as a function of compositional parameters by
+applying a Newtonian inversion, allowing for the quantification of the
+uncertainty of the inversion and of the uncertainty in composition. PyIRoGlass
+further provides functions for processing reflectance FTIR spectra to determine
+sample wafer thickness. Development of this Bayesian method with MCMC sampling
+allows for the sampling of all possible baselines and peaks to iteratively
+solve for the best-fit parameters, presenting a promising method forward for
+robustly estimating uncertainty and accounting for covariance within fit
+parameters within a unified framework to confidently process transmission FTIR
+spectra to determine volatile concentrations with uncertainties. The open-
+source nature of the Python package allows for continuous evolution as more
+data become available. [Open_In_Colab] [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/SarahShi/PyIRoGlass/HEAD)
```

### Comparing `PyIRoGlass-0.0.1/setup.py` & `PyIRoGlass-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `PyIRoGlass-0.0.1/src/PyIRoGlass/BaselineAvgPCA.npz` & `PyIRoGlass-0.1.0/src/PyIRoGlass/BaselineAvgPCA.npz`

 * *Files identical despite different names*

### Comparing `PyIRoGlass-0.0.1/src/PyIRoGlass/H2Om1635PCA.npz` & `PyIRoGlass-0.1.0/src/PyIRoGlass/H2Om1635PCA.npz`

 * *Files identical despite different names*

### Comparing `PyIRoGlass-0.0.1/src/PyIRoGlass/__init__.py` & `PyIRoGlass-0.1.0/src/PyIRoGlass/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 import warnings
 
 import matplotlib as mpl
 if os.environ.get('DISPLAY','') == '':
     mpl.use('Agg')
 from matplotlib import pyplot as plt
 mpl.use('pgf')
+import mc3.plots as mp
 import mc3.utils as mu
 import mc3.stats as ms
 
 from pykrige import OrdinaryKriging
 import scipy.signal as signal
 from scipy.linalg import solveh_banded
 import scipy.interpolate as interpolate
 
-__all__ = ['trace', 'histogram', 'pairwise', 'rms', 'modelfit', 'subplotter', 'themes',]
-themes = {'blue':{'edgecolor':'navy','facecolor':'royalblue','color':'navy'},
-    'red': {'edgecolor':'crimson','facecolor':'orangered','color':'darkred'},
-    'black':{'edgecolor':'0.3','facecolor':'0.3','color':'black'},
-    'green':{'edgecolor':'forestgreen','facecolor':'limegreen','color':'darkgreen'},
-    'orange':{'edgecolor':'darkorange','facecolor':'gold','color':'darkgoldenrod'},}
+# __all__ = ['trace', 'histogram', 'pairwise', 'rms', 'modelfit', 'subplotter', 'themes',]
+# themes = {'blue':{'edgecolor':'navy','facecolor':'royalblue','color':'navy'},
+#     'red': {'edgecolor':'crimson','facecolor':'orangered','color':'darkred'},
+#     'black':{'edgecolor':'0.3','facecolor':'0.3','color':'black'},
+#     'green':{'edgecolor':'forestgreen','facecolor':'limegreen','color':'darkgreen'},
+#     'orange':{'edgecolor':'darkorange','facecolor':'gold','color':'darkgoldenrod'},}
 from ._version import __version__
 
 # %%
 
 def Load_SampleCSV(paths, wn_high, wn_low): 
 
     """
@@ -133,14 +134,15 @@
             Thickness (pd.DataFrame): The dataframe containing the thickness and standard deviation data. 
     """
 
     ChemistryThickness = pd.read_csv(ChemistryThickness_Path)
     ChemistryThickness.set_index('Sample', inplace = True)
 
     Chemistry = ChemistryThickness.loc[:, ['SiO2', 'TiO2', 'Al2O3', 'Fe2O3', 'FeO', 'MnO', 'MgO', 'CaO', 'Na2O', 'K2O', 'P2O5']]
+    Chemistry = Chemistry.fillna(0)
     Thickness = ChemistryThickness.loc[:, ['Thickness', 'Sigma_Thickness']]
 
 
     return Chemistry, Thickness
 
 def Gauss(x, mu, sd, A=1):
 
@@ -391,16 +393,17 @@
     plotindex = np.argmax(plot_output['Absorbance'].index.to_numpy() > 3400)
     PH_3550 = np.max(plot_output['Subtracted_Peak_Hat'])
 
     return data_output, plot_output, PH_3550, plotindex
 
 # %% Plotting functions 
 
+
 def trace(posterior, title, zchain=None, pnames=None, thinning=50,
-    burnin=0, fignum=1000, savefile=None, fmt=".", ms=2.5, fs=11):
+    burnin=0, fignum=1000, savefile=None, fmt=".", ms=2.5, fs=12):
     
     """
     Plot parameter trace MCMC sampling.
 
     Parameters: 
         posterior (2D np.ndarray): MCMC posterior sampling with dimension: [nsamples, npars].
         zchain (1D np.ndarray): Chain index for each posterior sample.
@@ -451,15 +454,15 @@
     for page in range(npages):
         fig = plt.figure(fignum+page, figsize=(8.5,11.0))
         plt.clf()
         plt.subplots_adjust(left=0.15, right=0.95, bottom=0.05, top=0.95, hspace=0.15)
         while ipar < npars:
             ax = plt.subplot(npanels, 1, ipar%npanels+1)
             axes.append(ax)
-            ax.plot(posterior[0::thinning,ipar], fmt, ms=ms, rasterized = True)
+            ax.plot(posterior[0::thinning,ipar], fmt, ms=ms, c='#46A4F5', rasterized = True)
             yran = ax.get_ylim()
             if zchain is not None:
                 ax.vlines(xsep, yran[0], yran[1], "0.5")
             # Y-axis adjustments:
             ax.set_ylim(yran)
             ax.locator_params(axis='y', nbins=5, tight=True)
             ax.tick_params(labelsize=fs-1, direction='in', top=True, right=True)
@@ -483,23 +486,24 @@
                     bbox.set_points(bbox_points)
                 except:  # May fail for ssh connection without X display
                     ylow = 9.479-0.862*np.amin([npanels-1,npars-npanels*page-1])
                     bbox = mpl.transforms.Bbox([[0.0, ylow], [8.5, 11]])
 
                 fig.savefig(f"{sf[0]}_page{page:02d}{sf[1]}", bbox_inches=bbox)
             else:
-                fig.suptitle(title)
+                fig.suptitle(title, fontsize=fs+1)
                 plt.ioff()
                 fig.savefig(savefile, bbox_inches='tight')
 
     return axes
 
+
 def histogram(posterior, title, pnames=None, thinning=1, fignum=1100,
     savefile=None, bestp=None, quantile=None, pdf=None,
-    xpdf=None, ranges=None, axes=None, lw=2.0, fs=11,
+    xpdf=None, ranges=None, axes=None, lw=2.0, fs=12,
     theme='blue', yscale=False, orientation='vertical'):
     
     """
     Plot parameter marginal posterior distributions in histograms. 
 
     Parameters: 
         posterior (1D/2D np.ndarray): MCMC posterior sampling with dimension [nsamples] or [nsamples, nparameters]
@@ -551,15 +555,15 @@
     if ranges is None:
         ranges = np.repeat(None, npars)
 
     # Set number of rows:
     nrows, ncolumns, npanels = 4, 4, 16
     npages = int(1 + (npars-1)/npanels)
 
-    ylabel = "$N$ samples" if yscale else "Posterior density"
+    ylabel = "$N$ samples" if yscale else "Posterior Density"
     if axes is None:
         figs, axes = [], []
         for j in range(npages):
             fig = plt.figure(fignum+j, figsize=(8.5, 11.0))
             figs.append(fig)
             fig.clf()
             fig.subplots_adjust(left=0.1, right=0.97, bottom=0.08, 
@@ -644,15 +648,15 @@
                 plt.ioff()
                 fig.savefig(savefile, bbox_inches='tight')
     
     return axes
 
 def pairwise(posterior, title, pnames=None, thinning=100, fignum=1200,
     savefile=None, bestp=None, nbins=15, nlevels=10,
-    absolute_dens=False, ranges=None, fs=11, rect=None, margin=0.01):
+    absolute_dens=False, ranges=None, fs=12, rect=None, margin=0.01):
     
     """
     Plot parameter pairwise posterior distributions.
     Parameters: 
         posterior (2D np.ndarray): An MCMC posterior sampling with dimension: [nsamples, nparameters].
         pnames (str): Label names for parameters.
         thinning (int): Thinning factor for plotting (plot every thinning-th value).
@@ -764,15 +768,15 @@
         dy = (rect[3]-rect[1])*0.45
         ax2 = plt.axes([rect[2]-dx, rect[3]-dy, dx, dy])
     else:
         ax2 = plt.axes([0.95, 0.57, 0.025, 0.36])
     cb = mpl.colorbar.ColorbarBase(
         ax2, cmap=palette, norm=norm,
         spacing='proportional', boundaries=bounds, format='%.1f')
-    cb.set_label("Posterior density", fontsize=fs)
+    cb.set_label("Posterior Density", fontsize=fs)
     cb.ax.yaxis.set_ticks_position('left')
     cb.ax.yaxis.set_label_position('left')
     cb.ax.tick_params(labelsize=fs-1, direction='in', top=True, right=True)
     cb.set_ticks(np.linspace(0, 1, 5))
     for c in ax2.collections:
         c.set_edgecolor("face")
     plt.draw()
@@ -817,30 +821,30 @@
 
     # Residuals:
     rax = plt.axes([0.15, 0.1, 0.8, 0.2])
     rax.errorbar(binindp, bindata-binmodel, binuncert, fmt='ko', ms=4)
     rax.plot([indparams[0], indparams[-1]], [0,0], 'k:', lw=1.5)
     rax.tick_params(labelsize=fs-1, direction='in', top=True, right=True)
     rax.set_xlabel("Wavenumber $(\mathregular{cm^{-1}})$", fontsize=fs)
-    rax.set_ylabel('Absorbance Residual', fontsize=fs)
+    rax.set_ylabel('Residual', fontsize=fs)
     rax.invert_xaxis()
 
     # Data and Model:
     ax = plt.axes([0.15, 0.35, 0.8, 0.575])
     ax.errorbar(binindp, bindata, binuncert, fmt = 'ko', ms=4, label='Binned data')
     ax.plot(indparams, data, 'tab:blue', lw=3, label = 'Data')
     ax.plot(indparams, model, 'tab:purple', linestyle = '-.', lw=3, label='Best Fit')
     ax.set_xticklabels([])
     ax.invert_xaxis()
     ax.tick_params(labelsize=fs-1, direction='in', top=True, right=True)
     ax.set_ylabel('Absorbance', fontsize=fs)
     ax.legend(loc='best')
 
     if savefile is not None:
-        plt.suptitle(title)
+        plt.suptitle(title, fontsize=fs+1)
         plt.ioff()
         plt.savefig(savefile)
     return ax, rax
 
 def subplotter(rect, margin, ipan, nx, ny=None, ymargin=None):
     
     """
@@ -876,14 +880,15 @@
     yloc = (ny-1) - ((ipan-1) // nx)
     # Bottom-left corner of panel:
     xpanel = rect[0] + xloc*(dx+ margin)
     ypanel = rect[1] + yloc*(dy+ymargin)
 
     return plt.axes([xpanel, ypanel, dx, dy])
 
+
 # %%
 
 def MCMC(data, uncert, indparams, log, savefile):
     
     """
     Runs Monte Carlo-Markov Chain and outputs the best fit parameters and standard deviations.
 
@@ -898,35 +903,39 @@
     Returns:
         mc3_output (mc3.output): The output of the Monte Carlo-Markov Chain.
     
     """
 
     # Define initial values, limits, and step sizes for parameters
     func = Carbonate
-    
-    params = np.array([1.25, 2.00, 0.25, 0.01, 0.01, 1430, 25.0, 0.0100, 1510, 25.0, 0.0100, 0.10, 0.02, 0.01, 5e-4, 0.70])
-    pmin = np.array([0.00, -5.00, -1.00, -0.75, -0.75, 1415, 22.5, 0.0000, 1500, 22.5, 0.0000, 0.00, -0.50, -0.50, -5e-2, -1.00])
-    pmax = np.array([5.00, 8.00, 1.00, 0.75, 0.75, 1445, 40.0, 3.0000, 1535, 40.0, 3.0000, 3.00, 0.50, 0.50, 5e-2, 3.00])
-    pstep = np.array([0.30, 0.50, 0.20, 0.20, 0.20, 3.25, 2.25, 0.0005, 6.0, 2.25, 0.0005, 0.25, 0.75, 0.75, 0.002, 0.20])
 
-    # Define prior limits for parameters
-    priorlow = np.array([0.00, 0.00, 0.00, 0.00, 0.00, 0.0, 2.5, 0.0, 0.0, 2.5, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0])
-    priorup = np.array([0.00, 0.00, 0.00, 0.00, 0.00, 0.0, 2.5, 0.0, 0.0, 2.5, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0])
-
-    pnames   = ['Avg_BL',"PCA1","PCA2","PCA3","PCA4",'peak_G1430','std_G1430','G1430_amplitude','peak_G1515','std_G1515','G1515_amplitude','Average_1635Peak','1635PeakPCA1','1635PeakPCA2','m','b']
+    params = np.array([1.25,  2.00,  0.25,  0.01,  0.01, 1430, 30.0, 0.0100, 1510, 30.0, 0.0100, 0.10,  0.02,  0.01,  5e-4,  0.70])
+    pmin   = np.array([0.00, -8.00, -2.00, -1.0, -0.75, 1415, 22.5, 0.0000, 1500, 22.5, 0.0000, 0.00, -0.50, -0.50, -5e-2, -1.00])
+    pmax   = np.array([5.00,  8.00,  2.00,  1.0,  0.75, 1445, 40.0, 3.0000, 1535, 40.0, 3.0000, 3.00,  0.50,  0.50,  5e-2,  3.00])
+    pstep  = np.abs(pmin - pmax) * 0.01
 
-    texnames = ['$\overline{B}$',"$\overline{B}_{PC1}$","$\overline{B}_{PC2}$","$\overline{B}_{PC3}$",'$\overline{B}_{PC4}$','$\mu_{1430}$','$\sigma_{1430}$','$a_{1430}$','$\mu_{1515}$','$\sigma_{1515}$','$a_{1515}$','$\overline{H_{1635}}$','$\overline{H_{1635}}_{PC1}$','$\overline{H_{1635}}_{PC2}$','$m$','$b$']
+    # Define prior limits for parameters
+    prior    = np.array([0.00, 0.00, 0.00, 0.00, 0.00, 0.0, 30.0, 0.0, 0.0, 30.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0])
+    priorlow = np.array([0.00, 0.00, 0.00, 0.00, 0.00, 0.0, 5.00, 0.0, 0.0, 5.00, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0])
+    priorup  = np.array([0.00, 0.00, 0.00, 0.00, 0.00, 0.0, 5.00, 0.0, 0.0, 5.00, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0])
+
+    pnames   = ['B_mean',"B_PC1","B_PC2","B_PC3","B_PC4",'G1430_peak','G1430_std','G1430_amp',
+                'G1515_peak','G1515_std','G1515_amp','H1635_mean','H1635_PC1','H1635_PC2','m','b']
+
+    texnames = ['$\overline{B}$',"$\overline{B}_{PC1}$","$\overline{B}_{PC2}$","$\overline{B}_{PC3}$",'$\overline{B}_{PC4}$',
+                '$\mu_{1430}$','$\sigma_{1430}$','$a_{1430}$','$\mu_{1515}$','$\sigma_{1515}$','$a_{1515}$',
+                '$\overline{H_{1635}}$','$\overline{H_{1635}}_{PC1}$','$\overline{H_{1635}}_{PC2}$','$m$','$b$']
 
 
     mc3_output = mc3.sample(data=data, uncert=uncert, func=func, params=params, indparams=indparams,
-                            pmin=pmin, pmax=pmax, priorlow=priorlow, priorup=priorup,
+                            pmin=pmin, pmax=pmax, pstep=pstep, prior=prior, priorlow=priorlow, priorup=priorup, #
                             pnames=pnames, texnames=texnames, sampler='snooker', rms=False,
-                            nsamples=1e6, nchains=9, ncpu=3, burnin=5000, thinning=5,
-                            leastsq='trf', chisqscale=False, grtest=True, grbreak=1.01, grnmin=0.5,
-                            hsize=10, kickoff='normal', wlike=False, plots=False, log=log, savefile=savefile)
+                            nsamples=1e6, nchains=9, ncpu=4, burnin=1e4, thinning=5, leastsq='trf',
+                            chisqscale=False, grtest=True, grbreak=1.01, grnmin=0.5, hsize=10,
+                            kickoff='normal', wlike=False, plots=False, log=log, savefile=savefile)
 
     return mc3_output
 
 def Run_All_Spectra(dfs_dict, exportpath):
 
     """
     The Run_All_Spectra function inputs the dictionary of dataframes that were created by the Load_SampleCSV function and allows 
@@ -948,14 +957,17 @@
     from matplotlib import pyplot as plt
     import scipy.interpolate as interpolate
     from scipy.linalg import solveh_banded
 
     import os 
     import time
     import warnings
+    import mc3.plots as mp
+    import mc3.utils as mu
+    import mc3.stats as ms
 
     path_beg = os.getcwd() + '/'
 
     # Load files with PCA vectors for the baseline and H2Om, 1635 peak. 
     Wavenumber = Load_Wavenumber('BaselineAvgPCA.npz')
     PCAmatrix = Load_PCA('BaselineAvgPCA.npz')
     Peak_1635_PCAmatrix = Load_PCA('H2Om1635PCA.npz')
@@ -1068,35 +1080,34 @@
             elif spec.shape[0] == df_length: 
                 spec_mc3 = spec['Absorbance'].to_numpy()
             
             # Set uncertainty 
             uncert = np.ones_like(spec_mc3) * 0.01
 
             # Run PyIRoGlass MC3!!!
-
             if exportpath is not None: 
+                warnings.filterwarnings("ignore", category = DeprecationWarning)
                 # Create output directories for resulting files
-                output_dir = ["FIGURES", "PLOTFILES", "NPZFILES", "LOGFILES"] 
+                output_dir = ["FIGURES", "PLOTFILES", "NPZTXTFILES", "LOGFILES"] 
                 for ii in range(len(output_dir)):
                     if not os.path.exists(path_beg + output_dir[ii] + '/' + exportpath):
                         os.makedirs(path_beg + output_dir[ii] + '/' + exportpath, exist_ok=True)
 
-                plotpath = 'PLOTFILES/' + exportpath + '/'
-                logpath = 'LOGFILES/' + exportpath + '/'
-                savefilepath = 'NPZFILES/' + exportpath + '/'
-                figurepath = 'FIGURES/' + exportpath + '/'
+                figurepath     = 'FIGURES/' + exportpath + '/'
+                plotpath       = 'PLOTFILES/' + exportpath + '/'
+                savefilepath   = 'NPZTXTFILES/' + exportpath + '/'
+                logpath        = 'LOGFILES/' + exportpath + '/'
 
                 additional_dir = ["TRACE", "HISTOGRAM", "PAIRWISE", "MODELFIT"]
                 for ii in range(len(additional_dir)): 
                     if not os.path.exists(path_beg+plotpath+additional_dir[ii]): 
                         os.makedirs(path_beg+plotpath+additional_dir[ii], exist_ok=True)
 
-
-                mc3_output = MCMC(data = spec_mc3, uncert = uncert, indparams = indparams, 
-                                log = path_beg+logpath+files+'.log', savefile=path_beg+savefilepath+files+'.npz')
+                mc3_output = MCMC(data=spec_mc3, uncert=uncert, indparams=indparams, 
+                                log=path_beg+logpath+files+'.log', savefile=path_beg+savefilepath+files+'.npz')
             else: 
                 mc3_output = MCMC(data = spec_mc3, uncert = uncert, indparams = indparams, 
                                 log=None, savefile=None)
 
             # Save best-fit concentration outputs and calculate best-fit baselines and peaks for plotting
             CO2P_BP = mc3_output['bestp'][-11:-5]
             H2OmP1635_BP = mc3_output['bestp'][-5:-2]
@@ -1125,17 +1136,18 @@
             MAX_1515_ABS = spec['Absorbance'].to_numpy()[np.argmax((spec.index.to_numpy() > 1510) & (spec.index.to_numpy() < 1530))]
             MAX_1430_ABS = spec['Absorbance'].to_numpy()[np.argmax((spec.index.to_numpy() > 1410) & (spec.index.to_numpy() < 1440))]
 
             BL_MAX_1515_ABS = Baseline_Solve_BP[np.argmax((spec.index.to_numpy() > 1510) & (spec.index.to_numpy() < 1530))]
             BL_MAX_1430_ABS = Baseline_Solve_BP[np.argmax((spec.index.to_numpy() > 1410) & (spec.index.to_numpy() < 1450))]
             BL_MAX_1635_ABS = Baseline_Solve_BP[np.argmax(H1635_BP)]
 
+            warnings.filterwarnings( "ignore", module = "matplotlib\..*" )
+
             # Initialize plotting, create subplots of H2Om_{5200} and OH_{4500} baselines and peak fits
             if exportpath is not None: 
-
                 plotmin = np.round(np.min(data[H2O4500_wn_low_1:H2O5200_wn_high_1]['Absorbance']), decimals = 1)
                 plotmax = np.round(np.max(data[H2O4500_wn_low_1:H2O5200_wn_high_1]['Absorbance']), decimals = 1)
                 fig, ax = plt.subplots(figsize = (26, 8))
                 ax1 = plt.subplot2grid((2, 3), (0, 0))
                 ax1.plot(data.index, data['Absorbance'], 'k', linewidth = 1.5)
                 ax1.plot(data_H2O5200_1.index, data_H2O5200_1['Absorbance_Hat'], 
                         data_H2O5200_2.index, data_H2O5200_2['Absorbance_Hat'], 
@@ -1197,19 +1209,24 @@
                 ax3.set_xlim([1275, 4000])
                 ax3.set_ylabel('Absorbance')
                 ax3.set_ylim([plotmin-0.25, plotmax+0.5])
                 ax3.legend(loc = 'upper right', prop={'size': 10})
                 ax3.invert_xaxis()
 
                 # Load posterior errors and sampling errors to plot the range in iterated baselines. 
-                posteriorerror = np.load(path_beg+savefilepath+files+'.npz')
-                samplingerror = posteriorerror['posterior'][:, 0:5]
-                samplingerror = samplingerror[0: np.shape(posteriorerror['posterior'][:, :])[0] :int(np.shape(posteriorerror['posterior'][:, :])[0] / 200), :]
-                lineerror = posteriorerror['posterior'][:, -2:None]
-                lineerror = lineerror[0:np.shape(posteriorerror['posterior'][:, :])[0]:int(np.shape(posteriorerror['posterior'][:, :])[0] / 200), :]
+                mcmc_npz = np.load(path_beg+savefilepath+files+'.npz')
+                posterior = mcmc_npz['posterior']
+                mask = mcmc_npz['zmask']
+                masked_posterior = posterior[mask]
+
+                samplingerror = masked_posterior[:, 0:5]
+                samplingerror = samplingerror[0: np.shape(masked_posterior[:, :])[0]:int(np.shape(masked_posterior[:, :])[0] / 100), :]
+                lineerror = masked_posterior[:, -2:None]
+                lineerror = lineerror[0:np.shape(masked_posterior[:, :])[0]:int(np.shape(masked_posterior[:, :])[0] / 100), :]
+
                 Baseline_Array = np.array(samplingerror * PCAmatrix[:, :].T)
                 Baseline_Array_Plot = Baseline_Array
 
                 ax4 = plt.subplot2grid((2, 3), (0, 2), rowspan = 2)
                 for i in range(np.shape(Baseline_Array)[0]):
                     Linearray = Linear(Wavenumber, lineerror[i, 0], lineerror[i, 1])
                     Baseline_Array_Plot[i, :] = Baseline_Array[i, :] + Linearray
@@ -1230,23 +1247,31 @@
                 ax4.invert_xaxis()
                 plt.tight_layout()
                 plt.savefig(path_beg + figurepath + files + '.pdf')
                 plt.close('all')
 
                 texnames = ['$\overline{B}$',"$\overline{B}_{PC1}$","$\overline{B}_{PC2}$","$\overline{B}_{PC3}$",'$\overline{B}_{PC4}$','$\mu_{1430}$','$\sigma_{1430}$','$a_{1430}$','$\mu_{1515}$','$\sigma_{1515}$','$a_{1515}$','$\overline{H_{1635}}$','$\overline{H_{1635}}_{PC1}$','$\overline{H_{1635}}_{PC2}$','$m$','$b$']
 
-                fig1 = trace(mc3_output['posterior'], title = files, zchain=mc3_output['zchain'], burnin=mc3_output['burnin'], 
-                            pnames=texnames, savefile=path_beg+plotpath+'TRACE/'+files+'_trace.pdf')
+                posterior, zchain, zmask = mu.burn(mc3_output)
+                post = mp.Posterior(posterior, texnames)
+
+                fig = post.plot()
+                plt.suptitle(files)
+                plt.savefig(path_beg+plotpath+'PAIRWISE/'+files+'_pairwise.pdf')
                 plt.close('all')
-                fig2 = histogram(mc3_output['posterior'], title = files, pnames=texnames, bestp=mc3_output['bestp'], 
-                                savefile=path_beg+plotpath+'HISTOGRAM/'+files+'_histogram.pdf', quantile=0.683)
+
+                fig = post.plot_histogram(nx = 4, ny = 4)
+                plt.suptitle(files, y=1.015)
+                plt.savefig(path_beg+plotpath+'HISTOGRAM/'+files+'_histogram.pdf', bbox_inches='tight')
                 plt.close('all')
-                fig3 = pairwise(mc3_output['posterior'], title = files, pnames=texnames, bestp=mc3_output['bestp'], 
-                                savefile=path_beg+plotpath+'PAIRWISE/'+files+'_pairwise.pdf')
+            
+                fig3 = trace(mc3_output['posterior'], title = files, zchain=mc3_output['zchain'], burnin=mc3_output['burnin'], 
+                            pnames=texnames, savefile=path_beg+plotpath+'TRACE/'+files+'_trace.pdf')
                 plt.close('all')
+
                 fig4 = modelfit(spec_mc3, uncert, indparams[0], mc3_output['best_model'], title = files, 
                                 savefile=path_beg+plotpath+'MODELFIT/'+files+'_modelfit.pdf')
                 plt.close('all')
 
             else: 
                 pass 
 
@@ -1399,18 +1424,18 @@
     gfw_tot = gfw.sum(axis = 1)
     
     # Calculate density of glass, convert by multiplying by 1000 for values in kg/m^3
     density = 1000 * gfw_tot / xivbari_tot
 
     return mol, density
 
-def Epsilon_Calc(MI_Composition, T, P):
+def Epsilon_Calculation(MI_Composition, T, P):
 
     """
-    The Epsilon_Calc function computes the extinction coefficients and their uncertainties for various molecular 
+    The Epsilon_Calculation function computes the extinction coefficients and their uncertainties for various molecular 
     species in a given MI or glass composition dataset. 
 
     Parameters:
         MI_Composition (dictionary): Dictionary containing the weight percentages of each oxide in the glass composition
         T (int): temperature at which the density is calculated (in Celsius)
         P (int): pressure at which the density is calculated (in bars)
     
@@ -1490,15 +1515,15 @@
                                     'epsilon_H2OT_3550': epsilon_H2OT_3550, 'sigma_epsilon_H2OT_3550': CT68_3550,
                                     'epsilon_H2Om_1635': epsilon_H2Om_1635, 'sigma_epsilon_H2Om_1635': CT68_1635,
                                     'epsilon_CO2': epsilon_CO2, 'sigma_epsilon_CO2': CT68_CO2,
                                     'epsilon_H2Om_5200': epsilon_H2Om_5200, 'sigma_epsilon_H2Om_5200': CT68_5200,
                                     'epsilon_OH_4500': epsilon_OH_4500,'sigma_epsilon_OH_4500': CT68_4500
                                     })
 
-        return epsilon
+    return epsilon
 
 def Concentration_Output(Volatiles_DF, N, thickness, MI_Composition, T, P):
 
     """
     The Concentration_Output function inputs the peak heights for the total H2O peak (3550 cm^-1), molecular H2O peak (1635 cm^-1), 
     and carbonate peaks (1515 and 1430 cm^-1), number of samples for the Monte Carlo, thickness information, and MI composition, and 
     outputs the concentrations and uncertainties for each peak. 
@@ -2280,8 +2305,8 @@
     epsilon_final_estimate = Calculate_Epsilon(mest_f, comp)
     residuals = epsilon_final_estimate - epsilon
     E_calib = Calculate_Calibration_Error(covepsilon_est_f)
     SEE_inv = Calculate_SEE(residuals)
     R2_inv = Calculate_R2(epsilon, epsilon_final_estimate)
     RMSE_inv = Calculate_RMSE(residuals)
 
-    return E_calib, SEE_inv, R2_inv, RMSE_inv
+    return E_calib, SEE_inv, R2_inv, RMSE_inv
```

### Comparing `PyIRoGlass-0.0.1/src/PyIRoGlass.egg-info/PKG-INFO` & `PyIRoGlass-0.1.0/src/PyIRoGlass.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: PyIRoGlass
-Version: 0.0.1
+Version: 0.1.0
 Summary: PyIRoGlass
 Home-page: https://github.com/sarahshi/PyIRoGlass
 Author: Sarah C. Shi
 Author-email: sarah.c.shi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # PyIRoGlass
 [![PyPI](https://badgen.net/pypi/v/PyIRoGlass)](https://pypi.org/project/PyIRoGlass/)
 [![Build Status](https://github.com/SarahShi/PyIRoGlass/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/SarahShi/PyIRoGlass/actions/workflows/main.yml)
+[![Documentation Status](https://readthedocs.org/projects/pyiroglass/badge/?version=latest)](https://pyiroglass.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/SarahShi/PyIRoGlass/branch/main/graph/badge.svg)](https://codecov.io/gh/SarahShi/PyIRoGlass/branch/main)
 
 PyIRoGlass is a Bayesian MCMC-founded Python algorithm for determining volatile concentrations and speciation for $\mathrm{H_2O_{t, 3550}}$, $\mathrm{H_2O_{m, 1635}}$, $\mathrm{CO_{3, 1515}^{2-}}$, $\mathrm{CO_{3, 1430}^{2-}}$, $\mathrm{H_2O_{m, 5200}}$, and $\mathrm{OH_{4500}}$ from basaltic to andesitic transmission FTIR spectra. PyIRoGlass is written in the open-source language Python3 with the $\mathrm{MC^3}$ package, allowing for the proper sampling of parameter space and the determination of volatile concentrations with uncertainties. 
 
 
 Quantifying concentrations of volatiles in magmas is critical for estimating the conditions of magma storage, assessing phase equilibria, and understanding eruption. We develop and present PyIRoGlass, a new open-source Python package implementing a Bayesian method with Markov Chain Monte Carlo sampling, to process the transmission FTIR spectra of basaltic to andesitic glasses and to quantify volatile concentrations with uncertainties for all $\mathrm{H_2O}$ and $\mathrm{CO_2}$ species in basaltic to andesitic glasses, when devolatilized baselines are not readily available. We utilize spectra of natural, devolatilized melt inclusions from the Aleutians to determine the fundamental shapes and variability of the baseline in the mid-IR region, in which the $\mathrm{CO_3^{2-}}$ doublets and $\mathrm{H_2O_{m, 1635}}$ peaks are found. The shape of the baseline and that of the peaks varies across samples, dependent on the chemistry of samples and concentration of volatiles. All parameters within the Beer-Lambert Law — including the baseline, molar absorptivity, thickness, and density — are closely examined to quantify the associated uncertainties. Molar absorptivity is recalibrated as a function of compositional parameters by applying a Newtonian inversion, allowing for the quantification of the uncertainty of the inversion and of the uncertainty in composition. PyIRoGlass further provides functions for processing reflectance FTIR spectra to determine sample wafer thickness. Development of this Bayesian method with MCMC sampling allows for the sampling of all possible baselines and peaks to iteratively solve for the best-fit parameters, presenting a promising method forward for robustly estimating uncertainty and accounting for covariance within fit parameters within a unified framework to confidently process transmission FTIR spectra to determine volatile concentrations with uncertainties. The open-source nature of the Python package allows for continuous evolution as more data become available.
```

#### html2text {}

```diff
@@ -1,46 +1,48 @@
-Metadata-Version: 2.1 Name: PyIRoGlass Version: 0.0.1 Summary: PyIRoGlass Home-
+Metadata-Version: 2.1 Name: PyIRoGlass Version: 0.1.0 Summary: PyIRoGlass Home-
 page: https://github.com/sarahshi/PyIRoGlass Author: Sarah C. Shi Author-email:
 sarah.c.shi@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown #
 PyIRoGlass [![PyPI](https://badgen.net/pypi/v/PyIRoGlass)](https://pypi.org/
 project/PyIRoGlass/) [![Build Status](https://github.com/SarahShi/PyIRoGlass/
 actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/SarahShi/
-PyIRoGlass/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/
-SarahShi/PyIRoGlass/branch/main/graph/badge.svg)](https://codecov.io/gh/
-SarahShi/PyIRoGlass/branch/main) PyIRoGlass is a Bayesian MCMC-founded Python
-algorithm for determining volatile concentrations and speciation for $\mathrm
-{H_2O_{t, 3550}}$, $\mathrm{H_2O_{m, 1635}}$, $\mathrm{CO_{3, 1515}^{2-}}$,
-$\mathrm{CO_{3, 1430}^{2-}}$, $\mathrm{H_2O_{m, 5200}}$, and $\mathrm{OH_
-{4500}}$ from basaltic to andesitic transmission FTIR spectra. PyIRoGlass is
-written in the open-source language Python3 with the $\mathrm{MC^3}$ package,
-allowing for the proper sampling of parameter space and the determination of
-volatile concentrations with uncertainties. Quantifying concentrations of
-volatiles in magmas is critical for estimating the conditions of magma storage,
-assessing phase equilibria, and understanding eruption. We develop and present
-PyIRoGlass, a new open-source Python package implementing a Bayesian method
-with Markov Chain Monte Carlo sampling, to process the transmission FTIR
-spectra of basaltic to andesitic glasses and to quantify volatile
-concentrations with uncertainties for all $\mathrm{H_2O}$ and $\mathrm{CO_2}$
-species in basaltic to andesitic glasses, when devolatilized baselines are not
-readily available. We utilize spectra of natural, devolatilized melt inclusions
-from the Aleutians to determine the fundamental shapes and variability of the
-baseline in the mid-IR region, in which the $\mathrm{CO_3^{2-}}$ doublets and
-$\mathrm{H_2O_{m, 1635}}$ peaks are found. The shape of the baseline and that
-of the peaks varies across samples, dependent on the chemistry of samples and
-concentration of volatiles. All parameters within the Beer-Lambert Law â
-including the baseline, molar absorptivity, thickness, and density â are
-closely examined to quantify the associated uncertainties. Molar absorptivity
-is recalibrated as a function of compositional parameters by applying a
-Newtonian inversion, allowing for the quantification of the uncertainty of the
-inversion and of the uncertainty in composition. PyIRoGlass further provides
-functions for processing reflectance FTIR spectra to determine sample wafer
-thickness. Development of this Bayesian method with MCMC sampling allows for
-the sampling of all possible baselines and peaks to iteratively solve for the
-best-fit parameters, presenting a promising method forward for robustly
-estimating uncertainty and accounting for covariance within fit parameters
-within a unified framework to confidently process transmission FTIR spectra to
-determine volatile concentrations with uncertainties. The open-source nature of
-the Python package allows for continuous evolution as more data become
-available. [Open_In_Colab] [![Binder](https://mybinder.org/badge_logo.svg)]
-(https://mybinder.org/v2/gh/SarahShi/PyIRoGlass/HEAD)
+PyIRoGlass/actions/workflows/main.yml) [![Documentation Status](https://
+readthedocs.org/projects/pyiroglass/badge/?version=latest)](https://
+pyiroglass.readthedocs.io/en/latest/?badge=latest) [![codecov](https://
+codecov.io/gh/SarahShi/PyIRoGlass/branch/main/graph/badge.svg)](https://
+codecov.io/gh/SarahShi/PyIRoGlass/branch/main) PyIRoGlass is a Bayesian MCMC-
+founded Python algorithm for determining volatile concentrations and speciation
+for $\mathrm{H_2O_{t, 3550}}$, $\mathrm{H_2O_{m, 1635}}$, $\mathrm{CO_{3,
+1515}^{2-}}$, $\mathrm{CO_{3, 1430}^{2-}}$, $\mathrm{H_2O_{m, 5200}}$, and
+$\mathrm{OH_{4500}}$ from basaltic to andesitic transmission FTIR spectra.
+PyIRoGlass is written in the open-source language Python3 with the $\mathrm
+{MC^3}$ package, allowing for the proper sampling of parameter space and the
+determination of volatile concentrations with uncertainties. Quantifying
+concentrations of volatiles in magmas is critical for estimating the conditions
+of magma storage, assessing phase equilibria, and understanding eruption. We
+develop and present PyIRoGlass, a new open-source Python package implementing a
+Bayesian method with Markov Chain Monte Carlo sampling, to process the
+transmission FTIR spectra of basaltic to andesitic glasses and to quantify
+volatile concentrations with uncertainties for all $\mathrm{H_2O}$ and $\mathrm
+{CO_2}$ species in basaltic to andesitic glasses, when devolatilized baselines
+are not readily available. We utilize spectra of natural, devolatilized melt
+inclusions from the Aleutians to determine the fundamental shapes and
+variability of the baseline in the mid-IR region, in which the $\mathrm{CO_3^
+{2-}}$ doublets and $\mathrm{H_2O_{m, 1635}}$ peaks are found. The shape of the
+baseline and that of the peaks varies across samples, dependent on the
+chemistry of samples and concentration of volatiles. All parameters within the
+Beer-Lambert Law â including the baseline, molar absorptivity, thickness, and
+density â are closely examined to quantify the associated uncertainties.
+Molar absorptivity is recalibrated as a function of compositional parameters by
+applying a Newtonian inversion, allowing for the quantification of the
+uncertainty of the inversion and of the uncertainty in composition. PyIRoGlass
+further provides functions for processing reflectance FTIR spectra to determine
+sample wafer thickness. Development of this Bayesian method with MCMC sampling
+allows for the sampling of all possible baselines and peaks to iteratively
+solve for the best-fit parameters, presenting a promising method forward for
+robustly estimating uncertainty and accounting for covariance within fit
+parameters within a unified framework to confidently process transmission FTIR
+spectra to determine volatile concentrations with uncertainties. The open-
+source nature of the Python package allows for continuous evolution as more
+data become available. [Open_In_Colab] [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/SarahShi/PyIRoGlass/HEAD)
```

