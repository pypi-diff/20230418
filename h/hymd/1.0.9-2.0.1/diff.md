# Comparing `tmp/hymd-1.0.9.tar.gz` & `tmp/hymd-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hymd-1.0.9.tar", last modified: Tue Apr 18 07:58:40 2023, max compression
+gzip compressed data, was "hymd-2.0.1.tar", last modified: Wed Apr  5 15:34:58 2023, max compression
```

## Comparing `hymd-1.0.9.tar` & `hymd-2.0.1.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:58:40.784863 hymd-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-18 07:52:44.000000 hymd-1.0.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-18 07:58:40.784863 hymd-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-04-18 07:52:44.000000 hymd-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:58:40.780863 hymd-1.0.9/hymd/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/compute_angle_forces.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/compute_angle_forces__double.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/compute_bond_forces.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/compute_bond_forces__double.f90
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/compute_dihedral_forces.f90
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/compute_dihedral_forces__double.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/configure_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/dipole_reconstruction.f90
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/dipole_reconstruction__double.f90
--rw-r--r--   0 runner    (1001) docker     (123)    30797 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    25060 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    27400 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/force.py
--rw-r--r--   0 runner    (1001) docker     (123)    19583 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/gaussian_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)    41528 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    34606 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 07:52:44.000000 hymd-1.0.9/hymd/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:58:40.784863 hymd-1.0.9/hymd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-18 07:58:40.000000 hymd-1.0.9/hymd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-18 07:58:40.000000 hymd-1.0.9/hymd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:58:40.000000 hymd-1.0.9/hymd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 07:58:40.000000 hymd-1.0.9/hymd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 07:58:40.000000 hymd-1.0.9/hymd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-18 07:52:44.000000 hymd-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:58:40.788863 hymd-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-18 07:52:44.000000 hymd-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:58:40.784863 hymd-1.0.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-18 07:52:44.000000 hymd-1.0.9/test/test_configure_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-04-18 07:52:44.000000 hymd-1.0.9/test/test_distribute_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-18 07:52:44.000000 hymd-1.0.9/test/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-04-18 07:52:44.000000 hymd-1.0.9/test/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-04-18 07:52:44.000000 hymd-1.0.9/test/test_force.py
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-04-18 07:52:44.000000 hymd-1.0.9/test/test_hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)    32328 2023-04-18 07:52:44.000000 hymd-1.0.9/test/test_input_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12728 2023-04-18 07:52:44.000000 hymd-1.0.9/test/test_integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-18 07:52:44.000000 hymd-1.0.9/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-18 07:52:44.000000 hymd-1.0.9/test/test_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:34:58.060209 hymd-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-05 15:29:23.000000 hymd-2.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-04-05 15:34:58.060209 hymd-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-04-05 15:29:23.000000 hymd-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:34:58.060209 hymd-2.0.1/hymd/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/barostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/barostat_scr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/compute_angle_forces.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/compute_angle_forces__double.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/compute_bond_forces.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/compute_bond_forces__double.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/compute_dihedral_forces.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/compute_dihedral_forces__double.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/configure_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/dipole_reconstruction.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/dipole_reconstruction__double.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    46365 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26666 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29848 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19583 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/gaussian_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15703 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52393 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50045 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-05 15:29:23.000000 hymd-2.0.1/hymd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:34:58.060209 hymd-2.0.1/hymd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-04-05 15:34:58.000000 hymd-2.0.1/hymd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-05 15:34:58.000000 hymd-2.0.1/hymd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 15:34:58.000000 hymd-2.0.1/hymd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-05 15:34:58.000000 hymd-2.0.1/hymd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-05 15:34:58.000000 hymd-2.0.1/hymd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-05 15:29:23.000000 hymd-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 15:34:58.060209 hymd-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-05 15:29:23.000000 hymd-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:34:58.060209 hymd-2.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_configure_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_distribute_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_force.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13946 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33165 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12728 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-05 15:29:23.000000 hymd-2.0.1/test/test_thermostat.py
```

### Comparing `hymd-1.0.9/LICENSE.txt` & `hymd-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hymd-1.0.9/PKG-INFO` & `hymd-2.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hymd
-Version: 1.0.9
+Version: 2.0.1
 Summary: Massively parallel hybrid particle-field MD
 Home-page: https://github.com/Cascella-Group-UiO/HyMD
 Author: Morten Ledum
 Author-email: morten.ledum@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -12,33 +12,37 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <a href="https://cascella-group-uio.github.io/HyMD/">
   <img src="https://github.com/Cascella-Group-UiO/HyMD/blob/main/docs/img/hymd_logo_text_black.png?raw=true" width="500" title="HylleraasMD">
 </a>
 
 [![License: GPL v3](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.html) ![build](https://github.com/Cascella-Group-UiO/HyMD-2021/workflows/build/badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/actions/workflows/docs_pages.yml/badge.svg)](https://cascella-group-uio.github.io/HyMD/) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/branch/main/graph/badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-Group-UiO/HyMD) [![PyPI version](https://badge.fury.io/py/hymd.svg)](https://badge.fury.io/py/hymd)
 
 ---------
-**HylleraasMD** (HyMD) is a massively parallel Python package for hybrid particle-field molecular dynamics (hPF-MD) simulations of coarse-grained bio- and soft-matter systems.
+**HylleraasMD** (HyMD) is a massively parallel Python package for Hamiltonian hybrid particle-field molecular dynamics (HhPF-MD) simulations of coarse-grained bio- and soft-matter systems.
 
-HyMD can run canonical hPF-MD simulations [[1]](#1), or filtered density Hamiltonian hPF (HhPF-MD) simulations [[2]](#2), with or without explicit PME electrostatic interactions [[3]](#3). It includes all standard intramolecular interactions, including stretching, bending, torsional, and combined bending-dihedral potentials. Additionally, topological reconstruction of permanent peptide chain backbone dipoles is possible for accurate recreation of protein conformational dynamics [[4]](#4). Martini style elastic networks (ElNeDyn) [[5]](#5) are also supported.
+HyMD can run canonical hPF-MD simulations, or filtered density Hamiltonian hPF (HhPF-MD) simulations [[1]](#1),[[2]](#2),[[3]](#3) with or without explicit PME electrostatic interactions. It includes all standard intramolecular interactions,
+including stretching, bending, torsional, and combined bending-dihedral potentials. Additionally, topological reconstruction of permanent peptide chain backbone dipoles is possible for accurate recreation of protein conformational dynamics.
+It can run simulations in constant energy (NVE), constant volume (NVT) [[1]](#1) or constant pressure (NPT) conditions [[4]](#4).
 
-HyMD uses the [pmesh](github.com/rainwoodman/pmesh) library for particle-mesh operations, with the PPFT [[6]](#6) backend for FFTs through the [pfft-python bindings](github.com/rainwoodman/pfft-python). File IO is done via HDF5 formats to allow MPI parallel reads.
+HyMD uses the [pmesh](github.com/rainwoodman/pmesh) library for particle-mesh operations, with the PPFT [[5]](#5) backend for FFTs through the [pfft-python bindings](github.com/rainwoodman/pfft-python).
+File IO is done via HDF5 formats to allow MPI parallel reads.
 
 ## User Guide
 Detailed installation and user guide, together with comprehensive example simulations are located in the [HylleraasMD documentation](https://cascella-group-uio.github.io/HyMD/index.html).
 
 Run simulations by
 ```bash
 python3 -m hymd [CONFIGURATION_FILE] [TOPOLOGY_FILE] (--OPTIONAL_ARGS)
@@ -94,27 +98,28 @@
 ```
 Running MPI enabled pytest tests is simplified with a convenient script
 ```bash
 chmod +x pytest-mpi
 pytest-mpi -oo -n 2 -ns
 ```
 
+## Please cite our work
+If you use HyMD for your purposes, please cite the appropriate references from the section below.  
+If you cannot cite all, the fundamental works to be cited are [[1]](#1) and [[4]](#4). 
+
 ---------
 
 ### References
 <a id="1">[1]</a>
-Milano, G.; Kawakatsu, T. Hybrid particle-field molecular dynamics simulations for dense polymer systems. J. Chem. Phys. **2009**, 130, 214106.
+Ledum, M.; Sen, S.; Li, X.; Carrer, M.; Feng Y.; Cascella, M.; Bore, S. L. HylleraasMD: A Domain Decomposition-Based Hybrid Particle-Field Software for Multi-Scale Simulations of Soft Matter. ChemRxiv 2021
 
 <a id="2">[2]</a>
-Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid particle–field molecular dynamics. J. Chem. Phys. **2020**, 153, 094106.
+Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L. HyMD: Massively parallel hybrid particle-field molecular dynamics in Python.
 
 <a id="3">[3]</a>
-Kolli, H. B.; De Nicola, A.; Bore, S. L.; Schäfer, K.; Diezemann, G.; Gauss, J.; Kawakatsu, T.;Lu, Z.-Y.; Zhu, Y.-L.; Milano, G.; Cascella, M. Hybrid Particle-Field Molecular DynamicsSimulations of Charged Amphiphiles in an Aqueous Environment. J. Chem. Theory Comput. **2018**, 14, 4928–4937.
+Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid particle–field molecular dynamics. J. Chem. Phys. 2020, 153, 094106.
 
 <a id="4">[4]</a>
-Bore, S. L.; Milano, G.; Cascella, M. Hybrid Particle-Field Model for Conformational Dynamics of Peptide Chains. J. Chem. Theory Comput. **2018**, 14, 1120–1130.
+Sen, S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure: Pushing Particle–Field Molecular Dynamics to the Isobaric Ensemble. ChemRxiv 2023
 
 <a id="5">[5]</a>
-Periole, X.; Cavalli, M.; Marrink, S. J.; Ceruso, M. A. Combining an elastic network with a coarse-grained molecular force field: structure, dynamics, and intermolecular recognition. J. Chem. Theory Comput. **2009**, 5.9, 2531-2543.
-
-<a id="6">[6]</a>
-Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM J. Sci. Comput. **2013**, 35, C213–C236.
+Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM J. Sci. Comput. 2013, 35, C213–C236.
```

#### html2text {}

```diff
@@ -1,49 +1,51 @@
-Metadata-Version: 2.1 Name: hymd Version: 1.0.9 Summary: Massively parallel
+Metadata-Version: 2.1 Name: hymd Version: 2.0.1 Summary: Massively parallel
 hybrid particle-field MD Home-page: https://github.com/Cascella-Group-UiO/HyMD
 Author: Morten Ledum Author-email: morten.ledum@gmail.com License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
 OSI Approved :: GNU Lesser General Public License v3 (LGPLv3) Classifier:
 Intended Audience :: Science/Research Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Fortran Classifier: Topic ::
-Scientific/Engineering :: Chemistry Classifier: Topic :: Scientific/Engineering
-:: Physics Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE.txt [https://github.com/Cascella-Group-UiO/HyMD/blob/
-main/docs/img/hymd_logo_text_black.png?raw=true] [![License: GPL v3](https://
-img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/
-lgpl-3.0.html) ![build](https://github.com/Cascella-Group-UiO/HyMD-2021/
-workflows/build/badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/
-actions/workflows/docs_pages.yml/badge.svg)](https://cascella-group-
-uio.github.io/HyMD/) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/
-branch/main/graph/badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-
-Group-UiO/HyMD) [![PyPI version](https://badge.fury.io/py/hymd.svg)](https://
-badge.fury.io/py/hymd) --------- **HylleraasMD** (HyMD) is a massively parallel
-Python package for hybrid particle-field molecular dynamics (hPF-MD)
-simulations of coarse-grained bio- and soft-matter systems. HyMD can run
-canonical hPF-MD simulations [[1]](#1), or filtered density Hamiltonian hPF
-(HhPF-MD) simulations [[2]](#2), with or without explicit PME electrostatic
-interactions [[3]](#3). It includes all standard intramolecular interactions,
-including stretching, bending, torsional, and combined bending-dihedral
-potentials. Additionally, topological reconstruction of permanent peptide chain
-backbone dipoles is possible for accurate recreation of protein conformational
-dynamics [[4]](#4). Martini style elastic networks (ElNeDyn) [[5]](#5) are also
-supported. HyMD uses the [pmesh](github.com/rainwoodman/pmesh) library for
-particle-mesh operations, with the PPFT [[6]](#6) backend for FFTs through the
-[pfft-python bindings](github.com/rainwoodman/pfft-python). File IO is done via
-HDF5 formats to allow MPI parallel reads. ## User Guide Detailed installation
-and user guide, together with comprehensive example simulations are located in
-the [HylleraasMD documentation](https://cascella-group-uio.github.io/HyMD/
-index.html). Run simulations by ```bash python3 -m hymd [CONFIGURATION_FILE]
-[TOPOLOGY_FILE] (--OPTIONAL_ARGS) ``` #### Run interactively in Google
-Colaboratory A [Google Colaboratory](https://colab.research.google.com/
-) jupyter notebook is setup [here](https://colab.research.google.com/drive/
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Fortran Classifier: Topic :: Scientific/Engineering ::
+Chemistry Classifier: Topic :: Scientific/Engineering :: Physics Requires-
+Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE.txt
+[https://github.com/Cascella-Group-UiO/HyMD/blob/main/docs/img/
+hymd_logo_text_black.png?raw=true] [![License: GPL v3](https://img.shields.io/
+badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.html) !
+[build](https://github.com/Cascella-Group-UiO/HyMD-2021/workflows/build/
+badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/actions/
+workflows/docs_pages.yml/badge.svg)](https://cascella-group-uio.github.io/HyMD/
+) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/branch/main/graph/
+badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-Group-UiO/HyMD) [!
+[PyPI version](https://badge.fury.io/py/hymd.svg)](https://badge.fury.io/py/
+hymd) --------- **HylleraasMD** (HyMD) is a massively parallel Python package
+for Hamiltonian hybrid particle-field molecular dynamics (HhPF-MD) simulations
+of coarse-grained bio- and soft-matter systems. HyMD can run canonical hPF-MD
+simulations, or filtered density Hamiltonian hPF (HhPF-MD) simulations [[1]]
+(#1),[[2]](#2),[[3]](#3) with or without explicit PME electrostatic
+interactions. It includes all standard intramolecular interactions, including
+stretching, bending, torsional, and combined bending-dihedral potentials.
+Additionally, topological reconstruction of permanent peptide chain backbone
+dipoles is possible for accurate recreation of protein conformational dynamics.
+It can run simulations in constant energy (NVE), constant volume (NVT) [[1]]
+(#1) or constant pressure (NPT) conditions [[4]](#4). HyMD uses the [pmesh]
+(github.com/rainwoodman/pmesh) library for particle-mesh operations, with the
+PPFT [[5]](#5) backend for FFTs through the [pfft-python bindings](github.com/
+rainwoodman/pfft-python). File IO is done via HDF5 formats to allow MPI
+parallel reads. ## User Guide Detailed installation and user guide, together
+with comprehensive example simulations are located in the [HylleraasMD
+documentation](https://cascella-group-uio.github.io/HyMD/index.html). Run
+simulations by ```bash python3 -m hymd [CONFIGURATION_FILE] [TOPOLOGY_FILE] (--
+OPTIONAL_ARGS) ``` #### Run interactively in Google Colaboratory A [Google
+Colaboratory](https://colab.research.google.com/) jupyter notebook is setup
+[here](https://colab.research.google.com/drive/
 1jfzRaXjL3q53J4U8OrCgADepmf_HuCOh?usp=sharing) with a working HyMD fully
 installed and executable in the browser. ## Installation #### Non-Python
 dependencies HyMD installation **requires** a working MPI compiler. It is
 highly recommended to have *MPI-enabled* HDF5 and [h5py](https://docs.h5py.org/
 en/stable/mpi.html) for running parallel simulations with HyMD. Install both on
 Ubuntu with ```bash sudo apt-get update -y sudo apt-get install -y pkg-config
 libhdf5-mpi-dev libopenmpi-dev python3 -m pip uninstall h5py # Remove any
@@ -63,23 +65,21 @@
 O https://raw.githubusercontent.com/Cascella-Group-UiO/HyMD-tutorial/main/
 ideal_chain/ideal_chain.HDF5 /app$ /app$ # Run simulation /app$ python3 -m hymd
 ideal_chain.toml ideal_chain.HDF5 --verbose ``` ## Run tests Clone the
 repository and run tests with [pytest](https://docs.pytest.org/en/latest)
 ```bash git clone https://github.com/Cascella-Group-UiO/HyMD.git hymd cd hymd
 python3 -m pip install pytest pytest-mpi pytest ``` Running MPI enabled pytest
 tests is simplified with a convenient script ```bash chmod +x pytest-mpi
-pytest-mpi -oo -n 2 -ns ``` --------- ### References [1] Milano, G.; Kawakatsu,
-T. Hybrid particle-field molecular dynamics simulations for dense polymer
-systems. J. Chem. Phys. **2009**, 130, 214106. [2] Bore, S. L.; Cascella, M.
-Hamiltonian and alias-free hybrid particleâfield molecular dynamics. J. Chem.
-Phys. **2020**, 153, 094106. [3] Kolli, H. B.; De Nicola, A.; Bore, S. L.;
-SchÃ¤fer, K.; Diezemann, G.; Gauss, J.; Kawakatsu, T.;Lu, Z.-Y.; Zhu, Y.-L.;
-Milano, G.; Cascella, M. Hybrid Particle-Field Molecular DynamicsSimulations of
-Charged Amphiphiles in an Aqueous Environment. J. Chem. Theory Comput.
-**2018**, 14, 4928â4937. [4] Bore, S. L.; Milano, G.; Cascella, M. Hybrid
-Particle-Field Model for Conformational Dynamics of Peptide Chains. J. Chem.
-Theory Comput. **2018**, 14, 1120â1130. [5] Periole, X.; Cavalli, M.;
-Marrink, S. J.; Ceruso, M. A. Combining an elastic network with a coarse-
-grained molecular force field: structure, dynamics, and intermolecular
-recognition. J. Chem. Theory Comput. **2009**, 5.9, 2531-2543. [6] Pippig, M.
-PFFT: An extension of FFTW to massively parallel architectures. SIAM J. Sci.
-Comput. **2013**, 35, C213âC236.
+pytest-mpi -oo -n 2 -ns ``` ## Please cite our work If you use HyMD for your
+purposes, please cite the appropriate references from the section below. If you
+cannot cite all, the fundamental works to be cited are [[1]](#1) and [[4]](#4).
+--------- ### References [1] Ledum, M.; Sen, S.; Li, X.; Carrer, M.; Feng Y.;
+Cascella, M.; Bore, S. L. HylleraasMD: A Domain Decomposition-Based Hybrid
+Particle-Field Software for Multi-Scale Simulations of Soft Matter. ChemRxiv
+2021 [2] Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L.
+HyMD: Massively parallel hybrid particle-field molecular dynamics in Python.
+[3] Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid
+particleâfield molecular dynamics. J. Chem. Phys. 2020, 153, 094106. [4] Sen,
+S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure: Pushing
+ParticleâField Molecular Dynamics to the Isobaric Ensemble. ChemRxiv 2023 [5]
+Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM
+J. Sci. Comput. 2013, 35, C213âC236.
```

### Comparing `hymd-1.0.9/README.md` & `hymd-2.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 <a href="https://cascella-group-uio.github.io/HyMD/">
   <img src="https://github.com/Cascella-Group-UiO/HyMD/blob/main/docs/img/hymd_logo_text_black.png?raw=true" width="500" title="HylleraasMD">
 </a>
 
 [![License: GPL v3](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.html) ![build](https://github.com/Cascella-Group-UiO/HyMD-2021/workflows/build/badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/actions/workflows/docs_pages.yml/badge.svg)](https://cascella-group-uio.github.io/HyMD/) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/branch/main/graph/badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-Group-UiO/HyMD) [![PyPI version](https://badge.fury.io/py/hymd.svg)](https://badge.fury.io/py/hymd)
 
 ---------
-**HylleraasMD** (HyMD) is a massively parallel Python package for hybrid particle-field molecular dynamics (hPF-MD) simulations of coarse-grained bio- and soft-matter systems.
+**HylleraasMD** (HyMD) is a massively parallel Python package for Hamiltonian hybrid particle-field molecular dynamics (HhPF-MD) simulations of coarse-grained bio- and soft-matter systems.
 
-HyMD can run canonical hPF-MD simulations [[1]](#1), or filtered density Hamiltonian hPF (HhPF-MD) simulations [[2]](#2), with or without explicit PME electrostatic interactions [[3]](#3). It includes all standard intramolecular interactions, including stretching, bending, torsional, and combined bending-dihedral potentials. Additionally, topological reconstruction of permanent peptide chain backbone dipoles is possible for accurate recreation of protein conformational dynamics [[4]](#4). Martini style elastic networks (ElNeDyn) [[5]](#5) are also supported.
+HyMD can run canonical hPF-MD simulations, or filtered density Hamiltonian hPF (HhPF-MD) simulations [[1]](#1),[[2]](#2),[[3]](#3) with or without explicit PME electrostatic interactions. It includes all standard intramolecular interactions,
+including stretching, bending, torsional, and combined bending-dihedral potentials. Additionally, topological reconstruction of permanent peptide chain backbone dipoles is possible for accurate recreation of protein conformational dynamics.
+It can run simulations in constant energy (NVE), constant volume (NVT) [[1]](#1) or constant pressure (NPT) conditions [[4]](#4).
 
-HyMD uses the [pmesh](github.com/rainwoodman/pmesh) library for particle-mesh operations, with the PPFT [[6]](#6) backend for FFTs through the [pfft-python bindings](github.com/rainwoodman/pfft-python). File IO is done via HDF5 formats to allow MPI parallel reads.
+HyMD uses the [pmesh](github.com/rainwoodman/pmesh) library for particle-mesh operations, with the PPFT [[5]](#5) backend for FFTs through the [pfft-python bindings](github.com/rainwoodman/pfft-python).
+File IO is done via HDF5 formats to allow MPI parallel reads.
 
 ## User Guide
 Detailed installation and user guide, together with comprehensive example simulations are located in the [HylleraasMD documentation](https://cascella-group-uio.github.io/HyMD/index.html).
 
 Run simulations by
 ```bash
 python3 -m hymd [CONFIGURATION_FILE] [TOPOLOGY_FILE] (--OPTIONAL_ARGS)
@@ -69,27 +72,28 @@
 ```
 Running MPI enabled pytest tests is simplified with a convenient script
 ```bash
 chmod +x pytest-mpi
 pytest-mpi -oo -n 2 -ns
 ```
 
+## Please cite our work
+If you use HyMD for your purposes, please cite the appropriate references from the section below.  
+If you cannot cite all, the fundamental works to be cited are [[1]](#1) and [[4]](#4). 
+
 ---------
 
 ### References
 <a id="1">[1]</a>
-Milano, G.; Kawakatsu, T. Hybrid particle-field molecular dynamics simulations for dense polymer systems. J. Chem. Phys. **2009**, 130, 214106.
+Ledum, M.; Sen, S.; Li, X.; Carrer, M.; Feng Y.; Cascella, M.; Bore, S. L. HylleraasMD: A Domain Decomposition-Based Hybrid Particle-Field Software for Multi-Scale Simulations of Soft Matter. ChemRxiv 2021
 
 <a id="2">[2]</a>
-Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid particle–field molecular dynamics. J. Chem. Phys. **2020**, 153, 094106.
+Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L. HyMD: Massively parallel hybrid particle-field molecular dynamics in Python.
 
 <a id="3">[3]</a>
-Kolli, H. B.; De Nicola, A.; Bore, S. L.; Schäfer, K.; Diezemann, G.; Gauss, J.; Kawakatsu, T.;Lu, Z.-Y.; Zhu, Y.-L.; Milano, G.; Cascella, M. Hybrid Particle-Field Molecular DynamicsSimulations of Charged Amphiphiles in an Aqueous Environment. J. Chem. Theory Comput. **2018**, 14, 4928–4937.
+Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid particle–field molecular dynamics. J. Chem. Phys. 2020, 153, 094106.
 
 <a id="4">[4]</a>
-Bore, S. L.; Milano, G.; Cascella, M. Hybrid Particle-Field Model for Conformational Dynamics of Peptide Chains. J. Chem. Theory Comput. **2018**, 14, 1120–1130.
+Sen, S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure: Pushing Particle–Field Molecular Dynamics to the Isobaric Ensemble. ChemRxiv 2023
 
 <a id="5">[5]</a>
-Periole, X.; Cavalli, M.; Marrink, S. J.; Ceruso, M. A. Combining an elastic network with a coarse-grained molecular force field: structure, dynamics, and intermolecular recognition. J. Chem. Theory Comput. **2009**, 5.9, 2531-2543.
-
-<a id="6">[6]</a>
-Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM J. Sci. Comput. **2013**, 35, C213–C236.
+Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM J. Sci. Comput. 2013, 35, C213–C236.
```

#### html2text {}

```diff
@@ -4,25 +4,26 @@
 [build](https://github.com/Cascella-Group-UiO/HyMD-2021/workflows/build/
 badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/actions/
 workflows/docs_pages.yml/badge.svg)](https://cascella-group-uio.github.io/HyMD/
 ) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/branch/main/graph/
 badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-Group-UiO/HyMD) [!
 [PyPI version](https://badge.fury.io/py/hymd.svg)](https://badge.fury.io/py/
 hymd) --------- **HylleraasMD** (HyMD) is a massively parallel Python package
-for hybrid particle-field molecular dynamics (hPF-MD) simulations of coarse-
-grained bio- and soft-matter systems. HyMD can run canonical hPF-MD simulations
-[[1]](#1), or filtered density Hamiltonian hPF (HhPF-MD) simulations [[2]](#2),
-with or without explicit PME electrostatic interactions [[3]](#3). It includes
-all standard intramolecular interactions, including stretching, bending,
-torsional, and combined bending-dihedral potentials. Additionally, topological
-reconstruction of permanent peptide chain backbone dipoles is possible for
-accurate recreation of protein conformational dynamics [[4]](#4). Martini style
-elastic networks (ElNeDyn) [[5]](#5) are also supported. HyMD uses the [pmesh]
+for Hamiltonian hybrid particle-field molecular dynamics (HhPF-MD) simulations
+of coarse-grained bio- and soft-matter systems. HyMD can run canonical hPF-MD
+simulations, or filtered density Hamiltonian hPF (HhPF-MD) simulations [[1]]
+(#1),[[2]](#2),[[3]](#3) with or without explicit PME electrostatic
+interactions. It includes all standard intramolecular interactions, including
+stretching, bending, torsional, and combined bending-dihedral potentials.
+Additionally, topological reconstruction of permanent peptide chain backbone
+dipoles is possible for accurate recreation of protein conformational dynamics.
+It can run simulations in constant energy (NVE), constant volume (NVT) [[1]]
+(#1) or constant pressure (NPT) conditions [[4]](#4). HyMD uses the [pmesh]
 (github.com/rainwoodman/pmesh) library for particle-mesh operations, with the
-PPFT [[6]](#6) backend for FFTs through the [pfft-python bindings](github.com/
+PPFT [[5]](#5) backend for FFTs through the [pfft-python bindings](github.com/
 rainwoodman/pfft-python). File IO is done via HDF5 formats to allow MPI
 parallel reads. ## User Guide Detailed installation and user guide, together
 with comprehensive example simulations are located in the [HylleraasMD
 documentation](https://cascella-group-uio.github.io/HyMD/index.html). Run
 simulations by ```bash python3 -m hymd [CONFIGURATION_FILE] [TOPOLOGY_FILE] (--
 OPTIONAL_ARGS) ``` #### Run interactively in Google Colaboratory A [Google
 Colaboratory](https://colab.research.google.com/) jupyter notebook is setup
@@ -50,23 +51,21 @@
 O https://raw.githubusercontent.com/Cascella-Group-UiO/HyMD-tutorial/main/
 ideal_chain/ideal_chain.HDF5 /app$ /app$ # Run simulation /app$ python3 -m hymd
 ideal_chain.toml ideal_chain.HDF5 --verbose ``` ## Run tests Clone the
 repository and run tests with [pytest](https://docs.pytest.org/en/latest)
 ```bash git clone https://github.com/Cascella-Group-UiO/HyMD.git hymd cd hymd
 python3 -m pip install pytest pytest-mpi pytest ``` Running MPI enabled pytest
 tests is simplified with a convenient script ```bash chmod +x pytest-mpi
-pytest-mpi -oo -n 2 -ns ``` --------- ### References [1] Milano, G.; Kawakatsu,
-T. Hybrid particle-field molecular dynamics simulations for dense polymer
-systems. J. Chem. Phys. **2009**, 130, 214106. [2] Bore, S. L.; Cascella, M.
-Hamiltonian and alias-free hybrid particleâfield molecular dynamics. J. Chem.
-Phys. **2020**, 153, 094106. [3] Kolli, H. B.; De Nicola, A.; Bore, S. L.;
-SchÃ¤fer, K.; Diezemann, G.; Gauss, J.; Kawakatsu, T.;Lu, Z.-Y.; Zhu, Y.-L.;
-Milano, G.; Cascella, M. Hybrid Particle-Field Molecular DynamicsSimulations of
-Charged Amphiphiles in an Aqueous Environment. J. Chem. Theory Comput.
-**2018**, 14, 4928â4937. [4] Bore, S. L.; Milano, G.; Cascella, M. Hybrid
-Particle-Field Model for Conformational Dynamics of Peptide Chains. J. Chem.
-Theory Comput. **2018**, 14, 1120â1130. [5] Periole, X.; Cavalli, M.;
-Marrink, S. J.; Ceruso, M. A. Combining an elastic network with a coarse-
-grained molecular force field: structure, dynamics, and intermolecular
-recognition. J. Chem. Theory Comput. **2009**, 5.9, 2531-2543. [6] Pippig, M.
-PFFT: An extension of FFTW to massively parallel architectures. SIAM J. Sci.
-Comput. **2013**, 35, C213âC236.
+pytest-mpi -oo -n 2 -ns ``` ## Please cite our work If you use HyMD for your
+purposes, please cite the appropriate references from the section below. If you
+cannot cite all, the fundamental works to be cited are [[1]](#1) and [[4]](#4).
+--------- ### References [1] Ledum, M.; Sen, S.; Li, X.; Carrer, M.; Feng Y.;
+Cascella, M.; Bore, S. L. HylleraasMD: A Domain Decomposition-Based Hybrid
+Particle-Field Software for Multi-Scale Simulations of Soft Matter. ChemRxiv
+2021 [2] Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L.
+HyMD: Massively parallel hybrid particle-field molecular dynamics in Python.
+[3] Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid
+particleâfield molecular dynamics. J. Chem. Phys. 2020, 153, 094106. [4] Sen,
+S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure: Pushing
+ParticleâField Molecular Dynamics to the Isobaric Ensemble. ChemRxiv 2023 [5]
+Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM
+J. Sci. Comput. 2013, 35, C213âC236.
```

### Comparing `hymd-1.0.9/hymd/compute_angle_forces.f90` & `hymd-2.0.1/hymd/compute_angle_forces__double.f90`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-subroutine caf(f, r, box, a, b, c, t0, k, energy)
+subroutine caf_d(f, r, box, a, b, c, t0, k, energy, angle_pr)
     ! Compute three-particle bond forces and energy
     !
     ! Parameters
     ! ---------
     ! f : (N,D) numpy.ndarray
     !     Forces for N particles in D dimensions. Changed in place.
     ! r : (N,D) numpy.ndarray
@@ -23,31 +23,33 @@
     ! Returns
     ! -------
     ! energy : float
     !     Total energy of all two-particle bonds.
     !
     implicit none
 
-    real(4), dimension(:,:),     intent(in out) :: f
-    real(4), dimension(:,:),     intent(in)     :: r
+    real(8), dimension(:,:),     intent(inout)  :: f
+    real(8), dimension(:,:),     intent(in)     :: r
     real(8), dimension(:),       intent(in)     :: box
     integer, dimension(:),       intent(in)     :: a
     integer, dimension(:),       intent(in)     :: b
     integer, dimension(:),       intent(in)     :: c
     real(8), dimension(:),       intent(in)     :: t0
     real(8), dimension(:),       intent(in)     :: k
-    real(8),                    intent(out)     :: energy
+    real(8),                     intent(out)    :: energy
+    real(8), dimension(3),       intent(out)    :: angle_pr
 
     integer :: ind, aa, bb, cc
     real(8), dimension(3) :: ra, rc, ea, ec, fa, fc
     real(8) :: d, ff, xsinph, norm_a, norm_c
     real(8) :: xrasin, xrcsin
     real(8) :: cosphi, cosphi2, sinphi, theta
 
     energy = 0.0d00
+    angle_pr = 0.0d00
     f = 0.0d00
 
     do ind = 1, size(a)
       aa = a(ind) + 1
       bb = b(ind) + 1
       cc = c(ind) + 1
 
@@ -79,10 +81,11 @@
         fc = (ea - cosphi * ec) * xrcsin
 
         f(aa, :) = f(aa, :) - fa
         f(cc, :) = f(cc, :) - fc
         f(bb, :) = f(bb, :) + fa + fc
 
         energy = energy + 0.5d0 * ff * d
+        angle_pr = angle_pr - (fa * ra) - (fc * rc)
       end if
     end do
 end subroutine
```

### Comparing `hymd-1.0.9/hymd/compute_angle_forces__double.f90` & `hymd-2.0.1/hymd/compute_angle_forces.f90`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-subroutine caf_d(f, r, box, a, b, c, t0, k, energy)
+subroutine caf(f, r, box, a, b, c, t0, k, energy, angle_pr)
     ! Compute three-particle bond forces and energy
     !
     ! Parameters
     ! ---------
     ! f : (N,D) numpy.ndarray
     !     Forces for N particles in D dimensions. Changed in place.
     ! r : (N,D) numpy.ndarray
@@ -19,35 +19,39 @@
     !     Equilibrium bond angle for M individual three-particle bonds.
     ! k : (M,) numpy.ndarray
     !     Bond strength for M individual three-particle bonds.
     !
     ! Returns
     ! -------
     ! energy : float
-    !     Total energy of all two-particle bonds.
+    !     Total energy of all three-particle bonds.
+    ! angle_pr : (3,) numpy.ndarray
+    !     Total angle pressure due all three-particle bonds.
     !
     implicit none
 
-    real(8), dimension(:,:),     intent(in out) :: f
-    real(8), dimension(:,:),     intent(in)     :: r
+    real(4), dimension(:,:),     intent(inout)  :: f
+    real(4), dimension(:,:),     intent(in)     :: r
     real(8), dimension(:),       intent(in)     :: box
     integer, dimension(:),       intent(in)     :: a
     integer, dimension(:),       intent(in)     :: b
     integer, dimension(:),       intent(in)     :: c
     real(8), dimension(:),       intent(in)     :: t0
     real(8), dimension(:),       intent(in)     :: k
-    real(8),                    intent(out)     :: energy
+    real(8),                     intent(out)    :: energy
+    real(4), dimension(3),       intent(out)    :: angle_pr
 
     integer :: ind, aa, bb, cc
     real(8), dimension(3) :: ra, rc, ea, ec, fa, fc
     real(8) :: d, ff, xsinph, norm_a, norm_c
     real(8) :: xrasin, xrcsin
     real(8) :: cosphi, cosphi2, sinphi, theta
 
     energy = 0.0d00
+    angle_pr = 0.0d00
     f = 0.0d00
 
     do ind = 1, size(a)
       aa = a(ind) + 1
       bb = b(ind) + 1
       cc = c(ind) + 1
 
@@ -79,10 +83,11 @@
         fc = (ea - cosphi * ec) * xrcsin
 
         f(aa, :) = f(aa, :) - fa
         f(cc, :) = f(cc, :) - fc
         f(bb, :) = f(bb, :) + fa + fc
 
         energy = energy + 0.5d0 * ff * d
+        angle_pr = angle_pr - (fa * ra) - (fc * rc)
       end if
     end do
 end subroutine
```

### Comparing `hymd-1.0.9/hymd/compute_bond_forces.f90` & `hymd-2.0.1/hymd/compute_bond_forces.f90`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-subroutine cbf(f, r, box, a, b, r0, k, energy)
+subroutine cbf(f, r, box, a, b, r0, k, energy, bond_pr)
     ! Compute two-particle bond forces and energy
     !
     ! Parameters
     ! ---------
     ! f : (N,D) numpy.ndarray
     !     Forces for N particles in D dimensions. Changed in place.
     ! r : (N,D) numpy.ndarray
@@ -29,14 +29,15 @@
     real(4), dimension(:,:), intent(in)     :: r
     real(8), dimension(:),   intent(in)     :: box
     integer, dimension(:),   intent(in)     :: a
     integer, dimension(:),   intent(in)     :: b
     real(8), dimension(:),   intent(in)     :: r0
     real(8), dimension(:),   intent(in)     :: k
     real(8),                 intent(out)    :: energy
+    real(4), dimension(3),   intent(out)    :: bond_pr
 
     integer :: ind, aa, bb
     real(8), dimension(3) :: rab, fa
     real(8) :: df, rab_norm
 
     energy = 0.0d00
     f = 0.0d00
@@ -52,9 +53,10 @@
       df = k(ind) * (rab_norm - r0(ind))
       fa = -df * rab / rab_norm
 
       f(aa, :) = f(aa, :) - fa
       f(bb, :) = f(bb, :) + fa
 
       energy = energy + 0.5d00 * k(ind) * (rab_norm - r0(ind))**2
+      bond_pr = bond_pr + fa * rab
     end do
-end subroutine
+end subroutine
```

### Comparing `hymd-1.0.9/hymd/compute_bond_forces__double.f90` & `hymd-2.0.1/hymd/compute_bond_forces__double.f90`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-subroutine cbf_d(f, r, box, a, b, r0, k, energy)
+subroutine cbf_d(f, r, box, a, b, r0, k, energy, bond_pr)
     ! Compute two-particle bond forces and energy
     !
     ! Parameters
     ! ---------
     ! f : (N,D) numpy.ndarray
     !     Forces for N particles in D dimensions. Changed in place.
     ! r : (N,D) numpy.ndarray
@@ -29,14 +29,15 @@
     real(8), dimension(:,:), intent(in)     :: r
     real(8), dimension(:),   intent(in)     :: box
     integer, dimension(:),   intent(in)     :: a
     integer, dimension(:),   intent(in)     :: b
     real(8), dimension(:),   intent(in)     :: r0
     real(8), dimension(:),   intent(in)     :: k
     real(8),                 intent(out)    :: energy
+    real(8), dimension(3),   intent(out)    :: bond_pr
 
     integer :: ind, aa, bb
     real(8), dimension(3) :: rab, fa
     real(8) :: df, rab_norm
 
     energy = 0.0d00
     f = 0.0d00
@@ -52,9 +53,10 @@
       df = k(ind) * (rab_norm - r0(ind))
       fa = -df * rab / rab_norm
 
       f(aa, :) = f(aa, :) - fa
       f(bb, :) = f(bb, :) + fa
 
       energy = energy + 0.5d00 * k(ind) * (rab_norm - r0(ind))**2
+      bond_pr = bond_pr + fa * rab
     end do
-end subroutine
+end subroutine
```

### Comparing `hymd-1.0.9/hymd/compute_dihedral_forces.f90` & `hymd-2.0.1/hymd/compute_dihedral_forces.f90`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 subroutine cdf(force, r, dipoles, transfer_matrix, box, a, b, c, d, coeff, dtype, bb_index, dipole_flag, energy)
   use dipole_reconstruction
   implicit none
 
-  real(4), intent(in out) :: force(:,:)
+  real(4), intent(inout) :: force(:,:)
   real(4), intent(in) :: r(:,:)
-  real(4), intent(in out) :: dipoles(:,:,:)
-  real(4), intent(in out) :: transfer_matrix(:,:,:,:)
+  real(4), intent(inout) :: dipoles(:,:,:)
+  real(4), intent(inout) :: transfer_matrix(:,:,:,:)
   real(8), intent(in) :: box(:)
   integer, intent(in) :: a(:), b(:), c(:), d(:), dtype(:), bb_index(:), dipole_flag
   real(4), intent(in) :: coeff(:,:,:)
   real(8), intent(out) :: energy
    
   integer :: ind, aa, bb, cc, dd, i
   integer, dimension(2) :: c_shape
```

### Comparing `hymd-1.0.9/hymd/compute_dihedral_forces__double.f90` & `hymd-2.0.1/hymd/compute_dihedral_forces__double.f90`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 subroutine cdf_d(force, r, dipoles, transfer_matrix, box, a, b, c, d, coeff, dtype, bb_index, dipole_flag, energy)
   use dipole_reconstruction_d
   implicit none
 
-  real(8), intent(in out) :: force(:,:)
+  real(8), intent(inout) :: force(:,:)
   real(8), intent(in) :: r(:,:)
-  real(8), intent(in out) :: dipoles(:,:,:)
-  real(8), intent(in out) :: transfer_matrix(:,:,:,:)
+  real(8), intent(inout) :: dipoles(:,:,:)
+  real(8), intent(inout) :: transfer_matrix(:,:,:,:)
   real(8), intent(in) :: box(:)
   integer, intent(in) :: a(:), b(:), c(:), d(:), dtype(:), bb_index(:), dipole_flag
   real(4), intent(in) :: coeff(:,:,:)
   real(8), intent(out) :: energy
 
   integer :: ind, aa, bb, cc, dd, i
   integer, dimension(2) :: c_shape
```

### Comparing `hymd-1.0.9/hymd/configure_runtime.py` & `hymd-2.0.1/hymd/configure_runtime.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import sys
 import numpy as np
 import atexit
 import cProfile
 import logging
 import pstats
+import tomli
 from .logger import Logger, print_header
 from .input_parser import read_config_toml, parse_config_toml
 
 
 def configure_runtime(args_in, comm):
     """Parse command line arguments and configuration file
 
@@ -28,91 +29,121 @@
         Namespace containing command line arguments.
     config : hymd.input_parser.Config
         Parsed configuration object.
     """
     ap = ArgumentParser()
 
     ap.add_argument(
-        "-v", "--verbose", default=1, type=int, nargs="?",
+        "-v",
+        "--verbose",
+        default=1,
+        type=int,
+        nargs="?",
         help="Increase logging verbosity",
     )
     ap.add_argument(
-        "--profile", default=False, action="store_true",
+        "--profile",
+        default=False,
+        action="store_true",
         help="Profile program execution with cProfile",
     )
     ap.add_argument(
-        "--disable-field", default=False, action="store_true",
+        "--disable-field",
+        default=False,
+        action="store_true",
         help="Disable field forces",
     )
     ap.add_argument(
-        "--disable-bonds", default=False, action="store_true",
+        "--disable-bonds",
+        default=False,
+        action="store_true",
         help="Disable two-particle bond forces",
     )
     ap.add_argument(
-        "--disable-angle-bonds", default=False, action="store_true",
+        "--disable-angle-bonds",
+        default=False,
+        action="store_true",
         help="Disable three-particle angle bond forces",
     )
     ap.add_argument(
-        "--disable-dihedrals", default=False, action="store_true",
+        "--disable-dihedrals",
+        default=False,
+        action="store_true",
         help="Disable four-particle dihedral forces",
     )
     ap.add_argument(
-        "--disable-dipole", default=False, action="store_true",
+        "--disable-dipole",
+        default=False,
+        action="store_true",
         help="Disable BB dipole calculation",
     )
     ap.add_argument(
-        "--double-precision", default=False, action="store_true",
+        "--double-precision",
+        default=False,
+        action="store_true",
         help="Use double precision positions/velocities",
     )
     ap.add_argument(
-        "--double-output", default=False, action="store_true",
+        "--double-output",
+        default=False,
+        action="store_true",
         help="Use double precision in output h5md",
     )
     ap.add_argument(
-        "--dump-per-particle", default=False, action="store_true",
+        "--dump-per-particle",
+        default=False,
+        action="store_true",
         help="Log energy values per particle, not total",
     )
     ap.add_argument(
-        "--force-output", default=False, action="store_true",
+        "--force-output",
+        default=False,
+        action="store_true",
         help="Dump forces to h5md output",
     )
     ap.add_argument(
-        "--velocity-output", default=False, action="store_true",
+        "--velocity-output",
+        default=False,
+        action="store_true",
         help="Dump velocities to h5md output",
     )
     ap.add_argument(
-        "--disable-mpio", default=False, action="store_true",
-        help=(
-            "Avoid using h5py-mpi, potentially decreasing IO " "performance"
-        ),
+        "--disable-mpio",
+        default=False,
+        action="store_true",
+        help=("Avoid using h5py-mpi, potentially decreasing IO " "performance"),
     )
     ap.add_argument(
         "--destdir", default=".", help="Write output to specified directory"
     )
     ap.add_argument(
-        "--seed", default=None, type=int,
+        "--seed",
+        default=None,
+        type=int,
         help="Set the numpy random generator seed for every rank",
     )
     ap.add_argument(
-        "--logfile", default="sim.log",
+        "--logfile",
+        default="sim.log",
         help="Redirect event logging to specified file",
     )
     ap.add_argument(
-        "config", help="Config .py or .toml input configuration script"
+        "-p", "--topol", default=None, help="Gmx-like topology file in toml format"
     )
+    ap.add_argument("config", help="Config .py or .toml input configuration script")
     ap.add_argument("input", help="input.hdf5")
     args = ap.parse_args(args_in)
 
     if comm.Get_rank() == 0:
         os.makedirs(args.destdir, exist_ok=True)
     comm.barrier()
 
     # Safely define seeds
     seeds = None
-    if comm.Get_rank() == 0:    
+    if comm.Get_rank() == 0:
         if args.seed is not None:
             ss = np.random.SeedSequence(args.seed)
         else:
             ss = np.random.SeedSequence()
         seeds = ss.spawn(comm.Get_size())
 
     seeds = comm.bcast(seeds, root=0)
@@ -150,24 +181,38 @@
         atexit.register(profile_atexit)
 
         pr.enable()
 
     try:
         Logger.rank0.log(
             logging.INFO,
-            f"Attempting to parse config file {args.config} as "".toml",
+            f"Attempting to parse config file {args.config} as " ".toml",
         )
+
+        if args.topol is not None:
+            topol = tomli.loads(read_config_toml(args.topol))
+            # Check if we have single "itp" files and add their keys to topol
+            if os.path.dirname(args.topol) == "":
+                args.topol = "./" + args.topol
+            if "include" in topol["system"]:
+                for file in topol["system"]["include"]:
+                    path = f"{os.path.dirname(args.topol)}/{file}"
+                    itps = tomli.loads(read_config_toml(path))
+                    for mol, itp in itps.items():
+                        topol[mol] = itp
+        else:
+            topol = None
         toml_config = read_config_toml(args.config)
         config = parse_config_toml(
             toml_config, file_path=os.path.abspath(args.config), comm=comm
         )
         Logger.rank0.log(
             logging.INFO, f"Successfully parsed {args.config} as .toml file"
         )
         config.command_line_full = " ".join(sys.argv)
         Logger.rank0.log(logging.INFO, str(config))
     except ValueError as ve:
         raise ValueError(
             f"Unable to parse configuration file {args.config}"
             f"\n\ntoml parse traceback:" + repr(ve)
         )
-    return args, config, prng
+    return args, config, prng, topol
```

### Comparing `hymd-1.0.9/hymd/dipole_reconstruction.f90` & `hymd-2.0.1/hymd/dipole_reconstruction.f90`

 * *Files identical despite different names*

### Comparing `hymd-1.0.9/hymd/dipole_reconstruction__double.f90` & `hymd-2.0.1/hymd/dipole_reconstruction__double.f90`

 * *Files identical despite different names*

### Comparing `hymd-1.0.9/hymd/field.py` & `hymd-2.0.1/hymd/field.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,156 @@
 """Forces and energies from the discretized particle-field grid interactions
 """
 import logging
 import numpy as np
 from mpi4py import MPI
 from .logger import Logger
+import warnings
+
+
+def initialize_pm(pmesh, config, comm=MPI.COMM_WORLD):
+    """
+    Creates the necessary pmesh objects for pfft operations.
+
+    Parameters
+    ----------
+    pmesh : module 'pmesh.pm'
+    config : Config
+        Configuration dataclass containing simulation metadata and parameters.
+    comm : MPI.Intracomm, optional
+        MPI communicator to use for rank commuication. Defaults to
+        MPI.COMM_WORLD.
+
+    Returns
+    -------
+    pm : object 'pmesh.pm.ParticleMesh'
+    field_list : list[pmesh.pm.RealField], (multiple)
+        Essential list of pmesh objects required for MD
+    list_coulomb : list[pmesh.pm.RealField], (multiple)
+        Additional list of pmesh objects required for electrostatics.
+    """
+
+    if config.dtype == np.float64:
+        pmeshtype = "f8"
+    else:
+        pmeshtype = "f4"
+    # Ignore numpy numpy.VisibleDeprecationWarning: Creating an ndarray from
+    # ragged nested sequences until it is fixed in pmesh
+    with warnings.catch_warnings():
+        warnings.filterwarnings(
+            action="ignore",
+            category=np.VisibleDeprecationWarning,
+            message=r"Creating an ndarray from ragged nested sequences",
+        )
+        # The first argument of ParticleMesh has to be a tuple
+        pm = pmesh.ParticleMesh(
+            config.mesh_size, BoxSize=config.box_size, dtype=pmeshtype, comm=comm
+        )
+    phi = [pm.create("real", value=0.0) for _ in range(config.n_types)]
+    phi_fourier = [
+        pm.create("complex", value=0.0) for _ in range(config.n_types)
+    ]  # noqa: E501
+    force_on_grid = [
+        [pm.create("real", value=0.0) for d in range(3)] for _ in range(config.n_types)
+    ]
+    v_ext_fourier = [pm.create("complex", value=0.0) for _ in range(4)]
+    v_ext = [pm.create("real", value=0.0) for _ in range(config.n_types)]
+
+    phi_transfer = [pm.create("complex", value=0.0) for _ in range(3)]
+
+    phi_laplacian = [
+        [pm.create("real", value=0.0) for d in range(3)] for _ in range(config.n_types)
+    ]
+
+    # Initialize charge density fields
+    coulomb_list = []
+    elec_common_list = [None, None, None, None]
+    _SPACE_DIM = config.box_size.size
+
+    if config.coulombtype == "PIC_Spectral_GPE" or config.coulombtype == "PIC_Spectral":
+        phi_q = pm.create("real", value=0.0)
+        phi_q_fourier = pm.create("complex", value=0.0)
+        psi = pm.create("real", value=0.0)
+        elec_field = [pm.create("real", value=0.0) for _ in range(_SPACE_DIM)]
+
+        elec_common_list = [phi_q, phi_q_fourier, psi, elec_field]
+
+    if config.coulombtype == "PIC_Spectral":
+        elec_field_fourier = [
+            pm.create("complex", value=0.0) for _ in range(_SPACE_DIM)
+        ]  # for force calculation
+        psi_fourier = pm.create("complex", value=0.0)
+
+        coulomb_list = [
+            elec_field_fourier,
+            psi_fourier,
+        ]
+
+    if (
+        config.coulombtype == "PIC_Spectral_GPE"
+    ):  ## initializing the density mesh #dielectric_flag
+        phi_eps = pm.create(
+            "real", value=0.0
+        )  ## real contrib of the epsilon dielectric painted to grid
+        phi_eps_fourier = pm.create("complex", value=0.0)  # complex contrib of phi eps
+        phi_eta = [
+            pm.create("real", value=0.0) for _ in range(_SPACE_DIM)
+        ]  ## real contrib of factor in polarization charge density
+        phi_eta_fourier = [
+            pm.create("complex", value=0.0) for _ in range(_SPACE_DIM)
+        ]  ## fourier of factor in polarization charge density
+        phi_pol = pm.create(
+            "real", value=0.0
+        )  ## real contrib of the polarization charge
+        phi_pol_prev = pm.create("real", value=0.0)
+        elec_dot = pm.create("real", value=0.0)
+        elec_field_contrib = pm.create(
+            "real", value=0.0
+        )  # needed for pol energies later
+
+        # External potential and force meshes
+        Vbar_elec = [pm.create("real", value=0.0) for _ in range(config.n_types)]
+        Vbar_elec_fourier = [
+            pm.create("complex", value=0.0) for _ in range(config.n_types)
+        ]
+        force_mesh_elec = [
+            [pm.create("real", value=0.0) for d in range(3)]
+            for _ in range(config.n_types)
+        ]
+        force_mesh_elec_fourier = [
+            [pm.create("complex", value=0.0) for d in range(3)]
+            for _ in range(config.n_types)
+        ]
+
+        coulomb_list = [
+            phi_eps,
+            phi_eps_fourier,
+            phi_eta,
+            phi_eta_fourier,
+            phi_pol,
+            phi_pol_prev,
+            elec_dot,
+            elec_field_contrib,
+            Vbar_elec,
+            Vbar_elec_fourier,
+            force_mesh_elec,
+            force_mesh_elec_fourier,
+        ]
+
+    field_list = [
+        phi,
+        phi_fourier,
+        force_on_grid,
+        v_ext_fourier,
+        v_ext,
+        phi_transfer,
+        phi_laplacian,
+    ]
+
+    return (pm, field_list, elec_common_list, coulomb_list)
 
 
 def compute_field_force(layouts, r, force_mesh, force, types, n_types):
     """Interpolate particle-field forces from the grid onto particle positions
 
     Backmaps the forces calculated on the grid to particle positions using the
     window function :math:`P` (by default cloud-in-cell [CIC]). In the
@@ -34,15 +177,15 @@
     r : (N,D) numpy.ndarray
         Array of positions for :code:`N` particles in :code:`D` dimensions.
         Local for each MPI rank.
     force_mesh : list[pmesh.pm.RealField]
         Pmesh :code:`RealField` objects containing discretized particle-field
         force density values on the computational grid; :code:`D` fields in D
         dimensions for each particle type. Local for each MPI rank--the full
-        computaional grid is represented by the collective fields of all MPI
+        computational grid is represented by the collective fields of all MPI
         ranks.
     force : (N,D) numpy.ndarray
         Array of forces for :code:`N` particles in :code:`D` dimensions. Local
         for each MPI rank.
     types : (N,) numpy.ndarray
         Array of type indices for each of :code:`N` particles. Local for each
         MPI rank.
@@ -83,101 +226,36 @@
     Returns
     -------
     field_q_self_energy : float
         Electrostatic self energy.
     """
     elec_conversion_factor = config.coulomb_constant / config.dielectric_const
 
-    prefac = elec_conversion_factor * np.sqrt(1./(2.*np.pi*config.sigma*config.sigma))
+    prefac = elec_conversion_factor * np.sqrt(
+        1.0 / (2.0 * np.pi * config.sigma * config.sigma)
+    )
     _squared_charges = charges * charges
     squared_charges_sum = comm.allreduce(np.sum(_squared_charges))
     return prefac * squared_charges_sum
 
 
-def compute_field_energy_q(
-    config, phi_q, phi_q_fourier, elec_potential, elec_potential_fourier, 
-    field_q_self_energy, comm=MPI.COMM_WORLD,
-):
-    """Calculate the electrostatic energy from a field configuration
-
-    From the definition of the elecrostatic potential :math:`\\Psi`, the energy
-    is
-
-    .. math::
-
-        E = \\frac{1}{2\\varepsilon_0 \\varepsilon_r}\\int\\mathrm{d}\\mathbf{r}\\,
-            \\rho(\\mathbf{r}) \\Psi(\\mathbf{r}),
-
-    where :math:`\\rho(\\mathbf{r})` denotes the charge density at position
-    :math:`\\mathbf{r}`, :math:`\\varepsilon_0` is the vacuum permittivity 
-    and :math:`\\varepsilon_r` is the relative dielectric of the simulation
-    medium.
-
-    Parameters
-    ----------
-    config : Config
-        Configuration object.
-    phi_q : pmesh.pm.RealField
-        Pmesh :code:`RealField` object containing the discretized
-        electrostatic potential values in real space on the
-        computational grid. Local for each MPI rank--the full computayional grid
-        is represented by the collective fields of all MPI ranks.
-    phi_q_fourier : pmesh.pm.ComplexField
-        Pmesh :code:`ComplexField` object containing the discretized
-        electrostatic potential values in reciprocal space on the
-        computational grid. Local for each MPI rank--the full computayional grid
-        is represented by the collective fields of all MPI ranks.
-    elec_potential : pmesh.pm.RealField
-        Pmesh :code:`RealField` object for storing calculated discretized
-        electrostatic potential values in real space on the
-        computational grid. Pre-allocated, but empty; any values in this field
-        are discarded. Changed in-place. Local for each MPI rank--the full
-        computaional grid is represented by the collective fields of all MPI
-        ranks.
-    elec_potential_fourier : pmesh.pm.ComplexField
-        Pmesh :code:`ComplexField` object for storing calculated discretized
-        electrostatic potential values in reciprocal space on the
-        computational grid. Pre-allocated, but empty; any values in this field
-        are discarded. Changed in-place. Local for each MPI rank--the full
-        computaional grid is represented by the collective fields of all MPI
-        ranks.
-    field_q_self_energy : float
-        Electrostatic self energy to be subtracted.
-
-    Returns
-    -------
-    field_q_energy : float
-        Total electrostatic energy.
-    """
-    elec_conversion_factor = config.coulomb_constant / config.dielectric_const
-    V = np.prod(config.box_size)
-    n_mesh_cells = np.prod(np.full(3, config.mesh_size))
-    volume_per_cell = V / n_mesh_cells
-
-    # solve Poisson equation in Fourier space
-    def poisson_transfer_function(k, v):
-        return (
-            4. * np.pi * elec_conversion_factor * v
-            / k.normp(p=2, zeromode=1)
-        )
-    phi_q_fourier.apply(
-        poisson_transfer_function, out=elec_potential_fourier
-    )
-
-    # get electrostatic potential in real space and compute energy
-    elec_potential_fourier.c2r(out=elec_potential)
-    field_q_energy = 0.5 * volume_per_cell * comm.allreduce(np.sum(phi_q*elec_potential))
-
-    field_q_energy -= field_q_self_energy # subtract self-energy
-    return field_q_energy
-
-
 def update_field_force_q(
-    charges, phi_q, phi_q_fourier, elec_field_fourier, elec_field,
-    elec_forces, layout_q, hamiltonian, pm, positions, config,
+    charges,
+    phi_q,
+    phi_q_fourier,
+    psi,
+    psi_fourier,
+    elec_field_fourier,
+    elec_field,
+    elec_forces,
+    layout_q,
+    hamiltonian,
+    pm,
+    positions,
+    config,
 ):
     """Calculate the electrostatic particle-field forces on the grid
 
     Computes the electrostatic potential :math:`\\Psi` from particle charges
     through the smoothed charge density :math:`\\tilde\\rho`. With :math:`P`
     being the cloud-in-cell (CIC) window function, the charge density and
     filtered charge densities are computed as
@@ -230,34 +308,34 @@
     charges : (N,) numpy.ndarray
         Array of particle charge values for :code:`N` particles. Local for each
         MPI rank.
     phi_q : pmesh.pm.RealField
         Pmesh :code:`RealField` object for storing calculated discretized
         charge density density values on the computational grid. Pre-allocated,
         but empty; any values in this field are discarded. Changed in-place.
-        Local for each MPI rank--the full computaional grid is represented by
+        Local for each MPI rank--the full computational grid is represented by
         the collective fields of all MPI ranks.
     phi_q_fourier : pmesh.pm.ComplexField
         Pmesh :code:`ComplexField` object for storing calculated discretized
         Fourier transformed charge density values in reciprocal space on the
         computational grid. Pre-allocated, but empty; any values in this field
         are discarded. Changed in-place. Local for each MPI rank--the full
-        computaional grid is represented by the collective fields of all MPI
+        computational grid is represented by the collective fields of all MPI
         ranks.
     elec_field_fourier : pmesh.pm.ComplexField
         Pmesh :code:`ComplexField` object for storing calculated discretized
         electric field values in reciprocal space on the computational grid.
         Pre-allocated, but empty; any values in this field are discarded.
-        Changed in-place. Local for each MPI rank--the full computaional grid
+        Changed in-place. Local for each MPI rank--the full computational grid
         is represented by the collective fields of all MPI ranks.
     elec_field : pmesh.pm.RealField
         Pmesh :code:`RealField` object for storing calculated discretized
         electric field values on the computational grid. Pre-allocated,
         but empty; any values in this field are discarded. Changed in-place.
-        Local for each MPI rank--the full computaional grid is represented by
+        Local for each MPI rank--the full computational grid is represented by
         the collective fields of all MPI ranks.
     elec_forces : (N,D) numpy.ndarray
         Array of electrostatic forces on :code:`N` particles in :code:`D`
         dimensions.
     layout_q : pmesh.domain.Layout
         Pmesh communication layout object for domain decomposition of the full
         system. Used as blueprint by :code:`pmesh.pm.paint` and
@@ -274,173 +352,99 @@
         Local for each MPI rank.
     config : hymd.input_parser.Config
         Configuration object.
     """
     V = np.prod(config.box_size)
     n_mesh_cells = np.prod(np.full(3, config.mesh_size))
     volume_per_cell = V / n_mesh_cells
-    
+    n_dimensions = config.box_size.size
+    elec_conversion_factor = config.coulomb_constant / config.dielectric_const
+
     # charges to grid
     pm.paint(positions, layout=layout_q, mass=charges, out=phi_q)
     phi_q /= volume_per_cell
+    # print("phi_q", np.sum(phi_q))
     phi_q.r2c(out=phi_q_fourier)
 
     # smear charges with filter
     phi_q_fourier.apply(hamiltonian.H, out=phi_q_fourier)
-    phi_q_fourier.c2r(out=phi_q)
+
+    # solve Poisson equation in Fourier space to get electrostatic potential
+    def poisson_transfer_function(k, v):
+        return 4.0 * np.pi * elec_conversion_factor * v / k.normp(p=2, zeromode=1)
+
+    phi_q_fourier.apply(poisson_transfer_function, out=psi_fourier)
+    # print("psi_fourier", np.sum(psi_fourier))
+    psi_fourier.c2r(out=psi)
+    # print("phi_q * psi update_field", np.sum(phi_q * psi))
+
+    # exit()
 
     # compute electric field directly from smeared charged densities in Fourier
-    n_dimensions = config.box_size.size
-    elec_conversion_factor = config.coulomb_constant / config.dielectric_const
     for _d in np.arange(n_dimensions):
 
         def poisson_transfer_function(k, v, d=_d):
             return (
-                -1j * k[d] * 4.0 * np.pi * elec_conversion_factor * v
+                -1j
+                * k[d]
+                * 4.0
+                * np.pi
+                * elec_conversion_factor
+                * v
                 / k.normp(p=2, zeromode=1)
             )
-        phi_q_fourier.apply(
-            poisson_transfer_function, out=elec_field_fourier[_d]
-        )
+
+        phi_q_fourier.apply(poisson_transfer_function, out=elec_field_fourier[_d])
         elec_field_fourier[_d].c2r(out=elec_field[_d])
 
     # get electrostatic force from electric field
     for _d in np.arange(n_dimensions):
         elec_forces[:, _d] = charges * (
             elec_field[_d].readout(positions, layout=layout_q)
         )
 
 
-def update_field_force_energy_q(
-    charges, phi_q, phi_q_fourier, elec_field_fourier, elec_field, elec_forces,
-    elec_energy_field, field_q_energy, layout_q, pm, positions, config,
-    compute_energy=False, comm=MPI.COMM_WORLD,
+def comp_laplacian(
+    phi_fourier,
+    phi_transfer,
+    phi_laplacian,
+    hamiltonian,
+    config,
 ):
-    """Calculate the electrostatic particle-field energy and forces on the grid
-
-    .. deprecated:: 1.0.0
-        :code:`update_field_force_energy_q` was deprecated in favour of
-        :code:`update_field_force_q` and independent calls to
-        :code:`compute_field_energy_q` prior to 1.0.0 release.
-
-    Parameters
-    ----------
-    charges : (N,) numpy.ndarray
-        Array of particle charge values for :code:`N` particles. Local for each
-        MPI rank.
-    phi_q : pmesh.pm.RealField
-        Pmesh :code:`RealField` object for storing calculated discretized
-        charge density density values on the computational grid. Pre-allocated,
-        but empty; any values in this field are discarded. Changed in-place.
-        Local for each MPI rank--the full computaional grid is represented by
-        the collective fields of all MPI ranks.
-    phi_q_fourier : pmesh.pm.ComplexField
-        Pmesh :code:`ComplexField` object for storing calculated discretized
-        Fourier transformed charge density values in reciprocal space on the
-        computational grid. Pre-allocated, but empty; any values in this field
-        are discarded. Changed in-place. Local for each MPI rank--the full
-        computaional grid is represented by the collective fields of all MPI
-        ranks.
-    elec_field_fourier : pmesh.pm.ComplexField
-        Pmesh :code:`ComplexField` object for storing calculated discretized
-        electric field values in reciprocal space on the computational grid.
-        Pre-allocated, but empty; any values in this field are discarded.
-        Changed in-place. Local for each MPI rank--the full computaional grid
-        is represented by the collective fields of all MPI ranks.
-    elec_field : pmesh.pm.RealField
-        Pmesh :code:`RealField` object for storing calculated discretized
-        electric field values on the computational grid. Pre-allocated,
-        but empty; any values in this field are discarded. Changed in-place.
-        Local for each MPI rank--the full computaional grid is represented by
-        the collective fields of all MPI ranks.
-    elec_forces : (N,D) numpy.ndarray
-        Array of electrostatic forces on :code:`N` particles in :code:`D`
-        dimensions.
-    elec_energy_field : pmesh.pm.ComplexField
-        Pmesh :code:`ComplexField` object for storing calculated discretized
-        electrostatic energy density values in reciprocal space on the
-        computational grid. Pre-allocated, but empty; any values in this field
-        are discarded. Changed in-place. Local for each MPI rank--the full
-        computaional grid is represented by the collective fields of all MPI
-        ranks.
-    field_q_energy : float
-        Total elecrostatic energy.
-    layout_q : pmesh.domain.Layout
-        Pmesh communication layout object for domain decomposition of the full
-        system. Used as blueprint by :code:`pmesh.pm.paint` and
-        :code:`pmesh.pm.readout` for exchange of particle information across
-        MPI ranks as necessary.
-    pm : pmesh.pm.ParticleMesh
-        Pmesh :code:`ParticleMesh` object interfacing to the CIC window
-        function and the PFFT discrete Fourier transform library.
-    positions : (N,D) numpy.ndarray
-        Array of positions for :code:`N` particles in :code:`D` dimensions.
-        Local for each MPI rank.
-    config : Config
-        Configuration object.
-    compute_energy : bool, optional
-        Computes the electrostatic energy if :code:`True`, otherwise only
-        computes the electrostatic forces.
-    comm : mpi4py.Comm
-        MPI communicator to use for rank commuication.
-
-    Returns
-    -------
-    elec_field_energy : float
-        Total electrostatic energy.
-    """
-    V = np.prod(config.box_size)
-    n_mesh_cells = np.prod(np.full(3, config.mesh_size))
-    volume_per_cell = V / n_mesh_cells
-    pm.paint(positions, layout=layout_q, mass=charges, out=phi_q)
-    phi_q /= volume_per_cell
-    phi_q.r2c(out=phi_q_fourier)
-
-    def phi_transfer_function(k, v):
-        return v * np.exp(-0.5 * config.sigma ** 2 * k.normp(p=2, zeromode=1))
-
-    phi_q_fourier.apply(phi_transfer_function, out=phi_q_fourier)
-    phi_q_fourier.c2r(out=phi_q)
-    n_dimensions = config.box_size.size
-    elec_conversion_factor = config.coulomb_constant / config.dielectric_const
-
-    for _d in np.arange(n_dimensions):
-        def poisson_transfer_function(k, v, d=_d):
-            return (
-                -1j * k[d] * 4.0 * np.pi * elec_conversion_factor * v
-                / k.normp(p=2, zeromode=1)
-            )
+    for t in range(config.n_types):
+        np.copyto(phi_transfer[0].value, phi_fourier[t].value, casting="no", where=True)
+        np.copyto(phi_transfer[1].value, phi_fourier[t].value, casting="no", where=True)
+        np.copyto(phi_transfer[2].value, phi_fourier[t].value, casting="no", where=True)
 
-        phi_q_fourier.apply(
-            poisson_transfer_function, out=elec_field_fourier[_d]
-        )
-        elec_field_fourier[_d].c2r(out=elec_field[_d])
+        # Evaluate laplacian of phi in fourier space
+        for d in range(3):
 
-    for _d in np.arange(n_dimensions):
-        elec_forces[:, _d] = charges * (
-            elec_field[_d].readout(positions, layout=layout_q)
-        )
+            def laplacian_transfer(k, v, d=d):
+                return -k[d] ** 2 * v
 
-    if compute_energy:
-        def transfer_energy(k, v):
-            return (
-                4.0 * np.pi * elec_conversion_factor * np.abs(v)**2
-                / k.normp(p=2, zeromode=1)
-            )
-        phi_q_fourier.apply(
-            transfer_energy, kind="wavenumber", out=elec_energy_field
-        )
-        field_q_energy = 0.5 * comm.allreduce(np.sum(elec_energy_field.value))
-
-    return field_q_energy.real
+            phi_transfer[d].apply(laplacian_transfer, out=Ellipsis)
+            phi_transfer[d].c2r(out=phi_laplacian[t][d])
 
 
 def update_field(
-    phi, layouts, force_mesh, hamiltonian, pm, positions, types, config, v_ext,
-    phi_fourier, v_ext_fourier, compute_potential=False,
+    phi,
+    phi_laplacian,
+    phi_transfer,
+    layouts,
+    force_mesh,
+    hamiltonian,
+    pm,
+    positions,
+    types,
+    config,
+    v_ext,
+    phi_fourier,
+    v_ext_fourier,
+    m,
+    compute_potential=False,
 ):
     """Calculate the particle-field potential and force density
 
     If :code:`compute_potential` is :code:`True`, the energy may subsequently
     be computed by calling :code:`compute_field_and_kinetic_energy`.
 
     Computes the particle-field external potential :math:`V_\\text{ext}` from
@@ -488,26 +492,31 @@
 
     Parameters
     ----------
     phi : list[pmesh.pm.RealField]
         Pmesh :code:`RealField` objects containing discretized particle number
         density values on the computational grid; one for each particle type.
         Pre-allocated, but empty; any values in this field are discarded.
-        Changed in-place. Local for each MPI rank--the full computaional grid
+        Changed in-place. Local for each MPI rank--the full computational grid
         is represented by the collective fields of all MPI ranks.
+    phi_laplacian : list[pmesh.pm.RealField], (M, 3)
+        Like phi, but containing the laplacian of particle number densities.
+    phi_transfer : list[pmesh.pm.ComplexField], (3,)
+        Like phi_fourier, used as an intermediary to perform FFT operations
+        to obtain the gradient or laplacian of particle number densities.
     layouts : list[pmesh.domain.Layout]
         Pmesh communication layout objects for domain decompositions of each
         particle type. Used as blueprint by :code:`pmesh.pm.readout` for
         exchange of particle information across MPI ranks as necessary.
     force_mesh : list[pmesh.pm.RealField]
         Pmesh :code:`RealField` objects containing discretized particle-field
         force density values on the computational grid; :code:`D` fields in D
         dimensions for each particle type. Pre-allocated, but empty; any values
         in this field are discarded. Changed in-place. Local for each MPI
-        rank--the full computaional grid is represented by the collective
+        rank--the full computational grid is represented by the collective
         fields of all MPI ranks.
     hamiltonian : Hamiltonian
         Particle-field interaction energy handler object. Defines the
         grid-independent filtering function, :math:`H`.
     pm : pmesh.pm.ParticleMesh
         Pmesh :code:`ParticleMesh` object interfacing to the CIC window
         function and the PFFT discrete Fourier transform library.
@@ -520,34 +529,37 @@
     config : Config
         Configuration object.
     v_ext : list[pmesh.pm.RealField]
         Pmesh :code:`RealField` objects containing discretized particle-field
         external potential values on the computational grid; one for each
         particle type. Pre-allocated, but empty; any values in this field are
         discarded Changed in-place. Local for each MPI rank--the full
-        computaional grid is represented by the collective fields of all MPI
+        computational grid is represented by the collective fields of all MPI
         ranks.
     phi_fourier : list[pmesh.pm.ComplexField]
         Pmesh :code:`ComplexField` objects containing discretized particle
         number density values in reciprocal space on the computational grid;
         one for each particle type. Pre-allocated, but empty; any values in
         this field are discarded Changed in-place. Local for each MPI rank--the
-        full computaional grid is represented by the collective fields of all
+        full computational grid is represented by the collective fields of all
         MPI ranks.
     v_ext_fourier : list[pmesh.pm.ComplexField]
         Pmesh :code:`ComplesField` objects containing discretized
         particle-field external potential values in reciprocal space on the
         computational grid; :code:`D+1` fields in D dimensions for each
         particle type. :code:`D` copies are made after calculation for later
         use in force calculation, because the `force transfer function`
         application differentiates the field in-place, ruining the contents
         for differentiation in the remaining :code:`D-1` spatial directions.
         Pre-allocated, but empty; any values in this field are discarded.
-        Changed in-place. Local for each MPI rank--the full computaional grid
+        Changed in-place. Local for each MPI rank--the full computational grid
         is represented by the collective fields of all MPI ranks.
+    m: list[float], (M,)
+        pmesh.pm.ParticleMesh parameter for mass of particles in simulation unit.
+        Defaults to 1.0 for all particle types.
     compute_potential : bool, optional
         If :code:`True`, a :code:`D+1`-th copy of the Fourier transformed
         external potential field is made to be used later in particle-field
         energy calculation. If :code:`False`, only :code:`D` copies are made.
 
     See also
     --------
@@ -555,55 +567,73 @@
         Compute the particle-field energy after the external potential is
         calculated.
     """
     V = np.prod(config.box_size)
     n_mesh_cells = np.prod(np.full(3, config.mesh_size))
     volume_per_cell = V / n_mesh_cells
     for t in range(config.n_types):
-        pm.paint(positions[types == t], layout=layouts[t], out=phi[t])
+        pm.paint(positions[types == t], mass=m[t], layout=layouts[t], out=phi[t])
         phi[t] /= volume_per_cell
         phi[t].r2c(out=phi_fourier[t])
         phi_fourier[t].apply(hamiltonian.H, out=Ellipsis)
         phi_fourier[t].c2r(out=phi[t])
 
     # External potential
     for t in range(config.n_types):
-        hamiltonian.v_ext[t](phi).r2c(out=v_ext_fourier[0])
+        v = hamiltonian.v_ext[t](phi)
+
+        v.r2c(out=v_ext_fourier[0])
         v_ext_fourier[0].apply(hamiltonian.H, out=Ellipsis)
         np.copyto(
-            v_ext_fourier[1].value, v_ext_fourier[0].value, casting="no",
+            v_ext_fourier[1].value,
+            v_ext_fourier[0].value,
+            casting="no",
             where=True,
         )
         np.copyto(
-            v_ext_fourier[2].value, v_ext_fourier[0].value, casting="no",
+            v_ext_fourier[2].value,
+            v_ext_fourier[0].value,
+            casting="no",
             where=True,
         )
         if compute_potential:
             np.copyto(
-                v_ext_fourier[3].value, v_ext_fourier[0].value, casting="no",
+                v_ext_fourier[3].value,
+                v_ext_fourier[0].value,
+                casting="no",
                 where=True,
             )
 
         # Differentiate the external potential in fourier space
         for d in range(3):
+
             def force_transfer_function(k, v, d=d):
                 return -k[d] * 1j * v
 
             v_ext_fourier[d].apply(force_transfer_function, out=Ellipsis)
             v_ext_fourier[d].c2r(out=force_mesh[t][d])
 
         if compute_potential:
             v_ext_fourier[3].c2r(out=v_ext[t])
 
 
 def compute_field_and_kinetic_energy(
-    phi, velocity, hamiltonian, positions, types, v_ext, config, layouts,
+    phi,
+    phi_q,
+    psi,
+    velocity,
+    hamiltonian,
+    positions,
+    types,
+    v_ext,
+    config,
+    layouts,
     comm=MPI.COMM_WORLD,
 ):
-    """Compute the particle-field and kintic energy contributions
+    """Compute the particle-field and kinetic energy contributions
 
     Calculates the kinetic energy through
 
     .. math::
 
         E_k = \\sum_j \\frac{1}{2}m_j\\mathbf{v}_j\\cdot\\mathbf{v}_j,
 
@@ -617,15 +647,15 @@
     where :math:`w` is the interaction energy functional `density`.
 
     Parameters
     ----------
     phi : list[pmesh.pm.RealField]
         Pmesh :code:`RealField` objects containing discretized particle number
         density values on the computational grid; one for each particle type.
-        Local for each MPI rank--the full computaional grid is represented by
+        Local for each MPI rank--the full computational grid is represented by
         the collective fields of all MPI ranks.
     velocity : (N,D) numpy.ndarray
         Array of velocities for :code:`N` particles in :code:`D` dimensions.
         Local for each MPI rank.
     hamiltonian : Hamiltonian
         Particle-field interaction energy handler object. Defines the
         grid-independent filtering function, :math:`H`.
@@ -634,15 +664,15 @@
         Local for each MPI rank.
     types : (N,) numpy.ndarray
         Array of type indices for each of :code:`N` particles. Local for each
         MPI rank.
     v_ext : list[pmesh.pm.RealField]
         Pmesh :code:`RealField` objects containing discretized particle-field
         external potential values on the computational grid; one for each
-        particle type. Local for each MPI rank--the full computaional grid is
+        particle type. Local for each MPI rank--the full computational grid is
         represented by the collective fields of all MPI ranks.
     config : Config
         Configuration object.
     layouts : list[pmesh.domain.Layout]
         Pmesh communication layout objects for domain decompositions of each
         particle type. Used as blueprint by :code:`pmesh.pm.readout` for
         exchange of particle information across MPI ranks as necessary.
@@ -655,23 +685,439 @@
         Computes the up-to-date external potential for use in calculating the
         particle-field energy.
     """
     V = np.prod(config.box_size)
     n_mesh__cells = np.prod(np.full(3, config.mesh_size))
     volume_per_cell = V / n_mesh__cells
 
-    w = hamiltonian.w(phi) * volume_per_cell
-    field_energy = w.csum()
-    kinetic_energy = comm.allreduce(0.5 * config.mass * np.sum(velocity ** 2))
-    return field_energy, kinetic_energy
+    w_0 = hamiltonian.w_0(phi) * volume_per_cell
+    field_energy = w_0.csum()  # w to W
+
+    kinetic_energy = comm.allreduce(0.5 * config.mass * np.sum(velocity**2))
+
+    if config.coulombtype == "PIC_Spectral":
+        w_elec = hamiltonian.w_elec([phi_q, psi]) * volume_per_cell
+        field_q_energy = w_elec.csum()
+    else:
+        field_q_energy = 0.0
+
+    return field_energy, kinetic_energy, field_q_energy
+
+
+def compute_field_energy_q_GPE(
+    config,
+    phi_eps,
+    field_q_energy,
+    dot_elec,
+    comm=MPI.COMM_WORLD,
+):
+    """
+    Compute the electrostatic energy after electrosatic forces is
+    calculated.
+
+    From the definition of the elecrostatic potential :math:`\\Psi`, the energy
+    is
+
+        W = \\frac{1}{2}\\int\\mathrm{d}\\mathbf{r}\\,
+            \\epsilon(\\mathbf{r})} \\left(\\mathbf{E}\\cdot \\mathbf{E}\\right),
+
+    where :math:`\\epsilon(\\mathbf{r})}` is the anisotropic, spatially dependent,
+    relative dielectric of the simulation medium.
+
+    Parameters
+    ----------
+    config : hymd.input_parser.Config
+        Configuration object.
+    phi_eps : pmesh.pm.RealField
+        Pmesh :code:`RealField` object for storing calculated discretized
+        relative dielectric values on the computational grid.
+        Local for each MPI rank--the full computational grid is represented by
+        the collective fields of all MPI ranks.
+    field_q_energy : float
+        Total elecrostatic energy.
+    dot_elec : pmesh.pm.RealField
+        Pmesh :code:`RealField` object for storing :math:`|\\mathbf{E(r)}|^{2}`
+        on the computational grid. Local for each MPI rank -- the full computational
+        grid is represented by the collective fields of all MPI ranks.
+    comm : mpi4py.Comm
+        MPI communicator to use  for rank commuication.
+
+    See also
+    --------
+    update_field_force_q_GPE:
+        Compute the electrosatic force from an anisotropic dielectric general
+        Poisson equation.
+    """
+
+    V = np.prod(config.box_size)
+    n_mesh__cells = np.prod(np.full(3, config.mesh_size))
+    volume_per_cell = V / n_mesh__cells
+    # ^ due to integration on local cell before allreduce
+
+    eps_0 = 1.0 / (config.coulomb_constant * 4 * np.pi)
+    field_q_energy = (
+        volume_per_cell * (0.5 * eps_0) * comm.allreduce(np.sum(phi_eps * dot_elec))
+    )
+
+    return field_q_energy
+
+
+def update_field_force_q_GPE(
+    conv_fun,
+    phi,
+    types,
+    charges,
+    phi_q,
+    phi_q_fourier,
+    phi_eps,
+    phi_eps_fourier,
+    phi_eta,
+    phi_eta_fourier,
+    phi_pol_prev,
+    phi_pol,
+    elec_field,
+    elec_forces,
+    elec_field_contrib,
+    psi,
+    Vbar_elec,
+    Vbar_elec_fourier,
+    force_mesh_elec,
+    force_mesh_elec_fourier,
+    hamiltonian,
+    layout_q,
+    layouts,
+    pm,
+    positions,
+    config,
+    comm=MPI.COMM_WORLD,
+):
+    """
+    Calculate the electrostatic particle-field forces on the grid, arising from
+    a general Poisson equation, i.e. anisotropic permittivity/dielectric.
+    The function is called when tomli input config.coulombtype = "PIC_Spectral_GPE."
+
+    Computes the electrostatic potential :math:`\\Psi` from particle charges
+    through the smoothed charge density :math:`\\tilde\\rho`. With :math:`P`
+    being the cloud-in-cell (CIC) window function, the charge density and
+    filtered charge densities are computed as
+
+    .. math::
+
+        \\rho(\\mathbf{r}) = \\sum_i q_i P(\\mathbf{r}-\\mathbf{r}_i),
+
+    and
+
+    .. math::
+
+        \\tilde\\rho(\\mathbf{r}) = \\int\\mathrm{x}\\mathbf{r}\\,
+            \\rho(\\mathbf{x})H(\\mathbf{r}-\\mathbf{x}),
+
+    where :math:`H` is the grid-independent filtering function. The
+    electrostatic potential for a variable dielectric does not have an
+    analytical expression, and is computed in reciprocal through an iterative
+    method.
+
+    The GPE states that
+
+    .. math::
+
+            \\nabla \\cdot \\left(\\epsilon(\\mathbf{r})
+            \\nabla{\\mathbf{\\psi(r)}}\\right) = -\\rho({\\mathbf{r}}).
+
+    where :math:`\\epsilon(\\mathbf{r})` is the relative dielectric function.
+
+    Parameters
+    ----------
+    conv_fun : Convergence function.
+        Returns a scalar. Depends on MPI allreduce for similar convergence
+        across MPI ranks.
+    phi : list[pmesh.pm.RealField]
+        Pmesh :code:`RealField` objects containing discretized particle number
+        density values on the computational grid; one for each particle type.
+        Local for each MPI rank--the full computational grid is represented by
+        the collective fields of all MPI ranks.
+    types : (N,) numpy.ndarray
+        Array of type indices for each of :code:`N` particles. Local for each
+        MPI rank.
+    charges : (N,) numpy.ndarray
+        Array of particle charge values for :code:`N` particles. Local for each
+        MPI rank.
+    phi_q : pmesh.pm.RealField
+        Pmesh :code:`RealField` object for storing calculated discretized
+        charge density density values on the computational grid. Pre-allocated,
+        but empty. Changed in-place.
+        Local for each MPI rank--the full computational grid is represented by
+        the collective fields of all MPI ranks.
+    phi_q_fourier : pmesh.pm.ComplexField
+        Pmesh :code:`ComplexField` object for storing calculated discretized
+        Fourier transformed charge density values in reciprocal space on the
+        computational grid. Pre-allocated, but empty. Changed in-place.
+        Local for each MPI rank--the full computational grid is represented by
+        the collective fields of all MPI ranks.
+    phi_eps : pmesh.pm.RealField
+        Pmesh :code:`RealField` object for storing calculated discretized
+        relative dielectric values on the computational grid. Pre-allocated,
+        but empty. Changed in-place.
+        Local for each MPI rank--the full computational grid is represented by
+        the collective fields of all MPI ranks.
+    phi_eps_fourier : pmesh.pm.ComplexField
+        Pmesh :code:`ComplexField` object for storing calculated discretized
+        Fourier transformed relative dielectric values in reciprocal space on the
+        computational grid. Pre-allocated, but empty. Changed in-place.
+        Local for each MPI rank--the full computational grid is represented
+        by the collective fields of all MPI ranks.
+    phi_eta : pmesh.pm.RealField
+        Pmesh :code:`RealField` object for storing calculated discretized
+        gradients of the relative dielectric values on the computational grid.
+        Pre-allocated,but empty. Changed in-place.Local for each MPI rank--the
+        full computational grid is represented by the collective fields of all MPI ranks.
+    phi_eta_fourier : pmesh.pm.ComplexField
+        Pmesh :code:`ComplexField` object for storing the calculated discretized
+        Fourier transformed gradient relative dielectric values in reciprocal space on the
+        computational grid. Pre-allocated, but empty.  Changed in-place.
+        Local for each MPI rank--the full computational grid is represented
+        by the collective fields of all MPI ranks.
+    phi_pol_prev : pmesh.pm.RealField
+        Pmesh :code:`RealField` object for storing calculated discretized
+        polarization charge values on the computational grid. Parameter in
+        the iterative method.Pre-allocated,but empty. Changedin-place.
+        Local for each MPI rank--the full computational grid is represented
+        by the collective fields of all MPI ranks.
+    phi_pol : pmesh.pm.RealField
+        Pmesh :code:`RealField` object for storing calculated discretized
+        polarization charges on the computational grid. Parameter in the iterative
+        method, updating the next quess in solving for the electrostatic potential.
+        Pre-allocated,but empty.  Changed in-place.Local for each MPI rank--
+        the full computational grid is represented by the collective fields of
+        all MPI ranks.
+    elec_field : pmesh.pm.RealField
+        Pmesh :code:`RealField` object for storing calculated discretized
+        electric field values on the computational grid. Pre-allocated,
+        but empty. Changed in-place. Local for each MPI rank--the full
+        computational grid is represented by the collective fields of all
+        MPI ranks.
+    elec_forces : (N,D) numpy.ndarray
+        Array of electrostatic forces on :code:`N` particles in :code:`D`
+        dimensions.
+    elec_field_contrib : pmesh.pm.RealField
+        Pmesh :code:`RealField` object for storing
+        :math:`|\\mathbf{E(r)}|^2/\\phi_{0}` on the computational grid.
+        Pre-allocated, but empty. Changed in-place.
+        Local for each MPI rank-- the full computational grid is represented by
+        the collective fields of all MPI ranks.
+    psi : pmesh.pm.RealField
+        Pmesh :code:`RealField` object for storing electrostatic potential
+        on the computational grid. Pre-allocated, but empty. Changed in-place.
+        Local for each MPI rank-- the full computational grid is represented by
+        the collective fields of all MPI ranks.
+    Vbar_elec : mesh.pm.RealField
+        Pmesh :code:`RealField` object for storing functional derivatives of
+        :math:`\\|w(\\{ \\phi \\})_{elec}`on the computational grid.
+        Pre-allocated, but empty. Changed in-place. Local for each MPI rank--
+        the full computational grid is represented by the collective fields of
+         all MPI ranks.
+    Vbar_elec_fourier : pmesh.pm.ComplexField
+        Pmesh :code:`ComplexField` object for storing the calculated functional
+        derivatives of :math:`\\|w(\\{ \\phi \\})_{elec}` in reciprocal space on the
+        computational grid. Pre-allocated, but empty.  Changed in-place.
+        Local for each MPI rank--the full computational grid is represented
+        by the collective fields of all MPI ranks.
+    force_mesh_elec : pmesh.pm.RealField
+        Pmesh :code:`RealField` object for storing electrostatic force values
+        on the computational grid. Pre-allocated, but empty. Changed in-place.
+        Local for each MPI rank-- the full computational grid is represented by
+        the collective fields of all MPI ranks.
+    force_mesh_elec_fourier : pmesh.pm.ComplexField
+        Pmesh :code:`ComplexField` object for storing the calculated electrostatic
+        force values in reciprocal space on the computational grid. Local for
+        each MPI rank--the full computational grid is represented by the collective
+        fields of all MPI ranks.
+    hamiltonian : Hamiltonian
+        Particle-field interaction energy handler object. Defines the
+        grid-independent filtering function, :math:`H`.
+    layout_q : pmesh.domain.Layout
+        Pmesh communication layout object for domain decomposition of the full
+        system. Used as blueprint by :code:`pmesh.pm.paint` and
+        :code:`pmesh.pm.readout` for exchange of particle information across
+        MPI ranks as necessary.
+    layouts: list[pmesh.domain.Layout]
+        Pmesh communication layout objects for domain decompositions of each
+        particle type. Used as blueprint by :code:`pmesh.pm.readout` for
+        exchange of particle information across MPI ranks as necessary.
+    pm : pmesh.pm.ParticleMesh
+        Pmesh :code:`ParticleMesh` object interfacing to the CIC window
+        function and the PFFT discrete Fourier transform library.
+    positions : (N,D) numpy.ndarray
+        Array of positions for :code:`N` particles in :code:`D` dimensions.
+        Local for each MPI rank.
+    config : hymd.input_parser.Config
+        Configuration object.
+    comm: mpi4py.Comm
+        MPI communicator to use for rank commuication.
+
+    See also
+    --------
+    compute_field_energy_q_GPE:
+        Compute the electrostatic energy after electrosatic force is
+        calculated for a variable (anisotropic) dielectric general Poisson equation.
+    """
+
+    ## basic setup
+    V = np.prod(config.box_size)
+    n_mesh_cells = np.prod(np.full(3, config.mesh_size))
+    volume_per_cell = V / n_mesh_cells
+    ## old protocol in gen_qe_hpf_use_self
+    pm.paint(positions, layout=layout_q, mass=charges, out=phi_q)  ##
+    ## scale and fft
+    ## old protocol in gen_qe_hpf_use_self
+    phi_q /= volume_per_cell
+    phi_q.r2c(out=phi_q_fourier)
+
+    phi_q_fourier.apply(hamiltonian.H, out=phi_q_fourier)
+    ## ^------ use the same gaussian as the \kai interaciton
+    phi_q_fourier.c2r(out=phi_q)  ## this phi_q is after applying the smearing function
+
+    denom_phi_tot = pm.create("real", value=0.0)
+    num_types = pm.create("real", value=0.0)
+    ### ^ ----- Calculate the relative dielectric (permittivity) to field
+    ### ------- from a mean contribution of particle number densities
+
+    for t_ in range(config.n_types):
+        num_types = num_types + (config.dielectric_type[t_]) * phi[t_]
+        denom_phi_tot = denom_phi_tot + phi[t_]
+
+    np.divide(num_types, denom_phi_tot, where=np.abs(denom_phi_tot > 1e-6), out=phi_eps)
+
+    phi_eps.r2c(out=phi_eps_fourier)  # FFT dielectric
+
+    # phi_q_eps = (phi_q/phi_eps)
+    np.divide(phi_q, phi_eps, where=np.abs(phi_eps > 1e-6), out=phi_q)
+
+    _SPACE_DIM = 3
+    ##^--------- constants needed throughout the calculations
+
+    ### method for finding the gradient (fourier space), using the spatial dimension of k
+    for _d in np.arange(_SPACE_DIM):
+
+        def gradient_transfer_function(k, x, d=_d):
+            return 1j * k[d] * x
+
+        phi_eps_fourier.apply(gradient_transfer_function, out=phi_eta_fourier[_d])
+        phi_eta_fourier[_d].c2r(out=phi_eta[_d])
+        np.divide(phi_eta[_d], phi_eps, where=np.abs(phi_eps > 1e-6), out=phi_eta[_d])
+
+    ### iterative GPE solver ###
+    ### ----------------------------------------------
+    max_iter = 100
+    i = 0
+    delta = 1.0
+    # phi_pol_prev = pm.create("real", value = 0.0)
+    ### ^------ set to zero before each iterative procedure or soft start
+    conv_criteria = config.conv_crit  # conv. criteria (default 1e-6)
+    w = config.pol_mixing  # polarization mixing param (default 0.6)
+    while i < max_iter and delta > conv_criteria:
+        (phi_q + phi_pol_prev).r2c(out=phi_q_fourier)
+        for _d in np.arange(_SPACE_DIM):
+
+            def iterate_apply_k_vec(k, additive_terms, d=_d):
+                return additive_terms * (-1j * k[d]) / k.normp(p=2, zeromode=1)
+
+            phi_q_fourier.apply(iterate_apply_k_vec, out=phi_eta_fourier[_d])
+            phi_eta_fourier[_d].c2r(out=elec_field[_d])
+
+        phi_pol = -(
+            phi_eta[0] * elec_field[0]
+            + phi_eta[1] * elec_field[1]
+            + phi_eta[2] * elec_field[2]
+        )
+        ### ^-- Following a negative sign convention (-ik) of the FT, a neg sign is
+        ### --- mathematically correct by the definition of the GPE (double  - -> +)
+        phi_pol = w * phi_pol + (1.0 - w) * phi_pol_prev
+        diff = np.abs(phi_pol - phi_pol_prev)
+        delta = conv_fun(comm, diff)  # decided from toml input
+        phi_pol_prev = phi_pol.copy()
+        i = i + 1
+    # print("Stopping after iteration {:d} with stop crit {:.2e}, delta {:.2e}".format(i,conv_criteria,delta))
+
+    # compute_potential = True
+    def k_norm_divide(k, potential):
+        return potential / k.normp(p=2, zeromode=1)
+
+    ## > Electrostatic potential
+    eps0_inv = config.coulomb_constant * 4 * np.pi
+    ## ^ the 1/(4pi eps0)*4*pi = 1/eps0
+    ((eps0_inv) * (phi_q + phi_pol)).r2c(out=phi_q_fourier)
+    phi_q_fourier.apply(k_norm_divide, out=phi_q_fourier)
+    phi_q_fourier.c2r(out=psi)
+    ### ^ electrostatic potential for the GPE
+
+    for _d in np.arange(_SPACE_DIM):
+
+        def field_transfer_function(k, x, d=_d):
+            return (
+                -1j * k[d] * x
+            )  ## negative sign relation, due to E = - nabla psi relation
+
+        phi_q_fourier.apply(field_transfer_function, out=phi_eta_fourier[_d])
+        phi_eta_fourier[_d].c2r(out=elec_field[_d])
+    ## ^-------- Method: Obtaining the electric field from electrostatic potential
+    ## Assuming the electric field is conserved.
+    ## Assumption holds if no magnetic flux (magnetic induced fields)
+
+    ##############  Obtain forces  ##############
+    elec_dot = (
+        elec_field[0] * elec_field[0]
+        + elec_field[1] * elec_field[1]
+        + elec_field[2] * elec_field[2]
+    )
+    # needed for energy calculations
+
+    np.divide(
+        elec_dot,
+        denom_phi_tot,
+        where=np.abs(denom_phi_tot > 1e-6),
+        out=elec_field_contrib,
+    )
+
+    eps0_inv = config.coulomb_constant * 4 * np.pi
+
+    for t_ in range(config.n_types):
+        Vbar_elec[t_] = (
+            config.type_charges[t_] * psi
+            - (0.5 / eps0_inv)
+            * (config.dielectric_type[t_] - phi_eps)
+            * elec_field_contrib
+        )
+
+    # Obtain Vext,k
+    for t_ in range(config.n_types):
+        Vbar_elec[t_].r2c(out=Vbar_elec_fourier[t_])
+        Vbar_elec_fourier[t_].apply(hamiltonian.H, out=Vbar_elec_fourier[t_])
+
+    # force terms
+    # F = - grad Vext
+    for t_ in range(config.n_types):
+        for _d in np.arange(_SPACE_DIM):
+
+            def force_transfer_function(k, x, d=_d):
+                return -1j * k[_d] * x  ## negative gradient
+
+            Vbar_elec_fourier[t_].apply(
+                force_transfer_function, out=force_mesh_elec_fourier[t_][_d]
+            )
+            force_mesh_elec_fourier[t_][_d].c2r(out=force_mesh_elec[t_][_d])
+            elec_forces[types == t_, _d] = force_mesh_elec[t_][_d].readout(
+                positions[types == t_], layout=layouts[t_]
+            )
+
+    return Vbar_elec, phi_eps, elec_dot
 
 
 def domain_decomposition(
-    positions, pm, *args, molecules=None, bonds=None, verbose=0,
-    comm=MPI.COMM_WORLD
+    positions, pm, *args, molecules=None, bonds=None, verbose=0, comm=MPI.COMM_WORLD
 ):
     """Performs domain decomposition
 
     Rearranges the MPI rank memory layout into one that better mimics the PFFT
     pencil grid 2D decomposition. As molecules are always required to be fully
     contained on a single MPI rank, a perfect decomposition is not always
     possible. The best decomposition which leaves the center of mass of all
```

### Comparing `hymd-1.0.9/hymd/file_io.py` & `hymd-2.0.1/hymd/file_io.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,22 @@
 import logging
 import getpass
 from mpi4py import MPI
 from .logger import Logger, get_version
 
 
 class OutDataset:
-    """HDF5 dataset handler for file output
-    """
+    """HDF5 dataset handler for file output"""
 
     def __init__(
-        self, dest_directory, config, double_out=False, disable_mpio=False,
+        self,
+        dest_directory,
+        config,
+        double_out=False,
+        disable_mpio=False,
         comm=MPI.COMM_WORLD,
     ):
         """Constructor
 
         Parameters
         ----------
         dest_directory : str
@@ -44,23 +47,21 @@
             self.float_dtype = "float64"
         else:
             self.float_dtype = "float32"
 
         if disable_mpio:
             self.file = h5py.File(
                 os.path.join(
-                    dest_directory,
-                    f"sim.hdf5-{comm.rank:6d}-of-{comm.size:6d}"
+                    dest_directory, f"sim.hdf5-{comm.rank:6d}-of-{comm.size:6d}"
                 ),
                 "w",
             )
         else:
             self.file = h5py.File(
-                os.path.join(dest_directory, "sim.H5"), "w", driver="mpio",
-                comm=comm
+                os.path.join(dest_directory, "sim.H5"), "w", driver="mpio", comm=comm
             )
 
     def is_open(self, comm=MPI.COMM_WORLD):
         """Check if HDF5 output file is open
 
         Parameters
         ----------
@@ -78,16 +79,15 @@
         comm : mpi4py.Comm
             MPI communicator to use for rank communication.
         """
         comm.Barrier()
         self.file.close()
 
     def flush(self):
-        """Flushes output buffers, forcing file writes
-        """
+        """Flushes output buffers, forcing file writes"""
         self.file.flush()
 
 
 def setup_time_dependent_element(
     name, parent_group, n_frames, shape, dtype, units=None
 ):
     """Helper function for setting up time-dependent HDF5 group datasets
@@ -108,23 +108,36 @@
     H5MD specification :
         https://www.nongnu.org/h5md/h5md.html
     """  # noqa: E501
     group = parent_group.create_group(name)
     step = group.create_dataset("step", (n_frames,), "int32")
     time = group.create_dataset("time", (n_frames,), "float32")
     value = group.create_dataset("value", (n_frames, *shape), dtype)
+
     if units is not None:
-        group.attrs["units"] = units
+        value.attrs["unit"] = units
+        time.attrs["unit"] = "ps"
     return group, step, time, value
 
 
 def store_static(
-    h5md, rank_range, names, types, indices, config, bonds_2_atom1,
-    bonds_2_atom2, molecules=None, velocity_out=False, force_out=False,
-    charges=False, comm=MPI.COMM_WORLD,
+    h5md,
+    rank_range,
+    names,
+    types,
+    indices,
+    config,
+    bonds_2_atom1,
+    bonds_2_atom2,
+    molecules=None,
+    velocity_out=False,
+    force_out=False,
+    charges=False,
+    dielectrics=False,
+    comm=MPI.COMM_WORLD,
 ):
     """Outputs all static time-independent quantities to the HDF5 output file
 
     Parameters
     ----------
     h5md : OutDataset
         HDF5 dataset handler.
@@ -150,14 +163,16 @@
         only) may be used, both, without affecting the result.
     velocity_out : bool, optional
         If :code:`True`, velocities are written to output HDF5 file.
     force_out : bool, optional
         If :code:`True`, forces are written to output HDF5 file.
     charges : (N,) numpy.ndarray
         Array of particle charge values for :code:`N` particles.
+    dielectrics : (N,) numpy.ndarray
+        Array of particle relative dielectric values for :code:`N` particles.
     comm : mpi4py.Comm
         MPI communicator to use for rank commuication.
 
     See also
     --------
     prepare_bonds :
         Constructs two-, three-, and four-particle bonds from toplogy input
@@ -192,43 +207,46 @@
         except:
             pass
     except:
         pass
 
     h5md.particles_group = h5md.file.create_group("/particles")
     h5md.all_particles = h5md.particles_group.create_group("all")
-    mass = h5md.all_particles.create_dataset(
-        "mass", (config.n_particles,), dtype
-    )
+    mass = h5md.all_particles.create_dataset("mass", (config.n_particles,), dtype)
     mass[...] = config.mass
 
     if charges is not False:
         charge = h5md.all_particles.create_dataset(
             "charge", (config.n_particles,), dtype="float32"
         )
         charge[indices] = charges
+    if dielectrics is not False:
+        dielectric = h5md.all_particles.create_dataset(
+            "dielectric", (config.n_particles,), dtype="float32"
+        )
+        dielectric[indices] = dielectrics
 
     box = h5md.all_particles.create_group("box")
     box.attrs["dimension"] = 3
     box.attrs["boundary"] = np.array(
         [np.string_(s) for s in 3 * ["periodic"]], dtype="S8"
     )
-    h5md.edges = box.create_dataset("edges", (3,), dtype)
-    h5md.edges[:] = np.array(config.box_size)
 
     n_frames = config.n_steps // config.n_print
     if np.mod(config.n_steps - 1, config.n_print) != 0:
         n_frames += 1
     if np.mod(config.n_steps, config.n_print) == 1:
         n_frames += 1
     if n_frames == config.n_steps:
         n_frames += 1
 
     species = h5md.all_particles.create_dataset(
-        "species", (config.n_particles,), dtype="i",
+        "species",
+        (config.n_particles,),
+        dtype="i",
     )
 
     (
         _,
         h5md.positions_step,
         h5md.positions_time,
         h5md.positions,
@@ -262,81 +280,122 @@
             h5md.forces,
         ) = setup_time_dependent_element(
             "force",
             h5md.all_particles,
             n_frames,
             (config.n_particles, 3),
             dtype,
-            units="kJ nm mol-1",
+            units="kJ mol-1 nm-1",
         )
     (
         _,
         h5md.total_energy_step,
         h5md.total_energy_time,
         h5md.total_energy,
     ) = setup_time_dependent_element(
-        "total_energy", h5md.observables, n_frames, (1,), dtype, units="kJ mol-1"  # noqa: E501
+        "total_energy",
+        h5md.observables,
+        n_frames,
+        (1,),
+        dtype,
+        units="kJ mol-1",  # noqa: E501
     )
     (
         _,
         h5md.kinetc_energy_step,
         h5md.kinetc_energy_time,
         h5md.kinetc_energy,
     ) = setup_time_dependent_element(
-        "kinetic_energy", h5md.observables, n_frames, (1,), dtype, units="kJ mol-1"  # noqa: E501
+        "kinetic_energy",
+        h5md.observables,
+        n_frames,
+        (1,),
+        dtype,
+        units="kJ mol-1",  # noqa: E501
     )
     (
         _,
         h5md.potential_energy_step,
         h5md.potential_energy_time,
         h5md.potential_energy,
     ) = setup_time_dependent_element(
-        "potential_energy", h5md.observables, n_frames, (1,), dtype, units="kJ mol-1"  # noqa: E501
+        "potential_energy",
+        h5md.observables,
+        n_frames,
+        (1,),
+        dtype,
+        units="kJ mol-1",  # noqa: E501
     )
     (
         _,
         h5md.bond_energy_step,
         h5md.bond_energy_time,
         h5md.bond_energy,
     ) = setup_time_dependent_element(
-        "bond_energy", h5md.observables, n_frames, (1,), dtype, units="kJ mol-1"  # noqa: E501
+        "bond_energy",
+        h5md.observables,
+        n_frames,
+        (1,),
+        dtype,
+        units="kJ mol-1",  # noqa: E501
     )
     (
         _,
         h5md.angle_energy_step,
         h5md.angle_energy_time,
         h5md.angle_energy,
     ) = setup_time_dependent_element(
-        "angle_energy", h5md.observables, n_frames, (1,), dtype, units="kJ mol-1"  # noqa: E501
+        "angle_energy",
+        h5md.observables,
+        n_frames,
+        (1,),
+        dtype,
+        units="kJ mol-1",  # noqa: E501
     )
     (
         _,
         h5md.dihedral_energy_step,
         h5md.dihedral_energy_time,
         h5md.dihedral_energy,
     ) = setup_time_dependent_element(
-        "dihedral_energy", h5md.observables, n_frames, (1,), dtype, units="kJ mol-1"  # noqa: E501
+        "dihedral_energy",
+        h5md.observables,
+        n_frames,
+        (1,),
+        dtype,
+        units="kJ mol-1",  # noqa: E501
     )
     (
         _,
         h5md.field_energy_step,
         h5md.field_energy_time,
         h5md.field_energy,
     ) = setup_time_dependent_element(
-        "field_energy", h5md.observables, n_frames, (1,), dtype, units="kJ mol-1"  # noqa: E501
+        "field_energy",
+        h5md.observables,
+        n_frames,
+        (1,),
+        dtype,
+        units="kJ mol-1",  # noqa: E501
     )
     if charges is not False:
         (
             _,
             h5md.field_q_energy_step,
             h5md.field_q_energy_time,
             h5md.field_q_energy,
         ) = setup_time_dependent_element(
-            "field_q_energy", h5md.observables, n_frames, (1,), dtype, units="kJ mol-1"  # noqa: E501
+            "field_q_energy",
+            h5md.observables,
+            n_frames,
+            (1,),
+            dtype,
+            units="kJ mol-1",  # noqa: E501
         )  # <-------- xinmeng
+
     (
         _,
         h5md.total_momentum_step,
         h5md.total_momentum_time,
         h5md.total_momentum,
     ) = setup_time_dependent_element(  # noqa: E501
         "total_momentum",
@@ -382,15 +441,31 @@
     )
     (
         _,
         h5md.thermostat_work_step,
         h5md.thermostat_work_time,
         h5md.thermostat_work,
     ) = setup_time_dependent_element(
-        "thermostat_work", h5md.observables, n_frames, (1,), "float32", units="kJ mol-1"  # noqa: E501
+        "thermostat_work",
+        h5md.observables,
+        n_frames,
+        (1,),
+        "float32",
+        units="kJ mol-1",  # noqa: E501
+    )
+    (
+        _,
+        h5md.pressure_step,
+        h5md.pressure_time,
+        h5md.pressure,
+    ) = setup_time_dependent_element(
+        "pressure", h5md.observables, n_frames, (18,), "float32", units="Bar"
+    )
+    (_, h5md.box_step, h5md.box_time, h5md.box_value,) = setup_time_dependent_element(
+        "edges", box, n_frames, (3, 3), "float32", units="nm"
     )
 
     ind_sort = np.argsort(indices)
     for i in ind_sort:
         species[indices[i]] = config.name_to_type_map[names[i].decode("utf-8")]
 
     h5md.parameters.attrs["config.toml"] = np.string_(str(config))
@@ -402,15 +477,17 @@
 
     # VMD-h5mdplugin maximum name/type name length is 16 characters (for
     # whatever reason [VMD internals?]).
     name_dataset = vmd_group.create_dataset("name", (config.n_types,), "S16")
     type_dataset = vmd_group.create_dataset("type", (config.n_types,), "S16")
     if molecules is not None:
         resid_dataset = vmd_group.create_dataset(
-            "resid", (config.n_particles,), "i",
+            "resid",
+            (config.n_particles,),
+            "i",
         )
 
     # Change this
     for i, n in config.type_to_name_map.items():
         name_dataset[i] = np.string_(n[:16])
         if n == "W":
             type_dataset[i] = np.string_("solvent")
@@ -435,19 +512,46 @@
         bonds_from[rank_bond_start + i] = indices[a] + 1
         bonds_to[rank_bond_start + i] = indices[b] + 1
 
     if molecules is not None:
         resid_dataset[indices[ind_sort]] = molecules
 
 
+# store data old vs
+"""
+h5md, step, frame, indices, positions, velocities, forces, box_size,
+temperature, kinetic_energy, bond2_energy, bond3_energy, bond4_energy,
+field_energy, field_q_energy, time_step, config, velocity_out=False,
+force_out=False, charge_out=False, dump_per_particle=False,
+"""
+
+
 def store_data(
-    h5md, step, frame, indices, positions, velocities, forces, box_size,
-    temperature, kinetic_energy, bond2_energy, bond3_energy, bond4_energy,
-    field_energy, field_q_energy, time_step, config, velocity_out=False,
-    force_out=False, charge_out=False, dump_per_particle=False,
+    h5md,
+    step,
+    frame,
+    indices,
+    positions,
+    velocities,
+    forces,
+    box_size,
+    temperature,
+    pressure,
+    kinetic_energy,
+    bond2_energy,
+    bond3_energy,
+    bond4_energy,
+    field_energy,
+    field_q_energy,
+    time_step,
+    config,
+    velocity_out=False,
+    force_out=False,
+    charge_out=False,
+    dump_per_particle=False,
     comm=MPI.COMM_WORLD,
 ):
     """Writes time-step data to HDF5 output file
 
     Handles all quantities which change during simulation, as opposed to
     static quanitities (see :code:`store_static`).
 
@@ -513,14 +617,16 @@
         h5md.angle_energy_step,
         h5md.dihedral_energy_step,
         h5md.field_energy_step,
         h5md.total_momentum_step,
         h5md.angular_momentum_step,
         h5md.torque_step,
         h5md.temperature_step,
+        h5md.pressure_step,
+        h5md.box_step,
         h5md.thermostat_work_step,
     ):
         dset[frame] = step
 
     for dset in (
         h5md.positions_time,
         h5md.total_energy_time,
@@ -530,14 +636,16 @@
         h5md.angle_energy_time,
         h5md.dihedral_energy_time,
         h5md.field_energy_time,
         h5md.total_momentum_time,
         h5md.angular_momentum_time,
         h5md.torque_time,
         h5md.temperature_time,
+        h5md.pressure_time,
+        h5md.box_time,
         h5md.thermostat_work_time,
     ):
         dset[frame] = step * time_step
 
     if velocity_out:
         h5md.velocities_step[frame] = step
         h5md.velocities_time[frame] = step * time_step
@@ -555,21 +663,18 @@
         h5md.velocities[frame, indices[ind_sort]] = velocities[ind_sort]
     if force_out:
         h5md.forces[frame, indices[ind_sort]] = forces[ind_sort]
     if charge_out:
         h5md.field_q_energy[frame] = field_q_energy
 
     potential_energy = (
-        bond2_energy + bond3_energy + bond4_energy + field_energy
-        + field_q_energy
+        bond2_energy + bond3_energy + bond4_energy + field_energy + field_q_energy
     )
 
-    total_momentum = config.mass * comm.allreduce(
-        np.sum(velocities, axis=0), MPI.SUM
-    )
+    total_momentum = config.mass * comm.allreduce(np.sum(velocities, axis=0), MPI.SUM)
     angular_momentum = config.mass * comm.allreduce(
         np.sum(np.cross(positions, velocities), axis=0), MPI.SUM
     )
     torque = config.mass * comm.allreduce(
         np.sum(np.cross(positions, forces), axis=0), MPI.SUM
     )
     h5md.total_energy[frame] = kinetic_energy + potential_energy
@@ -579,14 +684,17 @@
     h5md.angle_energy[frame] = bond3_energy
     h5md.dihedral_energy[frame] = bond4_energy
     h5md.field_energy[frame] = field_energy
     h5md.total_momentum[frame, :] = total_momentum
     h5md.angular_momentum[frame, :] = angular_momentum
     h5md.torque[frame, :] = torque
     h5md.temperature[frame] = temperature
+    h5md.pressure[frame] = pressure
+    for d in range(3):
+        h5md.box_value[frame, d, d] = box_size[d]
     h5md.thermostat_work[frame] = config.thermostat_work
 
     fmt_ = [
         "step",
         "time",
         "temp",
         "tot E",
@@ -599,42 +707,42 @@
         "dih E",
         "Px",
         "Py",
         "Pz",
         "ΔH" if config.target_temperature else "ΔE",
     ]
     fmt_ = np.array(fmt_)
-    
+
     # create mask to show only energies != 0
-    en_array = np.array([
-        field_energy,
-        field_q_energy,
-        bond2_energy,
-        bond3_energy,
-        bond4_energy,
-    ])
+    en_array = np.array(
+        [
+            field_energy,
+            field_q_energy,
+            bond2_energy,
+            bond3_energy,
+            bond4_energy,
+        ]
+    )
     mask = np.full_like(fmt_, True, dtype=bool)
-    mask[range(6,11)] = en_array != 0.
+    mask[range(6, 11)] = en_array != 0.0
 
     header_ = fmt_[mask].shape[0] * "{:>13}"
     if config.initial_energy is None:
         fmt_[-1] = ""
 
     divide_by = 1.0
     if dump_per_particle:
         for i in range(3, 9):
             fmt_[i] = fmt_[i][:-2] + "E/N"
         fmt_[-1] += "/N"
         divide_by = config.n_particles
     total_energy = kinetic_energy + potential_energy
     if config.initial_energy is not None:
         if config.target_temperature:
-            H_tilde = (
-                total_energy - config.initial_energy - config.thermostat_work
-            )
+            H_tilde = total_energy - config.initial_energy - config.thermostat_work
         else:
             H_tilde = total_energy - config.initial_energy
     else:
         H_tilde = 0.0
 
     header = header_.format(*fmt_[mask])
     data_fmt = f'{"{:13}"}{(fmt_[mask].shape[0]-1) * "{:13.5g}" }'
@@ -651,21 +759,20 @@
         bond3_energy / divide_by,
         bond4_energy / divide_by,
         total_momentum[0] / divide_by,
         total_momentum[1] / divide_by,
         total_momentum[2] / divide_by,
         H_tilde / divide_by,
     ]
-    data = data_fmt.format(*[val for i,val in enumerate(all_data) if mask[i]])
+    data = data_fmt.format(*[val for i, val in enumerate(all_data) if mask[i]])
     Logger.rank0.log(logging.INFO, ("\n" + header + "\n" + data))
 
 
 def distribute_input(
-    in_file, rank, size, n_particles, max_molecule_size=201,
-    comm=MPI.COMM_WORLD
+    in_file, rank, size, n_particles, max_molecule_size=201, comm=MPI.COMM_WORLD
 ):
     """Assign global arrays onto MPI ranks, attempting load balancing
 
     Distributes approximately equal numbers of particles (workload) onto each
     independent MPI rank, while respecting the requirement that any molecule
     must be fully contained on a single MPI rank only (no splitting molecules
     across multiple CPUs).
@@ -713,17 +820,15 @@
     # To avoid splitting molecules across multiple different ranks, we need
     # to read in some extra indices before/after the expected break points
     # and iterate until we find a molecule break.
     #
     # Implicitly assuming no molecule is bigger than
     # min(max_molecule_size, n_particles // n_MPI_ranks) atoms.
     max_molecule_size += 2
-    grab_extra = (
-        max_molecule_size if np_per_MPI > max_molecule_size else np_per_MPI
-    )
+    grab_extra = max_molecule_size if np_per_MPI > max_molecule_size else np_per_MPI
     if rank == 0:
         mpi_range_start = 0
         if size == 1:
             mpi_range_end = n_particles
         else:
             mpi_range_end = (rank + 1) * np_per_MPI + grab_extra
     elif rank == size - 1:
@@ -743,19 +848,16 @@
         if size == 1:
             p_mpi_range[1] = n_particles
         else:
             p_mpi_range[1] = indices[
                 molecule_end_indices[molecule_end_indices >= np_per_MPI][0] + 1
             ]
     elif rank == size - 1:
-        p_mpi_range[0] = (
-            indices[molecule_end_indices[molecule_end_indices > 0][0]] + 1
-        )
+        p_mpi_range[0] = indices[molecule_end_indices[molecule_end_indices > 0][0]] + 1
         p_mpi_range[1] = n_particles
     else:
-        p_mpi_range[0] = (
-            indices[molecule_end_indices[molecule_end_indices > 0][0]] + 1
-        )
+        p_mpi_range[0] = indices[molecule_end_indices[molecule_end_indices > 0][0]] + 1
         p_mpi_range[1] = (
-            indices[molecule_end_indices[molecule_end_indices > np_per_MPI][0]] + 1  # noqa: E501
+            indices[molecule_end_indices[molecule_end_indices > np_per_MPI][0]]
+            + 1  # noqa: E501
         )
     return list(range(p_mpi_range[0], p_mpi_range[1])), molecules_flag
```

### Comparing `hymd-1.0.9/hymd/force.py` & `hymd-2.0.1/hymd/force.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Calculates intramolecular forces between bonded particles in molecules
 """
 import numpy as np
 import networkx as nx
 from dataclasses import dataclass
 
 # Imported here so we can call from force import compute_bond_forces__fortran
-from force_kernels import (  # noqa: F401
-    cbf as compute_bond_forces__fortran
-)
+from force_kernels import cbf as compute_bond_forces__fortran  # noqa: F401
 from force_kernels import (  # noqa: F401
     caf as compute_angle_forces__fortran,
 )
 from force_kernels import (  # noqa: F401
     cdf as compute_dihedral_forces__fortran,
 )
 from force_kernels import (  # noqa: F401
@@ -21,14 +19,20 @@
     caf_d as compute_angle_forces__fortran__double,
 )
 from force_kernels import (  # noqa: F401
     cdf_d as compute_dihedral_forces__fortran__double,
 )
 
 
+@dataclass  # might not be needed
+class Dielectric_type:
+    atom_1: str
+    dielectric_value: float
+
+
 @dataclass
 class Bond:
     """Dataclass representing a single two-particle bond type
 
     A `bond type` is a bond strength and equilibrium distance associated with
     any bond between particles of specific types :code:`A` and :code:`B`
     (where :code:`A` and :code:`B` may be the same or different). Harmonic
@@ -53,14 +57,15 @@
         Type name of particle 2.
     equilibrium : float
         Equilibrium distance at which the energy associated with the bond
         vanishes and the resulting force is zero.
     strength : float
         Harmonic bond strength coefficient (spring constant).
     """
+
     atom_1: str
     atom_2: str
     equilibrium: float
     strength: float
 
 
 @dataclass
@@ -107,14 +112,15 @@
         Harmonic bond strength coefficient.
 
     See also
     --------
     Bond :
         Two-particle bond type dataclass
     """
+
     atom_3: str
 
 
 @dataclass
 class Dihedral:
     """Dataclass representing a single four-particle bond type
 
@@ -201,14 +207,15 @@
         :math:`V_\\text{prop}` propensity potential, defined in terms of cosine
         series.
 
     References
     ----------
     Bore et al. J. Chem. Theory Comput., 14(2): 1120–1130, 2018.
     """
+
     atom_1: str
     atom_2: str
     atom_3: str
     atom_4: str
     coeffs: np.ndarray
     dih_type: int
 
@@ -247,14 +254,15 @@
         Interaction mixing energy.
 
     See also
     --------
     hymd.hamiltonian.DefaultWithChi :
         Interaction energy functional using :math:`\\chi`-interactions.
     """
+
     atom_1: str
     atom_2: str
     interaction_energy: float
 
 
 def find_all_paths(G, u, n):
     """Helper function that recursively finds all paths of given lenght 'n + 1' inside a network 'G'.
@@ -364,20 +372,16 @@
             connected = c[1]
             for j, path in connected.items():
                 if len(path) == 2 and path[-1] > path[0]:
                     name_i = bond_graph.nodes()[i]["name"]
                     name_j = bond_graph.nodes()[j]["name"]
 
                     for b in config.bonds:
-                        match_forward = (
-                            name_i == b.atom_1 and name_j == b.atom_2
-                        )
-                        match_backward = (
-                            name_i == b.atom_2 and name_j == b.atom_1
-                        )
+                        match_forward = name_i == b.atom_1 and name_j == b.atom_2
+                        match_backward = name_i == b.atom_2 and name_j == b.atom_1
                         if match_forward or match_backward:
                             bonds_2.append(
                                 [
                                     bond_graph.nodes()[i]["local_index"],
                                     bond_graph.nodes()[j]["local_index"],
                                     b.equilibrium,
                                     b.strength,
@@ -452,15 +456,69 @@
 
         if bb_dihedral:
             bb_index.append(bb_dihedral - 1)
 
     return bonds_2, bonds_3, bonds_4, bb_index
 
 
-def prepare_bonds(molecules, names, bonds, indices, config):
+def prepare_index_based_bonds(molecules, topol):
+    bonds_2 = []
+    bonds_3 = []
+    bonds_4 = []
+
+    different_molecules = np.unique(molecules)
+    for mol in different_molecules:
+        resid = mol + 1
+        top_summary = topol["system"]["molecules"]
+        resname = None
+        test_mol_number = 0
+        for molname in top_summary:
+            test_mol_number += molname[1]
+            if resid <= test_mol_number:
+                resname = molname[0]
+                break
+
+        if resname is None:
+            break
+
+        if "bonds" in topol[resname]:
+            first_id = np.where(molecules == mol)[0][0]
+            for bond in topol[resname]["bonds"]:
+                index_i = bond[0] - 1 + first_id
+                index_j = bond[1] - 1 + first_id
+                # bond[2] is the bond type, inherited by the itp format. Not used
+                equilibrium = bond[3]
+                strength = bond[4]
+                bonds_2.append([index_i, index_j, equilibrium, strength])
+
+        if "angles" in topol[resname]:
+            first_id = np.where(molecules == mol)[0][0]
+            for angle in topol[resname]["angles"]:
+                index_i = angle[0] - 1 + first_id
+                index_j = angle[1] - 1 + first_id
+                index_k = angle[2] - 1 + first_id
+                # angle[3] is the angle type, inherited by the itp format. Not used
+                equilibrium = np.radians(angle[4])
+                strength = angle[5]
+                bonds_3.append([index_i, index_j, index_k, equilibrium, strength])
+
+        if "dihedrals" in topol[resname]:
+            first_id = np.where(molecules == mol)[0][0]
+            for angle in topol[resname]["dihedrals"]:
+                index_i = angle[0] - 1 + first_id
+                index_j = angle[1] - 1 + first_id
+                index_k = angle[2] - 1 + first_id
+                index_l = angle[3] - 1 + first_id
+                dih_type = angle[4]
+                coeff = angle[5]
+                bonds_4.append([index_i, index_j, index_k, index_l, coeff, dih_type, 0])
+    return bonds_2, bonds_3, bonds_4
+
+
+def prepare_bonds(molecules, names, bonds, indices, config, topol=None):
     """Rearrange the bond information for usage in compiled Fortran kernels
 
     Restructures the lists resulting from the execution of
     :code:`prepare_bonds_old` into numpy arrays suitable for calls to optimized
     Fortran code calculating bonded forces and energiesself.
 
     Parameters
@@ -534,17 +592,22 @@
     See also
     --------
     prepare_bonds_old :
         Used internally to reconstruct the bonded interactions types from the
         connectivity information in the structure/topology input file and the
         bonded types specified in the configuration file.
     """
-    bonds_2, bonds_3, bonds_4, bb_index = prepare_bonds_old(
-        molecules, names, bonds, indices, config
-    )
+    if topol is not None:
+        bonds_2, bonds_3, bonds_4 = prepare_index_based_bonds(
+            molecules, topol
+        )
+    else:
+        bonds_2, bonds_3, bonds_4, bb_index = prepare_bonds_old(
+            molecules, names, bonds, indices, config
+        )
 
     # Bonds
     bonds_2_atom1 = np.empty(len(bonds_2), dtype=int)
     bonds_2_atom2 = np.empty(len(bonds_2), dtype=int)
     bonds_2_equilibrium = np.empty(len(bonds_2), dtype=np.float64)
     bonds_2_strength = np.empty(len(bonds_2), dtype=np.float64)
     for i, b in enumerate(bonds_2):
@@ -561,15 +624,14 @@
     bonds_3_strength = np.empty(len(bonds_3), dtype=np.float64)
     for i, b in enumerate(bonds_3):
         bonds_3_atom1[i] = b[0]
         bonds_3_atom2[i] = b[1]
         bonds_3_atom3[i] = b[2]
         bonds_3_equilibrium[i] = b[3]
         bonds_3_strength[i] = b[4]
-
     # Dihedrals
     bonds_4_atom1 = np.empty(len(bonds_4), dtype=int)
     bonds_4_atom2 = np.empty(len(bonds_4), dtype=int)
     bonds_4_atom3 = np.empty(len(bonds_4), dtype=int)
     bonds_4_atom4 = np.empty(len(bonds_4), dtype=int)
     number_of_coeff = 6
     len_of_coeff = 5
@@ -581,20 +643,36 @@
     for i, b in enumerate(bonds_4):
         bonds_4_atom1[i] = b[0]
         bonds_4_atom2[i] = b[1]
         bonds_4_atom3[i] = b[2]
         bonds_4_atom4[i] = b[3]
         bonds_4_coeff[i] = np.resize(b[4], (number_of_coeff, len_of_coeff))
         bonds_4_type[i] = b[5]
-    bonds_4_last[bb_index] = 1
+        if topol is not None:
+            bonds_4_last[i] = b[6]
+    if topol is None:
+        bonds_4_last[bb_index] = 1
 
     return (
-        bonds_2_atom1, bonds_2_atom2, bonds_2_equilibrium, bonds_2_strength,
-        bonds_3_atom1, bonds_3_atom2, bonds_3_atom3, bonds_3_equilibrium, bonds_3_strength,  # noqa: E501
-        bonds_4_atom1, bonds_4_atom2, bonds_4_atom3, bonds_4_atom4, bonds_4_coeff, bonds_4_type, bonds_4_last,  # noqa: E501
+        bonds_2_atom1,
+        bonds_2_atom2,
+        bonds_2_equilibrium,
+        bonds_2_strength,
+        bonds_3_atom1,
+        bonds_3_atom2,
+        bonds_3_atom3,
+        bonds_3_equilibrium,
+        bonds_3_strength,  # noqa: E501
+        bonds_4_atom1,
+        bonds_4_atom2,
+        bonds_4_atom3,
+        bonds_4_atom4,
+        bonds_4_coeff,
+        bonds_4_type,
+        bonds_4_last,  # noqa: E501
     )
 
 
 def compute_bond_forces__plain(f_bonds, r, bonds_2, box_size):
     """Computes forces resulting from bonded interactions
 
     .. deprecated:: 1.0.0
@@ -643,15 +721,15 @@
         xra = 1.0 / np.sqrt(np.dot(ra, ra))
         xrc = 1.0 / np.sqrt(np.dot(rc, rc))
         ea = ra * xra
         ec = rc * xrc
 
         cosphi = np.dot(ea, ec)
         theta = np.arccos(cosphi)
-        xsinph = 1.0 / np.sqrt(1.0 - cosphi ** 2)
+        xsinph = 1.0 / np.sqrt(1.0 - cosphi**2)
 
         d = theta - theta0
         f = -k * d
 
         xrasin = xra * xsinph * f
         xrcsin = xrc * xsinph * f
 
@@ -717,22 +795,22 @@
         f_dihedrals[d, :] += force_on_d
     return energy
 
 
 def dipole_forces_redistribution(
     f_on_bead, f_dipoles, trans_matrices, a, b, c, d, type_array, last_bb
 ):
-    """Redistribute electrostatic forces calculated from topologically 
+    """Redistribute electrostatic forces calculated from topologically
     reconstructed ghost dipole point charges to the backcone atoms of the protein.
     """
     f_on_bead.fill(0.0)
     for i, j, k, l, fd, matrix, dih_type, is_last in zip(
         a, b, c, d, f_dipoles, trans_matrices, type_array, last_bb
     ):
-        if dih_type ==1:
+        if dih_type == 1:
             sum_force = fd[0] + fd[1]
             diff_force = fd[0] - fd[1]
             f_on_bead[i] += matrix[0] @ diff_force  # Atom A
             f_on_bead[j] += matrix[1] @ diff_force + 0.5 * sum_force  # Atom B
             f_on_bead[k] += matrix[2] @ diff_force + 0.5 * sum_force  # Atom C
 
             if is_last == 1:
```

### Comparing `hymd-1.0.9/hymd/gaussian_core.py` & `hymd-2.0.1/hymd/gaussian_core.py`

 * *Files identical despite different names*

### Comparing `hymd-1.0.9/hymd/input_parser.py` & `hymd-2.0.1/hymd/input_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import datetime
 import logging
 import warnings
 import numpy as np
 from mpi4py import MPI
 from dataclasses import dataclass, field
 from typing import List, Union, ClassVar
-from .force import Bond, Angle, Dihedral, Chi
+from .force import Bond, Angle, Dihedral, Chi, Dielectric_type
+from .barostat import Target_pressure
 from .logger import Logger
 
 
 @dataclass
 class Config:
     """Configuration object
 
@@ -134,34 +135,42 @@
         keyword is set to :code:`"PIC_Spectral"`.
     dielectric_const : float, optional
         Specifies the relative dielectric constant of the simulation medium
         which regulates the strength of the electrostatic interactions. When
         using helical propensity dihedrals, this keyword must be specified—even
         if electrostatics are not included with the :code:`coulombtype`
         keyword.
+    dielectric_type: list[float], optional
+        Specifies the relative dielectric constant of the simulation medium
+        which regulates the strength of the electrostatic interactions. The list assigns
+        relative dielectric values to each bead type, and an anisotropic
+        dielectric function is obtained from a weighted average.
+
 
     See also
     --------
     hymd.input_parser.Bond :
         Two-particle bond type dataclass.
     hymd.input_parser.Angle :
         Three-particle bond type dataclass.
     hymd.input_parser.Dihedral :
         Four-particle bond type dataclass.
     """
+
     gas_constant: ClassVar[float] = 0.0083144621  # kJ mol-1 K-1
     coulomb_constant: ClassVar[float] = 138.935458  # kJ nm mol-1 e-2
 
     n_steps: int
     time_step: float
-    box_size: Union[List[float], np.ndarray]
     mesh_size: Union[Union[List[int], np.ndarray], int]
     sigma: float
     kappa: float
 
+    dtype: np.dtype = None
+    box_size: Union[List[float], np.ndarray] = None
     n_print: int = None
     tau: float = None
     start_temperature: Union[float, bool] = None
     target_temperature: Union[float, bool] = None
     mass: float = None
     hamiltonian: str = None
     domain_decomposition: Union[int, bool] = None
@@ -178,23 +187,43 @@
     max_molecule_size: int = None
     n_flush: int = None
     thermostat_work: float = 0.0
     thermostat_coupling_groups: List[List[str]] = field(default_factory=list)
     initial_energy: float = None
     cancel_com_momentum: Union[int, bool] = False
     coulombtype: str = None
+    convergence_type: str = None
+    pol_mixing: float = None
     dielectric_const: float = None
+    conv_crit: float = None
+    dielectric_type: List[Dielectric_type] = field(default_factory=list)
+    self_energy: float = None
+    type_charges: Union[List[float], np.ndarray] = None
+
+    # For NPT runs
+    rho0: float = None
+    a: float = None
+    pressure: bool = False
+    barostat: str = None
+    barostat_type: str = None
+    tau_p: float = None
+    target_pressure: List[Target_pressure] = field(default_factory=list)
+    n_b: int = None
+    m: List[float] = field(default_factory=list)
 
     def __str__(self):
+        target_pressure_str = "\ttarget_pressure:\n" + "".join(
+            "\t\tP_L: "
+            + f"{self.target_pressure.P_L}\n"
+            + "\t\tP_N: "
+            + f"{self.target_pressure.P_N}\n"
+        )
         bonds_str = "\tbonds:\n" + "".join(
             [
-                (
-                    f"\t\t{k.atom_1} {k.atom_2}: "
-                    f"{k.equilibrium}, {k.strength}\n"
-                )
+                (f"\t\t{k.atom_1} {k.atom_2}: " f"{k.equilibrium}, {k.strength}\n")
                 for k in self.bonds
             ]
         )
         angle_str = "\tangle_bonds:\n" + "".join(
             [
                 (
                     f"\t\t{k.atom_1} {k.atom_2} {k.atom_3}: "
@@ -207,45 +236,52 @@
             [
                 (
                     f"\t\t{k.atom_1} {k.atom_2} {k.atom_3} {k.atom_4}: "
                     # This might need to be fixed/made prettier, probably
                     # there's an easier way
                     + (
                         "\n\t\t"
-                        + " " * len(
-                            f"{k.atom_1} {k.atom_2} {k.atom_3} {k.atom_4}: "
-                        )
+                        + " " * len(f"{k.atom_1} {k.atom_2} {k.atom_3} {k.atom_4}: ")
                     ).join(
                         map(
                             str,
                             [
                                 [round(num, 3) for num in c_in]
                                 if isinstance(c_in, list)
                                 else c_in
                                 for c_in in k.coeffs
                             ],
                         )
                     )
                     + (
                         "\n\t\t"
-                        + " " * len(
-                            f"{k.atom_1} {k.atom_2} {k.atom_3} {k.atom_4}: "
-                        )
+                        + " " * len(f"{k.atom_1} {k.atom_2} {k.atom_3} {k.atom_4}: ")
                     )
                     + f"dih_type = {k.dih_type}\n"
                 )
                 for k in self.dihedrals
             ]
         )
         chi_str = "\tchi:\n" + "".join(
             [
                 (f"\t\t{k.atom_1} {k.atom_2}: " + f"{k.interaction_energy}\n")
                 for k in self.chi
             ]
         )
+
+        """ If dielectric wanted as dictionary
+            dielectric_type_str = "\tdielectric_type:\n" + "".join(
+                    [
+                        (f"\t\t{k.atom_1}: " + f"{k.dielectric_value}\n")
+                        for k in self.dielectric_type
+                    ]
+                )
+
+        """
+
         thermostat_coupling_groups_str = ""
         if any(self.thermostat_coupling_groups):
             thermostat_coupling_groups_str = (
                 "\tthermostat_coupling_groups:\n"
                 + "".join(
                     [
                         "\t\t" + ", ".join([f"{n}" for n in ng]) + "\n"
@@ -253,36 +289,37 @@
                     ]
                 )
             )
 
         ret_str = f'\n\n\tConfig: {self.file_name}\n\t{50 * "-"}\n'
         for k, v in self.__dict__.items():
             if k not in (
+                "target_pressure",
                 "bonds",
                 "angle_bonds",
                 "dihedrals",
                 "chi",
                 "thermostat_coupling_groups",
             ):
                 ret_str += f"\t{k}: {v}\n"
         ret_str += (
-            bonds_str
+            target_pressure_str
+            + bonds_str
             + angle_str
             + dihedrals_str
             + chi_str
             + thermostat_coupling_groups_str
         )
         return ret_str
 
 
 def read_config_toml(file_path):
     with open(file_path, "r") as in_file:
-        toml_content = in_file.read()
-    return toml_content
-
+        file_content = in_file.read()
+    return file_content
 
 def propensity_potential_coeffs(x: float, comm):
     alpha_coeffs = np.array(
         [
             [7.406, -5.298, -2.570, 1.336, 0.739],
             [-0.28632126, 1.2099146, 1.18122138, 0.49075168, 0.98495911],
         ]
@@ -325,44 +362,71 @@
             return np.concatenate((alpha_coeffs, coil_coeffs))
         else:
             beta_coeffs[0] *= 0.5 * (abs_x + x)
             return np.concatenate((beta_coeffs, coil_coeffs))
 
 
 def parse_config_toml(toml_content, file_path=None, comm=MPI.COMM_WORLD):
-    parsed_toml = tomli.loads(toml_content)
     config_dict = {}
 
+    # read toml to a dictionary
+    toml_content = tomli.loads(toml_content)
+
     # Defaults = None
     for n in (
+        "box_size",
         "n_print",
         "tau",
         "start_temperature",
         "target_temperature",
         "mass",
         "hamiltonian",
         "domain_decomposition",
         "integrator",
         "name",
         "n_particles",
         "max_molecule_size",
         "coulombtype",
+        "convergence_type",
         "dielectric_const",
+        "pol_mixing",
+        "conv_crit",
+        "dielectric_type",
+        "n_b",
+        "box_size",
         "n_flush",
+        "self_energy",
+        "dtype",
     ):
         config_dict[n] = None
 
     # Defaults = []
-    for n in ("bonds", "angle_bonds", "dihedrals", "chi", "tags"):
+
+    for n in (
+        "bonds",
+        "angle_bonds",
+        "dihedrals",
+        "chi",
+        "tags",
+        "m",
+        "dielectric_type",
+        "target_pressure",
+        "type_charges",
+    ):
         config_dict[n] = []
 
+    # Defaults: bool
+    config_dict["pressure"] = False
+
     # Flatten the .toml dictionary, ignoring the top level [tag] directives (if
     # any).
-    for k, v in parsed_toml.items():
+    for k, v in toml_content.items():
         if isinstance(v, dict):
+            if k == "nn": # Don't parse diff-hymd optimization options
+                continue
             for nested_k, nested_v in v.items():
                 config_dict[nested_k] = nested_v
         else:
             config_dict[k] = v
     for k, v in config_dict.items():
         if k == "bonds":
             config_dict["bonds"] = [None] * len(v)
@@ -386,27 +450,22 @@
         if k == "dihedrals":
             config_dict["dihedrals"] = [None] * len(v)
             for i, b in enumerate(v):
                 try:
                     dih_type = int(b[2][0])
                 except IndexError:
                     Logger.rank0.log(
-                        logging.WARNING,
-                        "Dihedral type not provided, defaulting to 0."
+                        logging.WARNING, "Dihedral type not provided, defaulting to 0."
                     )
                     dih_type = 0
 
                     # Probably it's better to move this in check_dihedrals?
                     wrong_len = len(b[1]) not in (1, 2)
-                    wrong_type_1 = len(b[1]) == 1 and not isinstance(
-                        b[1][0], float
-                    )
-                    wrong_type_2 = len(b[1]) == 2 and not isinstance(
-                        b[1][0], list
-                    )
+                    wrong_type_1 = len(b[1]) == 1 and not isinstance(b[1][0], float)
+                    wrong_type_2 = len(b[1]) == 2 and not isinstance(b[1][0], list)
                     if wrong_len or wrong_type_1 or wrong_type_2:
                         err_str = (
                             "The coefficients specified for the dihedral type "
                             "(0) do not match the correct structure. Either "
                             "use [lambda] or [[cn_prop], [dn_prop]], or select"
                             " the correct dihedral type."
                         )
@@ -421,42 +480,57 @@
                     coeff = np.array(
                         propensity_potential_coeffs(b[1][0][0], comm).tolist()
                         + b[1][1:]
                     )
                 elif dih_type == 2:
                     coeff = np.array(b[1])
                 else:
-                    coeff = np.insert(
-                        np.array(b[1]), 2, np.zeros((2, 5)), axis=0
-                    )
+                    coeff = np.insert(np.array(b[1]), 2, np.zeros((2, 5)), axis=0)
 
                 config_dict["dihedrals"][i] = Dihedral(
                     atom_1=b[0][0],
                     atom_2=b[0][1],
                     atom_3=b[0][2],
                     atom_4=b[0][3],
                     coeffs=coeff,
                     dih_type=dih_type,
                 )
-        # if k == "improper dihedrals":
-        #     config_dict["improper dihedrals"] = [None] * len(v)
-        # ...
         if k == "chi":
             config_dict["chi"] = [None] * len(v)
             for i, c in enumerate(v):
                 c_ = sorted([c[0], c[1]])
                 config_dict["chi"][i] = Chi(
                     atom_1=c_[0], atom_2=c_[1], interaction_energy=c[2]
                 )
 
+        """
+        if k == "dielectric_type":
+            config_dict["dielectric_type"] = [None] * len(v)
+            for i, c in enumerate(v):
+                c_ = sorted([c[0][0]])
+                config_dict["dielectric_type"][i] = Dielectric_type(
+                    atom_1=c_[0], dielectric_value=c[1][0]
+                )
+        """
+        if k == "target_pressure":
+            if len(v) == 2:
+                config_dict["target_pressure"] = Target_pressure(
+                    P_L=v[0],
+                    P_N=v[1],  # check condition # V array (still read as array?)
+                )
+            elif len(v) == 1:
+                config_dict["target_pressure"] = Target_pressure(P_L=v[0], P_N=None)
+            else:
+                config_dict["target_pressure"] = Target_pressure(P_L=None, P_N=None)
+
     if file_path is not None:
         config_dict["file_name"] = file_path
 
     for n in (
-        "n_steps", "time_step", "box_size", "mesh_size", "sigma", "kappa"
+        "n_steps", "time_step", "mesh_size", "sigma", "kappa"
     ):
         if n not in config_dict:
             err_str = (
                 f"No {n} specified in config file {file_path}. Unable to start"
                 f" simulation."
             )
             Logger.rank0.log(logging.ERROR, err_str)
@@ -635,17 +709,15 @@
                 d.atom_1 not in unique_names,
                 d.atom_2 not in unique_names,
                 d.atom_3 not in unique_names,
                 d.atom_4 not in unique_names,
             ]
             missing_names = [
                 atom
-                for i, atom in enumerate(
-                    [d.atom_1, d.atom_2, d.atom_3, d.atom_4]
-                )
+                for i, atom in enumerate([d.atom_1, d.atom_2, d.atom_3, d.atom_4])
                 if missing[i]
             ]
             missing_str = ", ".join(np.unique(missing_names))
 
             warn_str = (
                 f"Dihedral type {d.atom_1}--{d.atom_2}--{d.atom_3}--{d.atom_4}"
                 f" specified in {config.file_name} but no {missing_str} atoms "
@@ -682,48 +754,65 @@
                 f"specified system (names array)"
             )
             Logger.rank0.log(logging.WARNING, warn_str)
             if comm.Get_rank() == 0:
                 warnings.warn(warn_str)
 
     for i, n in enumerate(unique_names):
-        for m in unique_names[i+1:]:
+        for m in unique_names[i + 1 :]:
             found = False
             for c in config.chi:
                 if (c.atom_1 == n and c.atom_2 == m) or (
                     c.atom_1 == m and c.atom_2 == n
                 ):
                     found = True
             if not found:
-                config.chi.append(
-                    Chi(atom_1=n, atom_2=m, interaction_energy=0.0)
-                )
+                config.chi.append(Chi(atom_1=n, atom_2=m, interaction_energy=0.0))
                 warn_str = (
                     f"Atom types {n} and {m} found in the "
                     f"system, but no chi interaction {n}--{m} "
                     f"specified in {config.file_name}. Defaulting to "
                     f"chi[{n}, {m}] = 0"
                 )
                 Logger.rank0.log(logging.WARNING, warn_str)
                 if comm.Get_rank() == 0:
                     warnings.warn(warn_str)
     return config
 
 
-def check_box_size(config, comm=MPI.COMM_WORLD):
+def check_box_size(config, input_box, comm=MPI.COMM_WORLD):
+    if config.box_size is not None:
+        config.box_size = np.array(config.box_size, dtype=np.float32)
+        if input_box.all() and not np.allclose(config.box_size, input_box, atol=0.009):
+            err_str = (
+                f"Box size specified in {config.file_name}: "
+                f"{config.box_size} does not match input box:"
+                f"{input_box}"
+            )
+            Logger.rank0.log(logging.ERROR, err_str)
+            if comm.Get_rank() == 0:
+                raise ValueError(err_str)
+    else:
+        if input_box.all():
+            config.box_size = input_box
+        else:
+            err_str = f"No box information found"
+            Logger.rank0.log(logging.ERROR, err_str)
+            if comm.Get_rank() == 0:
+                raise ValueError(err_str)
+
     for b in config.box_size:
         if b <= 0.0:
             err_str = (
                 f"Invalid box size specified in {config.file_name}: "
                 f"{config.box_size}"
             )
             Logger.rank0.log(logging.ERROR, err_str)
             if comm.Get_rank() == 0:
                 raise ValueError(err_str)
-    config.box_size = np.array(config.box_size, dtype=np.float64)
     return config
 
 
 def check_integrator(config, comm=MPI.COMM_WORLD):
     if config.integrator.lower() not in ("velocity-verlet", "respa"):
         err_str = (
             f"Invalid integrator specified in {config.file_name}: "
@@ -759,18 +848,15 @@
                 f"Invalid number of inner rRESPA time steps in "
                 f"{config.file_name}: {config.respa_inner}. Must be "
                 f"positive integer"
             )
             Logger.rank0.log(logging.ERROR, err_str)
             raise ValueError(err_str)
 
-    if (
-        config.integrator.lower() == "velocity-verlet"
-        and config.respa_inner != 1
-    ):
+    if config.integrator.lower() == "velocity-verlet" and config.respa_inner != 1:
         warn_str = (
             f"Integrator type Velocity-Verlet specified in {config.file_name} "
             f"and inner rRESPA time steps set to {config.respa_inner}. "
             f"Using respa_inner = 1"
         )
         Logger.rank0.log(logging.WARNING, warn_str)
         if comm.Get_rank() == 0:
@@ -818,40 +904,38 @@
     if config.n_print:
         if config.n_flush is None:
             config.n_flush = 10000 // config.n_print
     return config
 
 
 def check_n_print(config, comm=MPI.COMM_WORLD):
-    if (not isinstance(config.n_print, int) and
-        not isinstance(config.n_print, float) and
-        config.n_print is not None):
-        err_str = (
-            f"invalid value for n_print ({config.n_print})"
-        )
+    if (
+        not isinstance(config.n_print, int)
+        and not isinstance(config.n_print, float)
+        and config.n_print is not None
+    ):
+        err_str = f"invalid value for n_print ({config.n_print})"
         Logger.rank0.log(logging.ERROR, err_str)
-        raise RuntimeError(err_str)        
-    
+        raise RuntimeError(err_str)
+
     if config.n_print is None or config.n_print <= 0:
         config.n_print = False
     elif not isinstance(config.n_print, int):
         if isinstance(config.n_print, float):
             warn_str = (
                 f"n_print is a float ({config.n_print}), not int, using "
                 f"{int(round(config.n_print))}"
             )
             Logger.rank0.log(logging.WARNING, warn_str)
             if comm.Get_rank() == 0:
                 warnings.warn(warn_str)
 
             config.n_print = int(round(config.n_print))
         else:
-            err_str = (
-                f"invalid value for n_print ({config.n_print})"
-            )
+            err_str = f"invalid value for n_print ({config.n_print})"
             Logger.rank0.log(logging.ERROR, err_str)
             raise RuntimeError(err_str)
     return config
 
 
 def check_tau(config, comm=MPI.COMM_WORLD):
     if config.tau is None and config.target_temperature is not None:
@@ -913,16 +997,15 @@
 def check_mass(config, comm=MPI.COMM_WORLD):
     if config.mass is None:
         info_str = "no mass specified, defaulting to 72.0"
         config.mass = 72.0
         Logger.rank0.log(logging.INFO, info_str)
     elif not isinstance(config.mass, int) and not isinstance(config.mass, float):
         err_str = (
-            f"specified mass is invalid type {config.mass}, "
-            f"({type(config.mass)})"
+            f"specified mass is invalid type {config.mass}, " f"({type(config.mass)})"
         )
         Logger.rank0.log(logging.ERROR, err_str)
         raise TypeError(err_str)
     elif config.mass < 0:
         err_str = f"invalid mass specified, {config.mass}"
         Logger.rank0.log(logging.ERROR, err_str)
         raise ValueError(err_str)
@@ -955,38 +1038,116 @@
                 f"an integer, using {int(round(dd))}"
             )
             config.domain_decomposition = int(round(dd))
         Logger.rank0.log(logging.WARNING, warn_str)
         if comm.Get_rank() == 0:
             warnings.warn(warn_str)
     else:
-        err_str = (f"invalid value for domain_decomposition "
-                   f"({config.domain_decomposition}) use an integer")
+        err_str = (
+            f"invalid value for domain_decomposition "
+            f"({config.domain_decomposition}) use an integer"
+        )
         Logger.rank0.log(logging.ERROR, err_str)
         raise ValueError(err_str)
 
     return config
 
 
 def check_name(config, comm=MPI.COMM_WORLD):
     if config.name is None:
         root_current_time = ""
         if comm.Get_rank() == 0:
-            root_current_time = datetime.datetime.now().strftime(
-                "%m/%d/%Y, %H:%M:%S"
-            )
+            root_current_time = datetime.datetime.now().strftime("%m/%d/%Y, %H:%M:%S")
         current_time = comm.bcast(root_current_time, root=0)
 
         if config.name is None:
             config.name = "sim" + current_time
     else:
         config.name = str(config.name)
     return config
 
 
+def check_NPT_conditions(config, comm=MPI.COMM_WORLD):
+    """
+    Check validity of barostat_type, barostat,
+    a, rho0, target_pressure, tau_p
+    """
+    if config.barostat is None:
+        if (
+            config.tau_p is not None
+            or (config.target_pressure.P_L and config.target_pressure.P_N) is not None
+        ):
+            err_str = (
+                "barostat not specified but config.tau_p "
+                "or config.target_pressure specified, cannot start simulation {config.barostat}"
+            )
+            Logger.rank0.log(logging.ERROR, err_str)
+            if comm.Get_rank() == 0:
+                raise TypeError(err_str)
+        if config.a:
+            warn_str = "a specified but no barostat," "setting a to average density"
+            Logger.rank0.log(logging.WARNING, warn_str)
+            if comm.Get_rank() == 0:
+                warnings.warn(warn_str)
+        if config.rho0:
+            warn_str = (
+                "rho0 specified but no barostat," "setting rho0 to average density"
+            )
+            Logger.rank0.log(logging.WARNING, warn_str)
+            if comm.Get_rank() == 0:
+                warnings.warn(warn_str)
+
+    if config.barostat is not None:
+        if not config.barostat_type:
+            config.barostat_type = "berendsen"
+            warn_str = "barostat_type not specified," "setting to berendsen"
+            Logger.rank0.log(logging.WARNING, warn_str)
+            if comm.Get_rank() == 0:
+                warnings.warn(warn_str)
+        if config.barostat != "isotropic" and config.barostat != "semiisotropic":
+            err_str = "barostat option not recognised. Valid options: isotropic, semiisotropic"
+            Logger.rank0.log(logging.ERROR, err_str)
+            if comm.Get_rank() == 0:
+                raise TypeError(err_str)
+        if config.target_pressure.P_L is None:
+            config.target_pressure.P_L = 1.0  # bar
+            config.target_pressure.P_N = None
+            if config.barostat == "semiisotropic":
+                config.target_pressure.P_N = 1.0  # bar
+            warn_str = (
+                "barostat specified but no target_pressure, defaulting to 1.0 bar"
+            )
+            Logger.rank0.log(logging.WARNING, warn_str)
+            if comm.Get_rank() == 0:
+                warnings.warn(warn_str)
+        if config.tau_p is None:
+            if config.tau <= 0.1:
+                config.tau_p = config.tau * 10.0
+            else:
+                config.tau_p = 1.0
+            warn_str = "barostat specified but no tau_p, defaulting to " + str(
+                config.tau_p
+            )
+            Logger.rank0.log(logging.WARNING, warn_str)
+            if comm.Get_rank() == 0:
+                warnings.warn(warn_str)
+        if not config.a:
+            err_str = "a not specified; cannot start simulation {config.a}"
+            Logger.rank0.log(logging.ERROR, err_str)
+            if comm.Get_rank() == 0:
+                raise TypeError(err_str)
+        if not config.rho0:
+            warn_str = "rho0 not specified;" "setting rho0 to average density"
+            Logger.rank0.log(logging.WARNING, warn_str)
+            if comm.Get_rank() == 0:
+                warnings.warn(warn_str)
+
+    return config
+
+
 def check_thermostat_coupling_groups(config, comm=MPI.COMM_WORLD):
     if any(config.thermostat_coupling_groups):
         found = [0 for _ in config.unique_names]
         unique_names = [n for n in config.unique_names]
         for i, group in enumerate(config.thermostat_coupling_groups):
             for species in group:
                 try:
@@ -1018,87 +1179,220 @@
                         f"thermostat coupling group, but {species} particles "
                         "were found in the system"
                     )
                     raise ValueError(err_str)
     return config
 
 
+def check_m(config, comm=MPI.COMM_WORLD):
+    if config.m == []:
+        config.m = [1.0 for t in range(config.n_types)]
+    return config
+
+
+def check_n_b(config, comm=MPI.COMM_WORLD):
+    if config.n_b is None:
+        warn_str = f"config.n_b not specified." "Defaulting to 1"
+        config.n_b = 1
+        Logger.rank0.log(logging.WARNING, warn_str)
+        if comm.Get_rank() == 0:
+            warnings.warn(warn_str)
+    return config
+
+
 def check_cancel_com_momentum(config, comm=MPI.COMM_WORLD):
     if isinstance(config.cancel_com_momentum, int):
         if config.cancel_com_momentum == 0 or config.cancel_com_momentum < 0:
             config.cancel_com_momentum = False
     elif not isinstance(config.cancel_com_momentum, bool):
         err_str = (
             f"Could not interpret {config.cancel_com_momentum} as an integer "
             f"or boolean."
         )
         raise ValueError(err_str)
     return config
 
 
-def check_config(config, indices, names, types, comm=MPI.COMM_WORLD):
+def sort_dielectric_by_type_id(config, charges, types):
+    """
+    Creates a list of length N CG-particles, sorted after the charges from
+    the input HDF5 file. Used in file_io.py
+    """
+    dielectric_val = np.zeros(config.n_types)
+    for j in range(config.n_types):
+        name = config.dielectric_type[j][0][0]
+        type_id = config.name_to_type_map[name]
+        dielectric_val[type_id] = config.dielectric_type[j][1][0]
+    config.dielectric_type = dielectric_val.copy()
+
+    N = len(charges)
+    len_list = np.zeros(config.n_types)
+    dielectric_by_types = np.zeros(N)
+    for i in range(N):
+        dielectric_by_types[i] = dielectric_val[types[i]]
+    # print("types ", types)
+    # print("diel  val", dielectric_by_types)
+    # print("charges", charges)
+    # print(config.name_to_type_map)
+    return dielectric_by_types  # by types with each particle id
+
+
+def check_charges_types_list(config, types, charges, comm=MPI.COMM_WORLD):
+    """
+    Creates a list of charge values of length types.
+    Charges are sorted according to type ID. Used in field.py.
+    # TODO: this is messy, we should fix it
+    """
+    if charges is None:
+        config.type_charges = [0.0] * config.n_types
+        return config
+
+    check_val = -100.0  # some random value that will never be encountered
+    charges_list = np.full(config.n_types, check_val)  # gatherv cant handle None
+    rank = comm.Get_rank()
+    # print(charges_list)
+    for t_ in range(config.n_types):
+        if t_ in types:
+            charges_list[t_] = charges[types == t_][0]
+
+    nprocs = int(comm.Get_size())
+    recv_charges = None
+    if rank == 0:
+        recv_charges = np.full(
+            config.n_types * nprocs, check_val
+        )  # gatherv cant handle None
+    comm.Gather(charges_list, recv_charges, root=0)
+
+    ## make a charges list
+    if rank == 0:
+        config_charges = np.zeros(config.n_types)
+        test_config = np.full(config.n_types, check_val)
+        for j in range(nprocs):
+            for i in range(config.n_types):
+                if recv_charges[i + j * config.n_types] != check_val:
+                    config_charges[i] = recv_charges[i + j * config.n_types]
+            if np.any([test_config, config_charges]):
+                continue
+            else:
+                break
+
+        # print(config_charges)
+        # print(config.name_to_type_map)
+        # print(charges[types == 0][0],charges[types == 1][0],charges[types == 2][0],charges[types == 3][0],
+        #        charges[types == 4][0])
+    else:
+        config_charges = np.zeros(config.n_types)
+
+    comm.Bcast(config_charges, root=0)
+    # print("config_charges", config_charges , "rank", rank)
+    # print(recv_charges)
+    # rank = comm.Get_rank()
+    # print(all_charges)
+    config.type_charges = config_charges
+    return config
+
+
+def check_dielectric(config, comm=MPI.COMM_WORLD):
+    """
+    Error handling for electrostatics.
+    Unit testing of toml/tomli input.
+    """
+    err_str_const = "Dielectric constant not given."
+    if config.coulombtype == "PIC_Spectral":
+        assert config.dielectric_const != None, err_str_const
+
+    err_str = "Dielectric list is empty."
+    if config.coulombtype == "PIC_Spectral_GPE":
+        assert len(config.dielectric_type) != 0, err_str
+        # default values
+        if config.pol_mixing is None:
+            config.pol_mixing = 0.6
+        if config.conv_crit is None:
+            config.conv_crit = 1e-6
+    return config
+
+
+def check_charges(config, charges, comm=MPI.COMM_WORLD):
+    """Check if charges across ranks sum to zero.
+
+    Parameters
+    ----------
+    charges : (N,) numpy.ndarray
+        Array of floats with charges for :code:`N` particles.
+    comm : mpi4py.Comm, optional
+        MPI communicator, defaults to :code:`mpi4py.COMM_WORLD`.
+    """
+    total_charge = comm.allreduce(np.sum(charges), MPI.SUM)
+
+    if not np.isclose(total_charge, 0.0):
+        warn_str = (
+            f"Charges in the input file do not sum to zero. "
+            f"Total charge is {total_charge}."
+        )
+        Logger.rank0.log(logging.WARNING, warn_str)
+        if comm.Get_rank() == 0:
+            warnings.warn(warn_str)
+
+    # if charges are ok, compute self energy
+    if config.coulombtype == "PIC_Spectral":
+        from .field import compute_self_energy_q
+
+        config.self_energy = compute_self_energy_q(config, charges, comm=comm)
+
+    return config
+
+
+def check_config(
+    config, indices, names, types, charges, input_box, comm=MPI.COMM_WORLD
+):
     """Performs various checks on the specfied config to ensure consistency
 
     Parameters
     ----------
     config : Config
         Configuration object.
     indices : (N,) numpy.ndarray
         Array of integer indices for :code:`N` particles.
     names : (N,) numpy.ndarray
         Array of string names for :code:`N` particles.
     types : (N,) numpy.ndarray
         Array of integer type indices for :code:`N` particles.
+    charges : (N,) numpy.ndarray
+        Array of floats charges for :code:`N` particles.
     comm : mpi4py.Comm, optional
         MPI communicator, defaults to :code:`mpi4py.COMM_WORLD`.
 
     Returns
     -------
     config : Config
         Validated configuration object.
     """
-    config.box_size = np.array(config.box_size)
     config = _find_unique_names(config, names, comm=comm)
     if types is not None:
         config = _setup_type_to_name_map(config, names, types, comm=comm)
-    config = check_box_size(config, comm=comm)
+    config = check_box_size(config, input_box, comm=comm)
     config = check_integrator(config, comm=comm)
     config = check_max_molecule_size(config, comm=comm)
     config = check_tau(config, comm=comm)
     config = check_start_and_target_temperature(config, comm=comm)
     config = check_mass(config, comm=comm)
     config = check_domain_decomposition(config, comm=comm)
     config = check_name(config, comm=comm)
     config = check_n_particles(config, indices, comm=comm)
     config = check_chi(config, names, comm=comm)
     config = check_bonds(config, names, comm=comm)
     config = check_angles(config, names, comm=comm)
     config = check_dihedrals(config, names, comm=comm)
     config = check_hamiltonian(config, comm=comm)
+    config = check_NPT_conditions(config, comm=comm)
+    config = check_n_b(config, comm=comm)
+    config = check_m(config, comm=comm)
     config = check_thermostat_coupling_groups(config, comm=comm)
     config = check_cancel_com_momentum(config, comm=comm)
+    config = check_dielectric(config, comm=comm)
     config = check_n_print(config, comm=comm)
     config = check_n_flush(config, comm=comm)
-    return config
-
-
-def check_charges(charges, comm=MPI.COMM_WORLD):
-    """Check if charges across ranks sum to zero.
-
-    Parameters
-    ----------
-    charges : (N,) numpy.ndarray
-        Array of floats with charges for :code:`N` particles.
-    comm : mpi4py.Comm, optional
-        MPI communicator, defaults to :code:`mpi4py.COMM_WORLD`.
-    """  
-    total_charge = comm.allreduce(np.sum(charges), MPI.SUM)
-
-    if not np.isclose(total_charge, 0.):
-        warn_str = (
-            f"Charges in the input file do not sum to zero. "
-            f"Total charge is {total_charge}."
-        )
-        Logger.rank0.log(logging.WARNING, warn_str)
-        if comm.Get_rank() == 0:
-            warnings.warn(warn_str)
+    config = check_charges_types_list(config, types, charges, comm=comm)
+    if charges is not None:
+        config = check_charges(config, charges, comm=comm)
 
+    return config
```

### Comparing `hymd-1.0.9/hymd/integrator.py` & `hymd-2.0.1/hymd/integrator.py`

 * *Files identical despite different names*

### Comparing `hymd-1.0.9/hymd/logger.py` & `hymd-2.0.1/hymd/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import os
 import logging
 from mpi4py import MPI
 from .version import __version__
 
 
 class MPIFilterRoot(logging.Filter):
-    """Log output Filter wrapper class for the root MPI rank log
-    """
+    """Log output Filter wrapper class for the root MPI rank log"""
+
     def filter(self, record):
         """Log event message filter
 
         Parameters
         ----------
         record : logging.LogRecord
             LogRecord object corresponding to the log event.
@@ -25,16 +25,16 @@
             record.size = MPI.COMM_WORLD.Get_size()
             return True
         else:
             return False
 
 
 class MPIFilterAll(logging.Filter):
-    """Log output Filter wrapper class for the all-MPI-ranks log
-    """
+    """Log output Filter wrapper class for the all-MPI-ranks log"""
+
     def filter(self, record):
         """Log event message filter
 
         Parameters
         ----------
         record : logging.LogRecord
             LogRecord object corresponding to the log event.
@@ -82,14 +82,15 @@
         loggers.
     rank0 : logging.Logger
         Default logger object for the root MPI rank.
     all_ranks : logging.Logger
         Default logger object for messages being emitted from all MPI ranks
         simultaneously.
     """
+
     level = None
     log_file = None
     format = " %(levelname)-8s [%(filename)s:%(lineno)d] <%(funcName)s> {rank %(rank)d/%(size)d} %(message)s"  # noqa: E501
     date_format = "%(asctime)s"
     formatter = logging.Formatter(fmt=date_format + format)
     rank0 = logging.getLogger("HyMD.rank_0")
     all_ranks = logging.getLogger("HyMD.all_ranks")
@@ -189,36 +190,37 @@
     / / / /_  __/ / /__  _________ _____ ______   /  |/  / __ \
    / /_/ / / / / / / _ \/ ___/ __ `/ __ `/ ___/  / /|_/ / / / /
   / __  / /_/ / / /  __/ /  / /_/ / /_/ (__  )  / /  / / /_/ / 
  /_/ /_/\__, /_/_/\___/_/   \__,_/\__,_/____/  /_/  /_/_____/  
        /____/ 
     """
 
-    refs = """
- [1] Milano, G.; Kawakatsu, T. Hybrid particle-field molecular dynamics 
- simulations for dense polymer systems. J. Chem. Phys. 2009, 130, 214106.
- 
- [2] Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid 
- particle–field molecular dynamics. J. Chem. Phys. 2020, 153, 094106.
+    refs_set1 = """
  
- [3] Kolli, H. B.; De Nicola, A.; Bore, S. L.; Schäfer, K.; Diezemann, G.;
- Gauss, J.; Kawakatsu, T.;Lu, Z.-Y.; Zhu, Y.-L.; Milano, G.; Cascella, M. 
- Hybrid Particle-Field Molecular DynamicsSimulations of Charged Amphiphiles 
- in an Aqueous Environment. J. Chem. Theory Comput. 2018, 14, 4928–4937.
- 
- [4] Bore, S. L.; Milano, G.; Cascella, M. Hybrid Particle-Field Model for
- Conformational Dynamics of Peptide Chains. J. Chem. Theory Comput. 2018,
- 14, 1120–1130.
+ [1] Ledum, M.; Sen, S.; Li, X.; Carrer, M.; Feng Y.; Cascella, M.; Bore, S. L. 
+ HylleraasMD: A Domain Decomposition-Based Hybrid Particle-Field Software for Multi-Scale Simulations of Soft Matter. ChemRxiv 2021
+
+ [2] Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L. 
+ HyMD: Massively parallel hybrid particle-field molecular dynamics in Python.
  
- [5] Periole, X.; Cavalli, M.; Marrink, S. J.; Ceruso, M. A. Combining an 
- elastic network with a coarse-grained molecular force field: structure, 
- dynamics, and intermolecular recognition. J. Chem. Theory Comput. 2009, 
- 5.9, 2531-2543.
+ [3] Bore, S. L.; Cascella, M. 
+ Hamiltonian and alias-free hybrid particle–field molecular dynamics. J. Chem. Phys. 2020, 153, 094106.
+
+ [4] Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM J. Sci. Comput. 2013, 35, C213–C236.
+"""
+    refs_set2 = """
+
+ [5] Sen, S.; Ledum, M.; Bore, S. L.; Cascella, M. 
+ Soft Matter under Pressure: Pushing Particle–Field Molecular Dynamics to the Isobaric Ensemble. ChemRxiv 2023
 """
 
     version = f"Version {get_version()}"
     header = banner
-    header += version.center(56)+"\n\n"
-    header += " Please read and cite accordingly the references below:"
-    header += refs
+    header += version.center(56) + "\n\n"
+    #header += " Please read and cite the references below:"
+    header += " PLEASE READ AND CITE THE REFERENCES BELOW:"
+    header += refs_set1
+    #header += " \n\n For constant pressure (NPT) simulations, please cite:"
+    header += " \n\n FOR CONSTANT PRESSURE (NPT) SIMULATIONS, PLEASE CITE:"
+    header += refs_set2
 
-    return header
+    return header
```

### Comparing `hymd-1.0.9/hymd/main.py` & `hymd-2.0.1/hymd/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,25 +6,35 @@
 import sys
 from mpi4py import MPI
 import numpy as np
 import pmesh.pm as pmesh
 import warnings
 from .configure_runtime import configure_runtime
 from .hamiltonian import get_hamiltonian
-from .input_parser import check_config, check_charges
+from .input_parser import check_config, sort_dielectric_by_type_id
 from .logger import Logger, format_timedelta
 from .file_io import distribute_input, OutDataset, store_static, store_data
-from .field import (compute_field_force, update_field,
-                    compute_field_and_kinetic_energy, domain_decomposition,
-                    update_field_force_q, compute_field_energy_q,
-                    compute_self_energy_q)
-from .thermostat import (csvr_thermostat, cancel_com_momentum,
-                         generate_initial_velocities)
+from .field import (
+    compute_field_force,
+    update_field,
+    compute_field_and_kinetic_energy,
+    domain_decomposition,
+    update_field_force_q,
+    update_field_force_q_GPE,
+    compute_field_energy_q_GPE,
+    initialize_pm,
+)
+from .thermostat import (
+    csvr_thermostat,
+    cancel_com_momentum,
+    generate_initial_velocities,
+)
 from .force import dipole_forces_redistribution, prepare_bonds
 from .integrator import integrate_velocity, integrate_position
+from .pressure import comp_pressure
 
 
 def main():
     """Main simulation driver
 
     Initializes structure, topology, and simulation configuration and iterates
     the molecular dynamics loop.
@@ -32,39 +42,32 @@
     comm = MPI.COMM_WORLD
     rank = comm.Get_rank()
     size = comm.Get_size()
 
     if rank == 0:
         start_time = datetime.datetime.now()
 
-    args, config, prng = configure_runtime(sys.argv[1:], comm)
+    args, config, prng, topol = configure_runtime(sys.argv[1:], comm)
 
     if args.double_precision:
         dtype = np.float64
+        config.dtype = dtype
+        from .force import compute_bond_forces__fortran__double as compute_bond_forces
+        from .force import compute_angle_forces__fortran__double as compute_angle_forces
         from .force import (
-            compute_bond_forces__fortran__double as compute_bond_forces
-        )
-        from .force import (
-            compute_angle_forces__fortran__double as compute_angle_forces
-        )
-        from .force import (
-            compute_dihedral_forces__fortran__double as compute_dihedral_forces
+            compute_dihedral_forces__fortran__double as compute_dihedral_forces,
         )
     else:
         dtype = np.float32
-        from .force import (
-            compute_bond_forces__fortran as compute_bond_forces
-        )
-        from .force import (
-            compute_angle_forces__fortran as compute_angle_forces
-        )
-        from .force import (
-            compute_dihedral_forces__fortran as compute_dihedral_forces
-        )
+        config.dtype = dtype
+        from .force import compute_bond_forces__fortran as compute_bond_forces
+        from .force import compute_angle_forces__fortran as compute_angle_forces
+        from .force import compute_dihedral_forces__fortran as compute_dihedral_forces
 
+    # read input .hdf5
     driver = "mpio" if not args.disable_mpio else None
     _kwargs = {"driver": driver, "comm": comm} if not args.disable_mpio else {}
     with h5py.File(args.input, "r", **_kwargs) as in_file:
         rank_range, molecules_flag = distribute_input(
             in_file,
             rank,
             size,
@@ -79,38 +82,99 @@
             velocities = in_file["velocities"][-1, rank_range, :]
             velocities = velocities.astype(dtype)
         else:
             velocities = np.zeros_like(positions, dtype=dtype)
 
         names = in_file["names"][rank_range]
 
+        if "box" in in_file.attrs:
+            config.box_size = np.array(in_file.attrs["box"])
+        else:
+            if getattr(config, "box_size") is None:
+                err_str = (
+                    f"No box size present in either config or input file. Unable to start"
+                    f" simulation."
+                )
+                Logger.rank0.log(logging.ERROR, err_str)
+                if comm.Get_rank() == 0:
+                    raise ValueError(err_str)
+
         types = None
         bonds = None
+        charges = None
         molecules = []
         if "types" in in_file:
             types = in_file["types"][rank_range]
         if molecules_flag:
             molecules = in_file["molecules"][rank_range]
-            bonds = in_file["bonds"][rank_range]
+            if topol is None:
+                bonds = in_file["bonds"][rank_range]
         if "charge" in in_file:
             charges = in_file["charge"][rank_range]
             charges_flag = True
         else:
             charges_flag = False
 
-    if charges_flag:
-        check_charges(charges, comm=comm)
+        if "box" in in_file:
+            input_box = in_file["box"][:]
+        else:
+            input_box = np.array([None, None, None])
+
+    # finishes config setup and checks
+    config = check_config(config, indices, names, types, charges, input_box, comm=comm)
+
+    # import barostat if necessary
+    if config.barostat_type == "berendsen":
+        from .barostat import isotropic, semiisotropic
+    elif config.barostat_type == "scr":
+        from .barostat_scr import isotropic, semiisotropic
+
+    # dielectric from toml
+    if config.coulombtype == "PIC_Spectral_GPE":
+        dielectric_sorted = sort_dielectric_by_type_id(config, charges, types)
+        dielectric_flag = True
+
+        if config.convergence_type is not None:
+            if config.convergence_type == "csum":
+
+                def conv_fun(comm, diff_mesh):
+                    return diff_mesh.csum()  # check if allreduce needed
+
+            elif config.convergence_type == "euclidean_norm":
 
-    config = check_config(config, indices, names, types, comm=comm)
+                def conv_fun(comm, diff_mesh):
+                    return diff_mesh.cnorm()  # check if allreduce nedded
+
+            elif config.convergence_type == "max_diff":
+
+                def conv_fun(comm, diffmesh):
+                    msg = np.max(diffmesh)
+                    res = comm.allreduce(sendobj=msg, op=MPI.MAX)
+                    return res
+
+        else:  # default choice is the max difference if not specified
+            config.convergence_type = "max_diff"
+
+            def conv_fun(comm, diffmesh):
+                msg = np.max(diffmesh)
+                res = comm.allreduce(sendobj=msg, op=MPI.MAX)
+                return res
+
+    else:
+        dielectric_flag = False
 
     if config.start_temperature:
         velocities = generate_initial_velocities(velocities, config, prng, comm=comm)
     elif config.cancel_com_momentum:
         velocities = cancel_com_momentum(velocities, config, comm=comm)
 
+    # set all PRNG to the root's PRNG
+    # this is done to avoid communication between ranks in the thermostat
+    prng = comm.bcast(prng, root=0)
+
     bond_forces = np.zeros_like(positions)
     angle_forces = np.zeros_like(positions)
     dihedral_forces = np.zeros_like(positions)
     reconstructed_forces = np.zeros_like(positions)
     field_forces = np.zeros_like(positions)
     elec_forces = np.zeros_like(positions)
 
@@ -130,61 +194,59 @@
     # Initialize energies
     field_energy = 0.0
     bond_energy = 0.0
     angle_energy = 0.0
     dihedral_energy = 0.0
     kinetic_energy = 0.0
     field_q_energy = 0.0
-    field_q_self_energy = 0.0
 
-    # Ignore numpy numpy.VisibleDeprecationWarning: Creating an ndarray from
-    # ragged nested sequences until it is fixed in pmesh
-    with warnings.catch_warnings():
-        warnings.filterwarnings(
-            action="ignore",
-            category=np.VisibleDeprecationWarning,
-            message=r"Creating an ndarray from ragged nested sequences",
-        )
-        pm = pmesh.ParticleMesh(
-            config.mesh_size, BoxSize=config.box_size,
-            dtype="f4" if dtype == np.float32 else np.float64, comm=comm
-        )
+    # more initialization
+    bond_pr_ = np.zeros(3, dtype=dtype)
+    angle_pr_ = np.zeros(3, dtype=dtype)
 
     hamiltonian = get_hamiltonian(config)
 
-    Logger.rank0.log(logging.INFO, f"pfft-python processor mesh: {str(pm.np)}")
-
-    # Initialize density fields
-    phi = [pm.create("real", value=0.0) for _ in range(config.n_types)]
-    phi_fourier = [
-        pm.create("complex", value=0.0) for _ in range(config.n_types)
-    ]  # noqa: E501
-    force_on_grid = [
-        [pm.create("real", value=0.0) for _ in range(3)] for _ in range(config.n_types)  # noqa: E501
-    ]
-    v_ext_fourier = [pm.create("complex", value=0.0) for _ in range(4)]
-    v_ext = [pm.create("real", value=0.0) for _ in range(config.n_types)]
+    pm_objs = initialize_pm(pmesh, config, comm)
+    pm, field_list, elec_common_list, coulomb_list = pm_objs
+    (
+        phi,
+        phi_fourier,
+        force_on_grid,
+        v_ext_fourier,
+        v_ext,
+        phi_transfer,
+        phi_laplacian,
+    ) = field_list
+
+    # when electrostatics is not used, these objs are None
+    phi_q, phi_q_fourier, psi, elec_field = elec_common_list
+
+    if len(coulomb_list) == 2:
+        (
+            elec_field_fourier,
+            psi_fourier,
+        ) = coulomb_list
+
+    elif len(coulomb_list) == 12:
+        [
+            phi_eps,
+            phi_eps_fourier,
+            phi_eta,
+            phi_eta_fourier,
+            phi_pol,
+            phi_pol_prev,
+            elec_dot,
+            elec_field_contrib,
+            Vbar_elec,
+            Vbar_elec_fourier,
+            force_mesh_elec,
+            force_mesh_elec_fourier,
+        ] = coulomb_list
 
-    # Initialize charge density fields
-    _SPACE_DIM = 3
-    if charges_flag and config.coulombtype == "PIC_Spectral":
-        phi_q = pm.create("real", value=0.0)
-        phi_q_fourier = pm.create("complex", value=0.0)
-        elec_field_fourier = [
-            pm.create("complex", value=0.0) for _ in range(_SPACE_DIM)
-        ]  # for force calculation
-        elec_field = [
-            pm.create("real", value=0.0) for _ in range(_SPACE_DIM)
-        ]  # for force calculation
-        elec_potential = pm.create(
-            "real", value=0.0
-        )
-        elec_potential_fourier = pm.create(
-            "complex", value=0.0
-        )
+    Logger.rank0.log(logging.INFO, f"pfft-python processor mesh: {str(pm.np)}")
 
     args_in = [
         velocities,
         indices,
         bond_forces,
         angle_forces,
         dihedral_forces,
@@ -193,39 +255,45 @@
         names,
         types,
     ]
 
     if charges_flag:
         args_in.append(charges)
         args_in.append(elec_forces)
+    if dielectric_flag:
+        args_in.append(dielectric_sorted)
 
     if config.domain_decomposition:
-        (positions,
-        velocities,
-        indices,
-        bond_forces,
-        angle_forces,
-        dihedral_forces,
-        reconstructed_forces,
-        field_forces,
-        names,
-        types,
-        *optional) = domain_decomposition(
+        (
+            positions,
+            velocities,
+            indices,
+            bond_forces,
+            angle_forces,
+            dihedral_forces,
+            reconstructed_forces,
+            field_forces,
+            names,
+            types,
+            *optional,
+        ) = domain_decomposition(
             positions,
             pm,
             *tuple(args_in),
             molecules=molecules if molecules_flag else None,
             bonds=bonds if molecules_flag else None,
             verbose=args.verbose,
             comm=comm,
         )
 
         if charges_flag:
             charges = optional.pop(0)
             elec_forces = optional.pop(0)
+        if dielectric_flag:
+            dielectric_sorted = optional.pop(0)
         if molecules_flag:
             bonds = optional.pop(0)
             molecules = optional.pop(0)
 
         # rebuild args_in to point to correct arrays
         args_in = [
             velocities,
@@ -238,74 +306,147 @@
             names,
             types,
         ]
 
         if charges_flag:
             args_in.append(charges)
             args_in.append(elec_forces)
+        if dielectric_flag:
+            args_in.append(dielectric_sorted)
 
     if not args.disable_field:
-        layouts = [pm.decompose(positions[types == t]) for t in range(config.n_types)]  # noqa: E501
+        layouts = [
+            pm.decompose(positions[types == t]) for t in range(config.n_types)
+        ]  # noqa: E501
         update_field(
-            phi, layouts, force_on_grid, hamiltonian, pm, positions, types,
-            config, v_ext, phi_fourier, v_ext_fourier, compute_potential=True,
-        )
-        field_energy, kinetic_energy = compute_field_and_kinetic_energy(
-            phi, velocities, hamiltonian, positions, types, v_ext, config,
-            layouts, comm=comm,
+            phi,
+            phi_laplacian,
+            phi_transfer,
+            layouts,
+            force_on_grid,
+            hamiltonian,
+            pm,
+            positions,
+            types,
+            config,
+            v_ext,
+            phi_fourier,
+            v_ext_fourier,
+            config.m,
+            compute_potential=True,
+        )
+        (
+            field_energy,
+            kinetic_energy,
+            field_q_energy,
+        ) = compute_field_and_kinetic_energy(
+            phi,
+            phi_q,
+            psi,
+            velocities,
+            hamiltonian,
+            positions,
+            types,
+            v_ext,
+            config,
+            layouts,
+            comm=comm,
         )
         compute_field_force(
-            layouts, positions, force_on_grid, field_forces, types,
-            config.n_types
+            layouts, positions, force_on_grid, field_forces, types, config.n_types
         )
     else:
-        kinetic_energy = comm.allreduce(
-            0.5 * config.mass * np.sum(velocities**2)
-        )
+        kinetic_energy = comm.allreduce(0.5 * config.mass * np.sum(velocities**2))
 
-    if charges_flag and config.coulombtype == "PIC_Spectral":
-        field_q_self_energy = compute_self_energy_q(config, charges, comm=comm)
+    if charges_flag:
         layout_q = pm.decompose(positions)
-        update_field_force_q(
-            charges, phi_q, phi_q_fourier, elec_field_fourier, elec_field,
-            elec_forces, layout_q, hamiltonian, pm, positions, config,
-        )
-
-        field_q_energy = compute_field_energy_q(
-            config, phi_q, phi_q_fourier, elec_potential, 
-            elec_potential_fourier, 
-            field_q_self_energy, comm=comm,
-        )
+        if config.coulombtype == "PIC_Spectral_GPE":  # dielectric_flag
+            Vbar_elec, phi_eps, elec_dot = update_field_force_q_GPE(
+                conv_fun,
+                phi,
+                types,
+                charges,
+                phi_q,
+                phi_q_fourier,
+                phi_eps,
+                phi_eps_fourier,
+                phi_eta,
+                phi_eta_fourier,
+                phi_pol_prev,
+                phi_pol,
+                elec_field,
+                elec_forces,
+                elec_field_contrib,
+                psi,
+                Vbar_elec,
+                Vbar_elec_fourier,
+                force_mesh_elec,
+                force_mesh_elec_fourier,
+                hamiltonian,
+                layout_q,
+                layouts,
+                pm,
+                positions,
+                config,
+                comm=comm,
+            )
 
-    if molecules_flag:
-        if not (args.disable_bonds
-                and args.disable_angle_bonds
-                and args.disable_dihedrals):
+            field_q_energy = compute_field_energy_q_GPE(
+                config, phi_eps, field_q_energy, elec_dot, comm=comm
+            )
 
-            bonds_prep = prepare_bonds(
-                molecules, names, bonds, indices, config
+        if config.coulombtype == "PIC_Spectral":
+            update_field_force_q(
+                charges,
+                phi_q,
+                phi_q_fourier,
+                psi,
+                psi_fourier,
+                elec_field_fourier,
+                elec_field,
+                elec_forces,
+                layout_q,
+                hamiltonian,
+                pm,
+                positions,
+                config,
             )
+
+    if molecules_flag:
+        if not (
+            args.disable_bonds and args.disable_angle_bonds and args.disable_dihedrals
+        ):
+            bonds_prep = prepare_bonds(molecules, names, bonds, indices, config, topol)
             (
                 # two-particle bonds
-                bonds_2_atom1, bonds_2_atom2, bonds_2_equilibrium,
+                bonds_2_atom1,
+                bonds_2_atom2,
+                bonds_2_equilibrium,
                 bonds_2_stength,
                 # three-particle bonds
-                bonds_3_atom1, bonds_3_atom2, bonds_3_atom3,
-                bonds_3_equilibrium, bonds_3_stength,
+                bonds_3_atom1,
+                bonds_3_atom2,
+                bonds_3_atom3,
+                bonds_3_equilibrium,
+                bonds_3_stength,
                 # four-particle bonds
-                bonds_4_atom1, bonds_4_atom2, bonds_4_atom3, bonds_4_atom4,
-                bonds_4_coeff, bonds_4_type, bonds_4_last,
+                bonds_4_atom1,
+                bonds_4_atom2,
+                bonds_4_atom3,
+                bonds_4_atom4,
+                bonds_4_coeff,
+                bonds_4_type,
+                bonds_4_last,
             ) = bonds_prep
 
             bonds_4_coeff = np.asfortranarray(bonds_4_coeff)
 
             if bonds_4_type.any() > 1:
                 err_str = (
-                    "0 and 1 are the only currently supported dihedral angle "
-                    "types."
+                    "0 and 1 are the only currently supported dihedral angle " "types."
                 )
                 Logger.rank0.log(logging.ERROR, err_str)
                 if rank == 0:
                     raise NotImplementedError(err_str)
 
             # Check if we have a protein
             protein_flag = comm.allreduce(bonds_4_type.any() == 1)
@@ -324,19 +465,20 @@
                         if bonds_4_type[i] == 1
                         else 2 * [0.0, 0.0]
                         for i in range(n_tors)
                     ],
                     dtype=dtype,
                 ).flatten()
                 dipole_forces = np.zeros_like(dipole_positions)
-                transfer_matrices = np.zeros(
-                    shape=(n_tors, 6, 3, 3), dtype=dtype
-                )
+                transfer_matrices = np.zeros(shape=(n_tors, 6, 3, 3), dtype=dtype)
                 phi_dipoles = pm.create("real", value=0.0)
                 phi_dipoles_fourier = pm.create("complex", value=0.0)
+                psi_dipoles = pm.create("real", value=0.0)
+                psi_dipoles_fourier = pm.create("complex", value=0.0)
+                _SPACE_DIM = 3
                 dipoles_field_fourier = [
                     pm.create("complex", value=0.0) for _ in range(_SPACE_DIM)
                 ]
                 dipoles_field = [
                     pm.create("real", value=0.0) for _ in range(_SPACE_DIM)
                 ]
 
@@ -345,107 +487,215 @@
         bond_forces = np.asfortranarray(bond_forces)
         angle_forces = np.asfortranarray(angle_forces)
         dihedral_forces = np.asfortranarray(dihedral_forces)
         dipole_positions = np.asfortranarray(dipole_positions)
         transfer_matrices = np.asfortranarray(transfer_matrices)
 
         if not args.disable_bonds:
-            bond_energy_ = compute_bond_forces(
-                bond_forces, positions, config.box_size, bonds_2_atom1,
-                bonds_2_atom2, bonds_2_equilibrium, bonds_2_stength,
+            bond_energy_, bond_pr_ = compute_bond_forces(
+                bond_forces,
+                positions,
+                config.box_size,
+                bonds_2_atom1,
+                bonds_2_atom2,
+                bonds_2_equilibrium,
+                bonds_2_stength,
             )
             bond_energy = comm.allreduce(bond_energy_, MPI.SUM)
         else:
             bonds_2_atom1, bonds_2_atom2 = [], []
         if not args.disable_angle_bonds:
-            angle_energy_ = compute_angle_forces(
-                angle_forces, positions, config.box_size, bonds_3_atom1,
-                bonds_3_atom2, bonds_3_atom3, bonds_3_equilibrium,
+            angle_energy_, angle_pr_ = compute_angle_forces(
+                angle_forces,
+                positions,
+                config.box_size,
+                bonds_3_atom1,
+                bonds_3_atom2,
+                bonds_3_atom3,
+                bonds_3_equilibrium,
                 bonds_3_stength,
             )
             angle_energy = comm.allreduce(angle_energy_, MPI.SUM)
+            # angle_pr = comm.allreduce(angle_pr_, MPI.SUM)
+
         if not args.disable_dihedrals:
             dihedral_energy_ = compute_dihedral_forces(
-                dihedral_forces, positions, dipole_positions,
-                transfer_matrices, config.box_size, bonds_4_atom1,
-                bonds_4_atom2, bonds_4_atom3, bonds_4_atom4, bonds_4_coeff,
-                bonds_4_type, bonds_4_last, dipole_flag,
+                dihedral_forces,
+                positions,
+                dipole_positions,
+                transfer_matrices,
+                config.box_size,
+                bonds_4_atom1,
+                bonds_4_atom2,
+                bonds_4_atom3,
+                bonds_4_atom4,
+                bonds_4_coeff,
+                bonds_4_type,
+                bonds_4_last,
+                dipole_flag,
             )
             dihedral_energy = comm.allreduce(dihedral_energy_, MPI.SUM)
 
         if protein_flag and not args.disable_dipole:
             dipole_positions = np.reshape(dipole_positions, (4 * n_tors, 3))
             dipole_forces = np.reshape(dipole_forces, (4 * n_tors, 3))
 
             layout_dipoles = pm.decompose(dipole_positions)
             update_field_force_q(
-                dipole_charges, phi_dipoles, phi_dipoles_fourier,
-                dipoles_field_fourier, dipoles_field, dipole_forces,
-                layout_dipoles, hamiltonian, pm, dipole_positions, config,
+                dipole_charges,
+                phi_dipoles,
+                phi_dipoles_fourier,
+                psi_dipoles,
+                psi_dipoles_fourier,
+                dipoles_field_fourier,
+                dipoles_field,
+                dipole_forces,
+                layout_dipoles,
+                hamiltonian,
+                pm,
+                dipole_positions,
+                config,
             )
 
             dipole_positions = np.reshape(dipole_positions, (n_tors, 4, 3))
             dipole_forces = np.reshape(dipole_forces, (n_tors, 4, 3))
 
             dipole_positions = np.asfortranarray(dipole_positions)
             dipole_forces_redistribution(
-                reconstructed_forces, dipole_forces, transfer_matrices,
-                bonds_4_atom1, bonds_4_atom2, bonds_4_atom3, bonds_4_atom4,
-                bonds_4_type, bonds_4_last,
+                reconstructed_forces,
+                dipole_forces,
+                transfer_matrices,
+                bonds_4_atom1,
+                bonds_4_atom2,
+                bonds_4_atom3,
+                bonds_4_atom4,
+                bonds_4_type,
+                bonds_4_last,
             )
 
     else:
         bonds_2_atom1, bonds_2_atom2 = [], []
 
     config.initial_energy = (
-        field_energy + kinetic_energy + bond_energy + angle_energy
-        + dihedral_energy + field_q_energy
+        field_energy
+        + kinetic_energy
+        + bond_energy
+        + angle_energy
+        + dihedral_energy
+        + field_q_energy
     )
 
     out_dataset = OutDataset(
-        args.destdir, config, double_out=args.double_output,
+        args.destdir,
+        config,
+        double_out=args.double_output,
         disable_mpio=args.disable_mpio,
     )
 
     store_static(
-        out_dataset, rank_range, names, types, indices, config, bonds_2_atom1,
-        bonds_2_atom2, molecules=molecules if molecules_flag else None,
-        velocity_out=args.velocity_output, force_out=args.force_output,
-        charges=charges if charges_flag else False, comm=comm,
+        out_dataset,
+        rank_range,
+        names,
+        types,
+        indices,
+        config,
+        bonds_2_atom1,
+        bonds_2_atom2,
+        molecules=molecules if molecules_flag else None,
+        velocity_out=args.velocity_output,
+        force_out=args.force_output,
+        charges=charges if charges_flag else False,
+        dielectrics=dielectric_sorted if dielectric_flag else False,
+        comm=comm,
     )
 
     if config.n_print > 0:
         step = 0
         frame = 0
         if not args.disable_field:
-            field_energy, kinetic_energy = compute_field_and_kinetic_energy(
-                phi, velocities, hamiltonian, positions, types, v_ext, config,
-                layouts, comm=comm,
+            (
+                field_energy,
+                kinetic_energy,
+                field_q_energy,
+            ) = compute_field_and_kinetic_energy(
+                phi,
+                phi_q,
+                psi,
+                velocities,
+                hamiltonian,
+                positions,
+                types,
+                v_ext,
+                config,
+                layouts,
+                comm=comm,
             )
         else:
-            kinetic_energy = comm.allreduce(
-                0.5 * config.mass * np.sum(velocities ** 2)
-            )
+            kinetic_energy = comm.allreduce(0.5 * config.mass * np.sum(velocities**2))
 
         temperature = (
-            (2 / 3) * kinetic_energy / (config.gas_constant * config.n_particles)  # noqa: E501
+            (2 / 3)
+            * kinetic_energy
+            / (config.gas_constant * config.n_particles)  # noqa: E501
         )
+
+        if config.pressure or config.barostat:
+            pressure = comp_pressure(
+                phi,
+                phi_q,
+                psi,
+                hamiltonian,
+                velocities,
+                config,
+                phi_fourier,
+                phi_laplacian,
+                phi_transfer,
+                positions,
+                bond_pr_,
+                angle_pr_,
+                comm=comm,
+            )
+
+            # if rank ==0 : print(pressure[9:12])
+            # print('phi_fft after pressure call: phi_fft[d=0]',phi_fft[0].value[0][0][0:2])
+        else:
+            pressure = 0.0  # 0.0 indicates not calculated. To be changed.
+
         forces_out = (
-            field_forces + bond_forces + angle_forces + dihedral_forces
+            field_forces
+            + bond_forces
+            + angle_forces
+            + dihedral_forces
             + reconstructed_forces
         )
         if charges_flag:
             forces_out += elec_forces
         store_data(
-            out_dataset, step, frame, indices, positions, velocities,
-            forces_out, config.box_size, temperature, kinetic_energy,
-            bond_energy, angle_energy, dihedral_energy, field_energy,
-            field_q_energy, config.time_step, config,
-            velocity_out=args.velocity_output, force_out=args.force_output,
-            charge_out=charges_flag, dump_per_particle=args.dump_per_particle,
+            out_dataset,
+            step,
+            frame,
+            indices,
+            positions,
+            velocities,
+            forces_out,
+            config.box_size,
+            temperature,
+            pressure,
+            kinetic_energy,
+            bond_energy,
+            angle_energy,
+            dihedral_energy,
+            field_energy,
+            field_q_energy,
+            config.time_step,
+            config,
+            velocity_out=args.velocity_output,
+            force_out=args.force_output,
+            charge_out=charges_flag,
+            dump_per_particle=args.dump_per_particle,
             comm=comm,
         )
 
     if rank == 0:
         loop_start_time = datetime.datetime.now()
         last_step_time = datetime.datetime.now()
 
@@ -463,17 +713,15 @@
                 np.mod(step, config.n_steps // 1000) == 0
                 or np.mod(step, config.n_print) == 0
             ):
                 log_step = True
             if rank == 0 and log_step and args.verbose > 1:
                 step_t = current_step_time - last_step_time
                 tot_t = current_step_time - loop_start_time
-                ns_sim = (
-                    (step + 1) * config.respa_inner * config.time_step / 1000.0
-                )
+                ns_sim = (step + 1) * config.respa_inner * config.time_step / 1000.0
 
                 seconds_per_day = 24 * 60 * 60
                 seconds_elapsed = tot_t.days * seconds_per_day
                 seconds_elapsed += tot_t.seconds
                 seconds_elapsed += 1e-6 * tot_t.microseconds
                 minutes_elapsed = seconds_elapsed / 60
                 hours_elapsed = minutes_elapsed / 60
@@ -488,140 +736,313 @@
                     f"{ns_per_day:.3f} ns/day   {hours_per_ns:.3f} hours/ns   "
                     f"{steps_per_s:.3f} steps/s"
                 )
                 Logger.rank0.log(logging.INFO, info_str)
 
         # Initial outer rRESPA velocity step
         velocities = integrate_velocity(
-            velocities, field_forces / config.mass,
+            velocities,
+            field_forces / config.mass,
             config.respa_inner * config.time_step,
         )
-        if charges_flag and config.coulombtype == "PIC_Spectral":
+
+        if charges_flag and (
+            config.coulombtype == "PIC_Spectral"
+            or config.coulombtype == "PIC_Spectral_GPE"
+        ):
             velocities = integrate_velocity(
-                velocities, elec_forces / config.mass,
+                velocities,
+                elec_forces / config.mass,
                 config.respa_inner * config.time_step,
             )
         if protein_flag:
             velocities = integrate_velocity(
-                velocities, reconstructed_forces / config.mass,
+                velocities,
+                reconstructed_forces / config.mass,
                 config.respa_inner * config.time_step,
             )
 
         # Inner rRESPA steps
         for inner in range(config.respa_inner):
             velocities = integrate_velocity(
                 velocities,
                 (bond_forces + angle_forces + dihedral_forces) / config.mass,
                 config.time_step,
             )
-            positions = integrate_position(
-                positions, velocities, config.time_step
-            )
+            positions = integrate_position(positions, velocities, config.time_step)
             positions = np.mod(positions, config.box_size[None, :])
 
             # Update fast forces
             if molecules_flag:
                 if not args.disable_bonds:
-                    bond_energy_ = compute_bond_forces(
-                        bond_forces, positions, config.box_size, bonds_2_atom1,
-                        bonds_2_atom2, bonds_2_equilibrium, bonds_2_stength,
+                    bond_energy_, bond_pr_ = compute_bond_forces(
+                        bond_forces,
+                        positions,
+                        config.box_size,
+                        bonds_2_atom1,
+                        bonds_2_atom2,
+                        bonds_2_equilibrium,
+                        bonds_2_stength,
                     )
                 if not args.disable_angle_bonds:
-                    angle_energy_ = compute_angle_forces(
-                        angle_forces, positions, config.box_size,
-                        bonds_3_atom1, bonds_3_atom2, bonds_3_atom3,
-                        bonds_3_equilibrium, bonds_3_stength,
+                    angle_energy_, angle_pr_ = compute_angle_forces(
+                        angle_forces,
+                        positions,
+                        config.box_size,
+                        bonds_3_atom1,
+                        bonds_3_atom2,
+                        bonds_3_atom3,
+                        bonds_3_equilibrium,
+                        bonds_3_stength,
                     )
                 if not args.disable_dihedrals:
-                    if (
-                        inner == config.respa_inner - 1
-                        and not args.disable_dipole
-                    ):
+                    if inner == config.respa_inner - 1 and not args.disable_dipole:
                         dipole_flag = 1
                     else:
                         dipole_flag = 0
                     dihedral_energy_ = compute_dihedral_forces(
-                        dihedral_forces, positions, dipole_positions,
-                        transfer_matrices, config.box_size, bonds_4_atom1,
-                        bonds_4_atom2, bonds_4_atom3, bonds_4_atom4,
-                        bonds_4_coeff, bonds_4_type, bonds_4_last, dipole_flag,
+                        dihedral_forces,
+                        positions,
+                        dipole_positions,
+                        transfer_matrices,
+                        config.box_size,
+                        bonds_4_atom1,
+                        bonds_4_atom2,
+                        bonds_4_atom3,
+                        bonds_4_atom4,
+                        bonds_4_coeff,
+                        bonds_4_type,
+                        bonds_4_last,
+                        dipole_flag,
                     )
 
             velocities = integrate_velocity(
                 velocities,
                 (bond_forces + angle_forces + dihedral_forces) / config.mass,
                 config.time_step,
             )
 
+        # Barostat
+        if config.barostat:
+            if config.barostat.lower() == "isotropic":
+                pm_objs, change = isotropic(
+                    pmesh,
+                    pm_objs,
+                    phi,
+                    phi_q,
+                    psi,
+                    hamiltonian,
+                    positions,
+                    velocities,
+                    config,
+                    phi_fourier,
+                    phi_laplacian,
+                    phi_transfer,
+                    bond_pr_,
+                    angle_pr_,
+                    step,
+                    prng,
+                    comm=comm,
+                )
+
+            elif config.barostat.lower() == "semiisotropic":
+                pm_objs, change = semiisotropic(
+                    pmesh,
+                    pm_objs,
+                    phi,
+                    phi_q,
+                    psi,
+                    hamiltonian,
+                    positions,
+                    velocities,
+                    config,
+                    phi_fourier,
+                    phi_laplacian,
+                    phi_transfer,
+                    bond_pr_,
+                    angle_pr_,
+                    step,
+                    prng,
+                    comm=comm,
+                )
+            pm, field_list, elec_common_list, coulomb_list = pm_objs
+            (
+                phi,
+                phi_fourier,
+                force_on_grid,
+                v_ext_fourier,
+                v_ext,
+                phi_transfer,
+                phi_laplacian,
+            ) = field_list
+
+            phi_q, phi_q_fourier, psi, elec_field = elec_common_list
+
+            if len(coulomb_list) == 2:
+                elec_field_fourier, psi_fourier = coulomb_list
+
+            elif len(coulomb_list) == 12:
+                (
+                    phi_eps,
+                    phi_eps_fourier,
+                    phi_eta,
+                    phi_eta_fourier,
+                    phi_pol,
+                    phi_pol_prev,
+                    elec_dot,
+                    elec_field_contrib,
+                    psi,
+                    Vbar_elec,
+                    Vbar_elec_fourier,
+                    force_mesh_elec,
+                    force_mesh_elec_fourier,
+                ) = coulomb_list
+
         # Update slow forces
         if not args.disable_field:
             layouts = [
-                pm.decompose(positions[types == t]) for t in range(config.n_types)  # noqa: E501
+                pm.decompose(positions[types == t])
+                for t in range(config.n_types)  # noqa: E501
             ]
             update_field(
-                phi, layouts, force_on_grid, hamiltonian, pm, positions, types,
-                config, v_ext, phi_fourier, v_ext_fourier,
+                phi,
+                phi_laplacian,
+                phi_transfer,
+                layouts,
+                force_on_grid,
+                hamiltonian,
+                pm,
+                positions,
+                types,
+                config,
+                v_ext,
+                phi_fourier,
+                v_ext_fourier,
+                config.m,
             )
             compute_field_force(
-                layouts, positions, force_on_grid, field_forces, types,
+                layouts,
+                positions,
+                force_on_grid,
+                field_forces,
+                types,
                 config.n_types,
             )
 
-            if charges_flag and config.coulombtype == "PIC_Spectral":
+            if charges_flag:
                 layout_q = pm.decompose(positions)
-                update_field_force_q(
-                    charges, phi_q, phi_q_fourier, elec_field_fourier,
-                    elec_field, elec_forces, layout_q, hamiltonian, 
-                    pm, positions, config,
-                )
-                field_q_energy = compute_field_energy_q(
-                    config, phi_q, phi_q_fourier, elec_potential, 
-                    elec_potential_fourier, 
-                    field_q_self_energy, comm=comm,
-                )
+                if config.coulombtype == "PIC_Spectral_GPE":  # dielectric_flag and
+                    Vbar_elec, phi_eps, elec_dot = update_field_force_q_GPE(
+                        conv_fun,
+                        phi,
+                        types,
+                        charges,
+                        phi_q,
+                        phi_q_fourier,
+                        phi_eps,
+                        phi_eps_fourier,
+                        phi_eta,
+                        phi_eta_fourier,
+                        phi_pol_prev,
+                        phi_pol,
+                        elec_field,
+                        elec_forces,
+                        elec_field_contrib,
+                        psi,
+                        Vbar_elec,
+                        Vbar_elec_fourier,
+                        force_mesh_elec,
+                        force_mesh_elec_fourier,
+                        hamiltonian,
+                        layout_q,
+                        layouts,
+                        pm,
+                        positions,
+                        config,
+                        comm=comm,
+                    )
+
+                    field_q_energy = compute_field_energy_q_GPE(
+                        config, phi_eps, field_q_energy, elec_dot, comm=comm
+                    )
+
+                if config.coulombtype == "PIC_Spectral":
+                    update_field_force_q(
+                        charges,
+                        phi_q,
+                        phi_q_fourier,
+                        psi,
+                        psi_fourier,
+                        elec_field_fourier,
+                        elec_field,
+                        elec_forces,
+                        layout_q,
+                        hamiltonian,
+                        pm,
+                        positions,
+                        config,
+                    )
 
             if protein_flag and not args.disable_dipole:
-                dipole_positions = np.reshape(
-                    dipole_positions, (4 * n_tors, 3)
-                )
-                dipole_forces = np.reshape(
-                    dipole_forces, (4 * n_tors, 3)
-                )
+                dipole_positions = np.reshape(dipole_positions, (4 * n_tors, 3))
+                dipole_forces = np.reshape(dipole_forces, (4 * n_tors, 3))
 
                 layout_dipoles = pm.decompose(dipole_positions)
                 update_field_force_q(
-                    dipole_charges, phi_dipoles, phi_dipoles_fourier,
-                    dipoles_field_fourier, dipoles_field, dipole_forces,
-                    layout_dipoles, hamiltonian, pm, dipole_positions, config,
+                    dipole_charges,
+                    phi_dipoles,
+                    phi_dipoles_fourier,
+                    psi_dipoles,
+                    psi_dipoles_fourier,
+                    dipoles_field_fourier,
+                    dipoles_field,
+                    dipole_forces,
+                    layout_dipoles,
+                    hamiltonian,
+                    pm,
+                    dipole_positions,
+                    config,
                 )
 
                 dipole_positions = np.reshape(dipole_positions, (n_tors, 4, 3))
                 dipole_forces = np.reshape(dipole_forces, (n_tors, 4, 3))
 
                 dipole_positions = np.asfortranarray(dipole_positions)
                 dipole_forces_redistribution(
-                    reconstructed_forces, dipole_forces, transfer_matrices,
-                    bonds_4_atom1, bonds_4_atom2, bonds_4_atom3, bonds_4_atom4,
-                    bonds_4_type, bonds_4_last,
+                    reconstructed_forces,
+                    dipole_forces,
+                    transfer_matrices,
+                    bonds_4_atom1,
+                    bonds_4_atom2,
+                    bonds_4_atom3,
+                    bonds_4_atom4,
+                    bonds_4_type,
+                    bonds_4_last,
                 )
 
         # Second rRESPA velocity step
         velocities = integrate_velocity(
-            velocities, field_forces / config.mass,
+            velocities,
+            field_forces / config.mass,
             config.respa_inner * config.time_step,
         )
 
-        if charges_flag and config.coulombtype == "PIC_Spectral":
+        if charges_flag and (
+            config.coulombtype == "PIC_Spectral"
+            or config.coulombtype == "PIC_Spectral_GPE"
+        ):
             velocities = integrate_velocity(
-                velocities, elec_forces / config.mass,
+                velocities,
+                elec_forces / config.mass,
                 config.respa_inner * config.time_step,
             )
         if protein_flag and not args.disable_dipole:
             velocities = integrate_velocity(
-                velocities, reconstructed_forces / config.mass,
+                velocities,
+                reconstructed_forces / config.mass,
                 config.respa_inner * config.time_step,
             )
 
         # Only compute and keep the molecular bond energy from the last rRESPA
         # inner step
         if molecules_flag:
             if not args.disable_bonds:
@@ -634,37 +1055,41 @@
         if config.domain_decomposition:
             if np.mod(step, config.domain_decomposition) == 0:
                 positions = np.ascontiguousarray(positions)
                 bond_forces = np.ascontiguousarray(bond_forces)
                 angle_forces = np.ascontiguousarray(angle_forces)
                 dihedral_forces = np.ascontiguousarray(dihedral_forces)
 
-                (positions,
-                velocities,
-                indices,
-                bond_forces,
-                angle_forces,
-                dihedral_forces,
-                reconstructed_forces,
-                field_forces,
-                names,
-                types,
-                *optional) = domain_decomposition(
+                (
+                    positions,
+                    velocities,
+                    indices,
+                    bond_forces,
+                    angle_forces,
+                    dihedral_forces,
+                    reconstructed_forces,
+                    field_forces,
+                    names,
+                    types,
+                    *optional,
+                ) = domain_decomposition(
                     positions,
                     pm,
                     *tuple(args_in),
                     molecules=molecules if molecules_flag else None,
                     bonds=bonds if molecules_flag else None,
                     verbose=args.verbose,
                     comm=comm,
                 )
 
                 if charges_flag:
                     charges = optional.pop(0)
                     elec_forces = optional.pop(0)
+                if dielectric_flag:
+                    dielectric_sorted = optional.pop(0)
                 if molecules_flag:
                     bonds = optional.pop(0)
                     molecules = optional.pop(0)
 
                 # rebuild args_in to point to correct arrays
                 args_in = [
                     velocities,
@@ -677,50 +1102,60 @@
                     names,
                     types,
                 ]
 
                 if charges_flag:
                     args_in.append(charges)
                     args_in.append(elec_forces)
+                if dielectric_flag:
+                    args_in.append(dielectric_sorted)
 
                 positions = np.asfortranarray(positions)
                 bond_forces = np.asfortranarray(bond_forces)
                 angle_forces = np.asfortranarray(angle_forces)
                 dihedral_forces = np.asfortranarray(dihedral_forces)
 
                 layouts = [
-                    pm.decompose(positions[types == t]) for t in range(config.n_types)  # noqa: E501
+                    pm.decompose(positions[types == t])
+                    for t in range(config.n_types)  # noqa: E501
                 ]
                 if molecules_flag:
                     bonds_prep = prepare_bonds(
-                        molecules, names, bonds, indices, config
+                        molecules, names, bonds, indices, config, topol
                     )
                     (
                         # two-particle bonds
-                        bonds_2_atom1, bonds_2_atom2, bonds_2_equilibrium,
+                        bonds_2_atom1,
+                        bonds_2_atom2,
+                        bonds_2_equilibrium,
                         bonds_2_stength,
                         # three-particle bonds
-                        bonds_3_atom1, bonds_3_atom2, bonds_3_atom3,
-                        bonds_3_equilibrium, bonds_3_stength,
+                        bonds_3_atom1,
+                        bonds_3_atom2,
+                        bonds_3_atom3,
+                        bonds_3_equilibrium,
+                        bonds_3_stength,
                         # four-particle bonds
-                        bonds_4_atom1, bonds_4_atom2, bonds_4_atom3,
-                        bonds_4_atom4, bonds_4_coeff, bonds_4_type,
+                        bonds_4_atom1,
+                        bonds_4_atom2,
+                        bonds_4_atom3,
+                        bonds_4_atom4,
+                        bonds_4_coeff,
+                        bonds_4_type,
                         bonds_4_last,
                     ) = bonds_prep
 
                     bonds_4_coeff = np.asfortranarray(bonds_4_coeff)
 
                     # Reinitialize dipoles so each rank has the right amount
                     if protein_flag and not args.disable_dipole:
                         # Each rank will have different n_tors, we don't need
                         # to domain decompose dipoles
                         n_tors = len(bonds_4_atom1)
-                        dipole_positions = np.zeros(
-                            (n_tors, 4, 3), dtype=dtype
-                        )
+                        dipole_positions = np.zeros((n_tors, 4, 3), dtype=dtype)
 
                         # 4 because we need to take into account the last angle
                         # in the molecule
                         dipole_charges = np.array(
                             [
                                 2 * [0.25, -0.25]
                                 if (bonds_4_type[i], bonds_4_last[i]) == (1, 1)
@@ -732,80 +1167,152 @@
                             dtype=dtype,
                         ).flatten()
                         dipole_forces = np.zeros_like(dipole_positions)
                         transfer_matrices = np.zeros(
                             shape=(n_tors, 6, 3, 3), dtype=dtype
                         )
                         dipole_positions = np.asfortranarray(dipole_positions)
-                        transfer_matrices = np.asfortranarray(transfer_matrices)  # noqa: E501
+                        transfer_matrices = np.asfortranarray(
+                            transfer_matrices
+                        )  # noqa: E501
 
         for t in range(config.n_types):
             if args.verbose > 2:
                 exchange_cost = layouts[t].get_exchange_cost()
                 Logger.all_ranks.log(
                     logging.INFO,
                     (
                         f"(GHOSTS: Total number of particles of type "
                         f"{config.type_to_name_map[t]} to be "
                         f"exchanged = {exchange_cost[rank]}"
                     ),
                 )
 
         # Thermostat
-        if config.target_temperature:
+        if config.target_temperature and np.mod(step, config.n_b) == 0:
             csvr_thermostat(velocities, names, config, prng, comm=comm)
 
         # Remove total linear momentum
         if config.cancel_com_momentum:
             if np.mod(step, config.cancel_com_momentum) == 0:
                 velocities = cancel_com_momentum(velocities, config, comm=comm)
 
         # Print trajectory
         if config.n_print > 0:
             if np.mod(step, config.n_print) == 0:
                 frame = step // config.n_print
                 if not args.disable_field:
+                    layouts = [
+                        pm.decompose(positions[types == t])
+                        for t in range(config.n_types)
+                    ]
+                    update_field(
+                        phi,
+                        phi_laplacian,
+                        phi_transfer,
+                        layouts,
+                        force_on_grid,
+                        hamiltonian,
+                        pm,
+                        positions,
+                        types,
+                        config,
+                        v_ext,
+                        phi_fourier,
+                        v_ext_fourier,
+                        config.m,
+                        compute_potential=True,
+                    )
                     (
-                        field_energy, kinetic_energy,
+                        field_energy,
+                        kinetic_energy,
+                        field_q_energy,
                     ) = compute_field_and_kinetic_energy(
-                        phi, velocities, hamiltonian, positions, types, v_ext,
-                        config, layouts, comm=comm,
+                        phi,
+                        phi_q,
+                        psi,
+                        velocities,
+                        hamiltonian,
+                        positions,
+                        types,
+                        v_ext,
+                        config,
+                        layouts,
+                        comm=comm,
                     )
 
-                    if charges_flag and config.coulombtype == "PIC_Spectral":
-                        field_q_energy = compute_field_energy_q(
-                            config, phi_q, phi_q_fourier, elec_potential, 
-                            elec_potential_fourier, 
-                            field_q_self_energy, comm=comm,
-                        )
+                    if charges_flag:
+                        if config.coulombtype == "PIC_Spectral_GPE":
+                            field_q_energy = compute_field_energy_q_GPE(
+                                config, phi_eps, field_q_energy, elec_dot, comm=comm
+                            )
                 else:
                     kinetic_energy = comm.allreduce(
-                        0.5 * config.mass * np.sum(velocities ** 2)
+                        0.5 * config.mass * np.sum(velocities**2)
                     )
                 temperature = (
-                    (2 / 3) * kinetic_energy
+                    (2 / 3)
+                    * kinetic_energy
                     / (config.gas_constant * config.n_particles)
                 )
                 if args.disable_field:
                     field_energy = 0.0
 
+                if config.pressure or config.barostat:
+                    pressure = comp_pressure(
+                        phi,
+                        phi_q,
+                        psi,
+                        hamiltonian,
+                        velocities,
+                        config,
+                        phi_fourier,
+                        phi_laplacian,
+                        phi_transfer,
+                        positions,
+                        bond_pr_,
+                        angle_pr_,
+                        comm=comm,
+                    )
+                else:
+                    pressure = 0.0  # 0.0 indicates not calculated. To be changed.
+
                 forces_out = (
-                    field_forces + bond_forces + angle_forces
-                    + dihedral_forces + reconstructed_forces
+                    field_forces
+                    + bond_forces
+                    + angle_forces
+                    + dihedral_forces
+                    + reconstructed_forces
                 )
                 if charges_flag:
                     forces_out += elec_forces
                 store_data(
-                    out_dataset, step, frame, indices, positions, velocities,
-                    forces_out, config.box_size, temperature, kinetic_energy,
-                    bond_energy, angle_energy, dihedral_energy, field_energy,
-                    field_q_energy, config.respa_inner * config.time_step,
-                    config, velocity_out=args.velocity_output,
-                    force_out=args.force_output, charge_out=charges_flag,
-                    dump_per_particle=args.dump_per_particle, comm=comm,
+                    out_dataset,
+                    step,
+                    frame,
+                    indices,
+                    positions,
+                    velocities,
+                    forces_out,
+                    config.box_size,
+                    temperature,
+                    pressure,
+                    kinetic_energy,
+                    bond_energy,
+                    angle_energy,
+                    dihedral_energy,
+                    field_energy,
+                    field_q_energy,
+                    config.respa_inner * config.time_step,
+                    config,
+                    velocity_out=args.velocity_output,
+                    force_out=args.force_output,
+                    charge_out=charges_flag,
+                    dump_per_particle=args.dump_per_particle,
+                    comm=comm,
                 )
                 if np.mod(step, config.n_print * config.n_flush) == 0:
                     out_dataset.flush()
         last_step_time = current_step_time
 
     # End simulation
     if rank == 0:
@@ -821,58 +1328,160 @@
                 f"MD loop time: {format_timedelta(loop_time)}"
             ),
         )
 
     if config.n_print > 0 and np.mod(config.n_steps, config.n_print) != 0:
         if not args.disable_field:
             update_field(
-                phi, layouts, force_on_grid, hamiltonian, pm, positions, types,
-                config, v_ext, phi_fourier, v_ext_fourier,
+                phi,
+                phi_laplacian,
+                phi_transfer,
+                layouts,
+                force_on_grid,
+                hamiltonian,
+                pm,
+                positions,
+                types,
+                config,
+                v_ext,
+                phi_fourier,
+                v_ext_fourier,
+                config.m,
                 compute_potential=True,
             )
-            field_energy, kinetic_energy = compute_field_and_kinetic_energy(
-                phi, velocities, hamiltonian, positions, types, v_ext, config,
-                layouts, comm=comm,
+            (
+                field_energy,
+                kinetic_energy,
+                field_q_energy,
+            ) = compute_field_and_kinetic_energy(
+                phi,
+                phi_q,
+                psi,
+                velocities,
+                hamiltonian,
+                positions,
+                types,
+                v_ext,
+                config,
+                layouts,
+                comm=comm,
             )
 
-            if charges_flag and config.coulombtype == "PIC_Spectral":
+            if charges_flag:
                 layout_q = pm.decompose(positions)
-                update_field_force_q(
-                    charges, phi_q, phi_q_fourier, elec_field_fourier,
-                    elec_field, elec_forces, layout_q, hamiltonian, pm,
-                    positions, config,
-                )
+                if config.coulombtype == "PIC_Spectral_GPE":
+                    Vbar_elec, phi_eps, elec_dot = update_field_force_q_GPE(
+                        conv_fun,
+                        phi,
+                        types,
+                        charges,
+                        phi_q,
+                        phi_q_fourier,
+                        phi_eps,
+                        phi_eps_fourier,
+                        phi_eta,
+                        phi_eta_fourier,
+                        phi_pol_prev,
+                        phi_pol,
+                        elec_field,
+                        elec_forces,
+                        elec_field_contrib,
+                        psi,
+                        Vbar_elec,
+                        Vbar_elec_fourier,
+                        force_mesh_elec,
+                        force_mesh_elec_fourier,
+                        hamiltonian,
+                        layout_q,
+                        layouts,
+                        pm,
+                        positions,
+                        config,
+                        comm=comm,
+                    )
 
-                field_q_energy = compute_field_energy_q(
-                    config, phi_q, phi_q_fourier, elec_potential, 
-                    elec_potential_fourier, 
-                    field_q_self_energy, comm=comm,
-                )
+                    field_q_energy = compute_field_energy_q_GPE(
+                        config, phi_eps, field_q_energy, elec_dot, comm=comm
+                    )
+
+                if config.coulombtype == "PIC_Spectral":
+                    update_field_force_q(
+                        charges,
+                        phi_q,
+                        phi_q_fourier,
+                        psi,
+                        psi_fourier,
+                        elec_field_fourier,
+                        elec_field,
+                        elec_forces,
+                        layout_q,
+                        hamiltonian,
+                        pm,
+                        positions,
+                        config,
+                    )
 
         else:
-            kinetic_energy = comm.allreduce(
-                0.5 * config.mass * np.sum(velocities**2)
-            )
+            kinetic_energy = comm.allreduce(0.5 * config.mass * np.sum(velocities**2))
         frame = (step + 1) // config.n_print
         temperature = (
-            (2 / 3) * kinetic_energy
-            / (config.gas_constant * config.n_particles)
+            (2 / 3) * kinetic_energy / (config.gas_constant * config.n_particles)
         )
         if args.disable_field:
             field_energy = 0.0
+
+        if config.pressure or config.barostat:
+            pressure = comp_pressure(
+                phi,
+                phi_q,
+                psi,
+                hamiltonian,
+                velocities,
+                config,
+                phi_fourier,
+                phi_laplacian,
+                phi_transfer,
+                positions,
+                bond_pr_,
+                angle_pr_,
+                Vbar_elec,
+                comm=comm,
+            )
+        else:
+            pressure = 0.0  # 0.0 indicates not calculated. To be changed.
+
         forces_out = (
-            field_forces + bond_forces + angle_forces + dihedral_forces
+            field_forces
+            + bond_forces
+            + angle_forces
+            + dihedral_forces
             + reconstructed_forces
         )
         if charges_flag:
             forces_out += elec_forces
         store_data(
-            out_dataset, step, frame, indices, positions, velocities,
-            forces_out, config.box_size, temperature, kinetic_energy,
-            bond_energy, angle_energy, dihedral_energy, field_energy,
-            field_q_energy, config.respa_inner * config.time_step, config,
-            velocity_out=args.velocity_output, force_out=args.force_output,
-            charge_out=charges_flag, dump_per_particle=args.dump_per_particle,
+            out_dataset,
+            step,
+            frame,
+            indices,
+            positions,
+            velocities,
+            forces_out,
+            config.box_size,
+            temperature,
+            pressure,
+            kinetic_energy,
+            bond_energy,
+            angle_energy,
+            dihedral_energy,
+            field_energy,
+            field_q_energy,
+            config.respa_inner * config.time_step,
+            config,
+            velocity_out=args.velocity_output,
+            force_out=args.force_output,
+            charge_out=charges_flag,
+            dump_per_particle=args.dump_per_particle,
             comm=comm,
         )
 
     out_dataset.close_file()
```

### Comparing `hymd-1.0.9/hymd/thermostat.py` & `hymd-2.0.1/hymd/thermostat.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,24 +19,23 @@
     kT_start = config.gas_constant * config.start_temperature
     n_particles_ = velocities.shape[0]
     velocities[...] = prng.normal(
         loc=0, scale=kT_start / config.mass, size=(n_particles_, 3)
     )
     velocities = cancel_com_momentum(velocities, config, comm=comm)
     kinetic_energy = comm.allreduce(
-        0.5 * config.mass * np.sum(velocities ** 2), MPI.SUM
+        0.5 * config.mass * np.sum(velocities**2), MPI.SUM
     )
     start_kinetic_energy_target = (
-        1.5 * config.gas_constant * config.n_particles
-        * config.start_temperature
+        1.5 * config.gas_constant * config.n_particles * config.start_temperature
     )
     factor = np.sqrt(1.5 * config.n_particles * kT_start / kinetic_energy)
     velocities[...] = velocities[...] * factor
     kinetic_energy = comm.allreduce(
-        0.5 * config.mass * np.sum(velocities ** 2), MPI.SUM
+        0.5 * config.mass * np.sum(velocities**2), MPI.SUM
     )
     Logger.rank0.log(
         logging.INFO,
         (
             f"Initialized {config.n_particles} velocities, target kinetic "
             f"energy: {start_kinetic_energy_target}, actual kinetic energy "
             f"generated: {kinetic_energy}"
@@ -106,19 +105,23 @@
     Computer Programming (Reading, MA: Addison-Wesley), pp. 120ff.
     J. H. Ahrens and U. Dieter, Computing 12 (1974), 223-246.
     """
     return prng.chisquare(M)
 
 
 def csvr_thermostat(
-    velocity: np.ndarray, names: np.ndarray, config: Config,
+    velocity: np.ndarray,
+    names: np.ndarray,
+    config: Config,
     prng: np.random.Generator,
     comm: MPI.Intracomm = MPI.COMM_WORLD,
     random_gaussian: Callable[[np.random.Generator], float] = _random_gaussian,
-    random_chi_squared: Callable[[np.random.Generator, int, float], float] = _random_chi_squared,
+    random_chi_squared: Callable[
+        [np.random.Generator, int, float], float
+    ] = _random_chi_squared,
     remove_center_of_mass_momentum: bool = True,
 ) -> np.ndarray:
     """Canonical sampling through velocity rescaling thermostat
 
     Implements the CSVR thermostat. Rescales the system kinetic energy by a
     stochastically chosen factor to keep the temperature constant. Requires
     communcation of the kinetic energies calculated locally for each MPI rank.
@@ -140,14 +143,16 @@
     ----------
     velocity : (N, D) numpy.ndarray
         Array of velocities of N particles in D dimensions.
     names : (N,) numpy.ndarray
         Array of particle names.
     config : Config
         Configuration dataclass containing simulation metadata and parameters.
+    prng : np.random.Generator
+        Numpy object that provides a stream of random bits
     comm : MPI.Intracomm, optional
         MPI communicator to use for rank commuication. Defaults to
         MPI.COMM_WORLD.
     random_gaussian : callable, optional
         Function for generating standard normally distributed numbers.
     random_chi_squared : callable, optional
         Function for generating :math:`\\chi^2`-distributed numbers
@@ -178,44 +183,37 @@
         )
         group_n_particles = comm.allreduce(len(ind[0]), MPI.SUM)
 
         # Clean velocities of center of mass momentum
         if remove_center_of_mass_momentum and group_n_particles > 1:
             com_velocity = comm.allreduce(np.sum(velocity[ind], axis=0))
             velocity_clean = velocity[ind] - com_velocity / group_n_particles
-            K = comm.allreduce(0.5 * config.mass
-                               * np.sum(velocity_clean[...]**2))
+            K = comm.allreduce(0.5 * config.mass * np.sum(velocity_clean[...] ** 2))
         else:
-            K = comm.allreduce(0.5 * config.mass * np.sum(velocity[...]**2))
+            K = comm.allreduce(0.5 * config.mass * np.sum(velocity[...] ** 2))
         K_target = (
-            1.5 * config.gas_constant * group_n_particles
-            * config.target_temperature
+            1.5 * config.gas_constant * group_n_particles * config.target_temperature
         )
         N_f = 3 * group_n_particles
         c = np.exp(-(config.time_step * config.respa_inner) / config.tau)
 
-        # Draw random numbers and broadcast them so they are identical across
-        # MPI ranks
-        R = SNf = None
-        if comm.Get_rank() == 0:
-            R = random_gaussian(prng)
-            SNf = random_chi_squared(prng, N_f - 1)
-        R = comm.bcast(R, root=0)
-        SNf = comm.bcast(SNf, root=0)
+        # Random numbers are identical across ranks because all ranks have
+        # the same prng after the initialization of the velocities
+        R = random_gaussian(prng)
+        SNf = random_chi_squared(prng, N_f - 1)
 
         alpha2 = (
-            c + (1 - c) * (SNf + R**2) * K_target / (N_f * K)
+            c
+            + (1 - c) * (SNf + R**2) * K_target / (N_f * K)
             + 2 * R * np.sqrt(c * (1 - c) * K_target / (N_f * K))
         )
         dK = K * (alpha2 - 1)
         alpha = np.sqrt(alpha2)
 
         if remove_center_of_mass_momentum and group_n_particles > 1:
             # Assign velocities and reapply the previously removed center
             # of mass momentum removed
             velocity_clean *= alpha
-            velocity[ind] = (
-                velocity_clean + com_velocity / group_n_particles
-            )
+            velocity[ind] = velocity_clean + com_velocity / group_n_particles
         else:
             velocity *= alpha
         config.thermostat_work += dK
```

### Comparing `hymd-1.0.9/hymd.egg-info/PKG-INFO` & `hymd-2.0.1/hymd.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hymd
-Version: 1.0.9
+Version: 2.0.1
 Summary: Massively parallel hybrid particle-field MD
 Home-page: https://github.com/Cascella-Group-UiO/HyMD
 Author: Morten Ledum
 Author-email: morten.ledum@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -12,33 +12,37 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <a href="https://cascella-group-uio.github.io/HyMD/">
   <img src="https://github.com/Cascella-Group-UiO/HyMD/blob/main/docs/img/hymd_logo_text_black.png?raw=true" width="500" title="HylleraasMD">
 </a>
 
 [![License: GPL v3](https://img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.html) ![build](https://github.com/Cascella-Group-UiO/HyMD-2021/workflows/build/badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/actions/workflows/docs_pages.yml/badge.svg)](https://cascella-group-uio.github.io/HyMD/) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/branch/main/graph/badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-Group-UiO/HyMD) [![PyPI version](https://badge.fury.io/py/hymd.svg)](https://badge.fury.io/py/hymd)
 
 ---------
-**HylleraasMD** (HyMD) is a massively parallel Python package for hybrid particle-field molecular dynamics (hPF-MD) simulations of coarse-grained bio- and soft-matter systems.
+**HylleraasMD** (HyMD) is a massively parallel Python package for Hamiltonian hybrid particle-field molecular dynamics (HhPF-MD) simulations of coarse-grained bio- and soft-matter systems.
 
-HyMD can run canonical hPF-MD simulations [[1]](#1), or filtered density Hamiltonian hPF (HhPF-MD) simulations [[2]](#2), with or without explicit PME electrostatic interactions [[3]](#3). It includes all standard intramolecular interactions, including stretching, bending, torsional, and combined bending-dihedral potentials. Additionally, topological reconstruction of permanent peptide chain backbone dipoles is possible for accurate recreation of protein conformational dynamics [[4]](#4). Martini style elastic networks (ElNeDyn) [[5]](#5) are also supported.
+HyMD can run canonical hPF-MD simulations, or filtered density Hamiltonian hPF (HhPF-MD) simulations [[1]](#1),[[2]](#2),[[3]](#3) with or without explicit PME electrostatic interactions. It includes all standard intramolecular interactions,
+including stretching, bending, torsional, and combined bending-dihedral potentials. Additionally, topological reconstruction of permanent peptide chain backbone dipoles is possible for accurate recreation of protein conformational dynamics.
+It can run simulations in constant energy (NVE), constant volume (NVT) [[1]](#1) or constant pressure (NPT) conditions [[4]](#4).
 
-HyMD uses the [pmesh](github.com/rainwoodman/pmesh) library for particle-mesh operations, with the PPFT [[6]](#6) backend for FFTs through the [pfft-python bindings](github.com/rainwoodman/pfft-python). File IO is done via HDF5 formats to allow MPI parallel reads.
+HyMD uses the [pmesh](github.com/rainwoodman/pmesh) library for particle-mesh operations, with the PPFT [[5]](#5) backend for FFTs through the [pfft-python bindings](github.com/rainwoodman/pfft-python).
+File IO is done via HDF5 formats to allow MPI parallel reads.
 
 ## User Guide
 Detailed installation and user guide, together with comprehensive example simulations are located in the [HylleraasMD documentation](https://cascella-group-uio.github.io/HyMD/index.html).
 
 Run simulations by
 ```bash
 python3 -m hymd [CONFIGURATION_FILE] [TOPOLOGY_FILE] (--OPTIONAL_ARGS)
@@ -94,27 +98,28 @@
 ```
 Running MPI enabled pytest tests is simplified with a convenient script
 ```bash
 chmod +x pytest-mpi
 pytest-mpi -oo -n 2 -ns
 ```
 
+## Please cite our work
+If you use HyMD for your purposes, please cite the appropriate references from the section below.  
+If you cannot cite all, the fundamental works to be cited are [[1]](#1) and [[4]](#4). 
+
 ---------
 
 ### References
 <a id="1">[1]</a>
-Milano, G.; Kawakatsu, T. Hybrid particle-field molecular dynamics simulations for dense polymer systems. J. Chem. Phys. **2009**, 130, 214106.
+Ledum, M.; Sen, S.; Li, X.; Carrer, M.; Feng Y.; Cascella, M.; Bore, S. L. HylleraasMD: A Domain Decomposition-Based Hybrid Particle-Field Software for Multi-Scale Simulations of Soft Matter. ChemRxiv 2021
 
 <a id="2">[2]</a>
-Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid particle–field molecular dynamics. J. Chem. Phys. **2020**, 153, 094106.
+Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L. HyMD: Massively parallel hybrid particle-field molecular dynamics in Python.
 
 <a id="3">[3]</a>
-Kolli, H. B.; De Nicola, A.; Bore, S. L.; Schäfer, K.; Diezemann, G.; Gauss, J.; Kawakatsu, T.;Lu, Z.-Y.; Zhu, Y.-L.; Milano, G.; Cascella, M. Hybrid Particle-Field Molecular DynamicsSimulations of Charged Amphiphiles in an Aqueous Environment. J. Chem. Theory Comput. **2018**, 14, 4928–4937.
+Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid particle–field molecular dynamics. J. Chem. Phys. 2020, 153, 094106.
 
 <a id="4">[4]</a>
-Bore, S. L.; Milano, G.; Cascella, M. Hybrid Particle-Field Model for Conformational Dynamics of Peptide Chains. J. Chem. Theory Comput. **2018**, 14, 1120–1130.
+Sen, S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure: Pushing Particle–Field Molecular Dynamics to the Isobaric Ensemble. ChemRxiv 2023
 
 <a id="5">[5]</a>
-Periole, X.; Cavalli, M.; Marrink, S. J.; Ceruso, M. A. Combining an elastic network with a coarse-grained molecular force field: structure, dynamics, and intermolecular recognition. J. Chem. Theory Comput. **2009**, 5.9, 2531-2543.
-
-<a id="6">[6]</a>
-Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM J. Sci. Comput. **2013**, 35, C213–C236.
+Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM J. Sci. Comput. 2013, 35, C213–C236.
```

#### html2text {}

```diff
@@ -1,49 +1,51 @@
-Metadata-Version: 2.1 Name: hymd Version: 1.0.9 Summary: Massively parallel
+Metadata-Version: 2.1 Name: hymd Version: 2.0.1 Summary: Massively parallel
 hybrid particle-field MD Home-page: https://github.com/Cascella-Group-UiO/HyMD
 Author: Morten Ledum Author-email: morten.ledum@gmail.com License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
 OSI Approved :: GNU Lesser General Public License v3 (LGPLv3) Classifier:
 Intended Audience :: Science/Research Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Fortran Classifier: Topic ::
-Scientific/Engineering :: Chemistry Classifier: Topic :: Scientific/Engineering
-:: Physics Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE.txt [https://github.com/Cascella-Group-UiO/HyMD/blob/
-main/docs/img/hymd_logo_text_black.png?raw=true] [![License: GPL v3](https://
-img.shields.io/badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/
-lgpl-3.0.html) ![build](https://github.com/Cascella-Group-UiO/HyMD-2021/
-workflows/build/badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/
-actions/workflows/docs_pages.yml/badge.svg)](https://cascella-group-
-uio.github.io/HyMD/) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/
-branch/main/graph/badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-
-Group-UiO/HyMD) [![PyPI version](https://badge.fury.io/py/hymd.svg)](https://
-badge.fury.io/py/hymd) --------- **HylleraasMD** (HyMD) is a massively parallel
-Python package for hybrid particle-field molecular dynamics (hPF-MD)
-simulations of coarse-grained bio- and soft-matter systems. HyMD can run
-canonical hPF-MD simulations [[1]](#1), or filtered density Hamiltonian hPF
-(HhPF-MD) simulations [[2]](#2), with or without explicit PME electrostatic
-interactions [[3]](#3). It includes all standard intramolecular interactions,
-including stretching, bending, torsional, and combined bending-dihedral
-potentials. Additionally, topological reconstruction of permanent peptide chain
-backbone dipoles is possible for accurate recreation of protein conformational
-dynamics [[4]](#4). Martini style elastic networks (ElNeDyn) [[5]](#5) are also
-supported. HyMD uses the [pmesh](github.com/rainwoodman/pmesh) library for
-particle-mesh operations, with the PPFT [[6]](#6) backend for FFTs through the
-[pfft-python bindings](github.com/rainwoodman/pfft-python). File IO is done via
-HDF5 formats to allow MPI parallel reads. ## User Guide Detailed installation
-and user guide, together with comprehensive example simulations are located in
-the [HylleraasMD documentation](https://cascella-group-uio.github.io/HyMD/
-index.html). Run simulations by ```bash python3 -m hymd [CONFIGURATION_FILE]
-[TOPOLOGY_FILE] (--OPTIONAL_ARGS) ``` #### Run interactively in Google
-Colaboratory A [Google Colaboratory](https://colab.research.google.com/
-) jupyter notebook is setup [here](https://colab.research.google.com/drive/
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Fortran Classifier: Topic :: Scientific/Engineering ::
+Chemistry Classifier: Topic :: Scientific/Engineering :: Physics Requires-
+Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE.txt
+[https://github.com/Cascella-Group-UiO/HyMD/blob/main/docs/img/
+hymd_logo_text_black.png?raw=true] [![License: GPL v3](https://img.shields.io/
+badge/License-LGPLv3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.html) !
+[build](https://github.com/Cascella-Group-UiO/HyMD-2021/workflows/build/
+badge.svg) [![docs](https://github.com/Cascella-Group-UiO/HyMD/actions/
+workflows/docs_pages.yml/badge.svg)](https://cascella-group-uio.github.io/HyMD/
+) [![codecov](https://codecov.io/gh/Cascella-Group-UiO/HyMD/branch/main/graph/
+badge.svg?token=BXZ7B9RXV9)](https://codecov.io/gh/Cascella-Group-UiO/HyMD) [!
+[PyPI version](https://badge.fury.io/py/hymd.svg)](https://badge.fury.io/py/
+hymd) --------- **HylleraasMD** (HyMD) is a massively parallel Python package
+for Hamiltonian hybrid particle-field molecular dynamics (HhPF-MD) simulations
+of coarse-grained bio- and soft-matter systems. HyMD can run canonical hPF-MD
+simulations, or filtered density Hamiltonian hPF (HhPF-MD) simulations [[1]]
+(#1),[[2]](#2),[[3]](#3) with or without explicit PME electrostatic
+interactions. It includes all standard intramolecular interactions, including
+stretching, bending, torsional, and combined bending-dihedral potentials.
+Additionally, topological reconstruction of permanent peptide chain backbone
+dipoles is possible for accurate recreation of protein conformational dynamics.
+It can run simulations in constant energy (NVE), constant volume (NVT) [[1]]
+(#1) or constant pressure (NPT) conditions [[4]](#4). HyMD uses the [pmesh]
+(github.com/rainwoodman/pmesh) library for particle-mesh operations, with the
+PPFT [[5]](#5) backend for FFTs through the [pfft-python bindings](github.com/
+rainwoodman/pfft-python). File IO is done via HDF5 formats to allow MPI
+parallel reads. ## User Guide Detailed installation and user guide, together
+with comprehensive example simulations are located in the [HylleraasMD
+documentation](https://cascella-group-uio.github.io/HyMD/index.html). Run
+simulations by ```bash python3 -m hymd [CONFIGURATION_FILE] [TOPOLOGY_FILE] (--
+OPTIONAL_ARGS) ``` #### Run interactively in Google Colaboratory A [Google
+Colaboratory](https://colab.research.google.com/) jupyter notebook is setup
+[here](https://colab.research.google.com/drive/
 1jfzRaXjL3q53J4U8OrCgADepmf_HuCOh?usp=sharing) with a working HyMD fully
 installed and executable in the browser. ## Installation #### Non-Python
 dependencies HyMD installation **requires** a working MPI compiler. It is
 highly recommended to have *MPI-enabled* HDF5 and [h5py](https://docs.h5py.org/
 en/stable/mpi.html) for running parallel simulations with HyMD. Install both on
 Ubuntu with ```bash sudo apt-get update -y sudo apt-get install -y pkg-config
 libhdf5-mpi-dev libopenmpi-dev python3 -m pip uninstall h5py # Remove any
@@ -63,23 +65,21 @@
 O https://raw.githubusercontent.com/Cascella-Group-UiO/HyMD-tutorial/main/
 ideal_chain/ideal_chain.HDF5 /app$ /app$ # Run simulation /app$ python3 -m hymd
 ideal_chain.toml ideal_chain.HDF5 --verbose ``` ## Run tests Clone the
 repository and run tests with [pytest](https://docs.pytest.org/en/latest)
 ```bash git clone https://github.com/Cascella-Group-UiO/HyMD.git hymd cd hymd
 python3 -m pip install pytest pytest-mpi pytest ``` Running MPI enabled pytest
 tests is simplified with a convenient script ```bash chmod +x pytest-mpi
-pytest-mpi -oo -n 2 -ns ``` --------- ### References [1] Milano, G.; Kawakatsu,
-T. Hybrid particle-field molecular dynamics simulations for dense polymer
-systems. J. Chem. Phys. **2009**, 130, 214106. [2] Bore, S. L.; Cascella, M.
-Hamiltonian and alias-free hybrid particleâfield molecular dynamics. J. Chem.
-Phys. **2020**, 153, 094106. [3] Kolli, H. B.; De Nicola, A.; Bore, S. L.;
-SchÃ¤fer, K.; Diezemann, G.; Gauss, J.; Kawakatsu, T.;Lu, Z.-Y.; Zhu, Y.-L.;
-Milano, G.; Cascella, M. Hybrid Particle-Field Molecular DynamicsSimulations of
-Charged Amphiphiles in an Aqueous Environment. J. Chem. Theory Comput.
-**2018**, 14, 4928â4937. [4] Bore, S. L.; Milano, G.; Cascella, M. Hybrid
-Particle-Field Model for Conformational Dynamics of Peptide Chains. J. Chem.
-Theory Comput. **2018**, 14, 1120â1130. [5] Periole, X.; Cavalli, M.;
-Marrink, S. J.; Ceruso, M. A. Combining an elastic network with a coarse-
-grained molecular force field: structure, dynamics, and intermolecular
-recognition. J. Chem. Theory Comput. **2009**, 5.9, 2531-2543. [6] Pippig, M.
-PFFT: An extension of FFTW to massively parallel architectures. SIAM J. Sci.
-Comput. **2013**, 35, C213âC236.
+pytest-mpi -oo -n 2 -ns ``` ## Please cite our work If you use HyMD for your
+purposes, please cite the appropriate references from the section below. If you
+cannot cite all, the fundamental works to be cited are [[1]](#1) and [[4]](#4).
+--------- ### References [1] Ledum, M.; Sen, S.; Li, X.; Carrer, M.; Feng Y.;
+Cascella, M.; Bore, S. L. HylleraasMD: A Domain Decomposition-Based Hybrid
+Particle-Field Software for Multi-Scale Simulations of Soft Matter. ChemRxiv
+2021 [2] Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L.
+HyMD: Massively parallel hybrid particle-field molecular dynamics in Python.
+[3] Bore, S. L.; Cascella, M. Hamiltonian and alias-free hybrid
+particleâfield molecular dynamics. J. Chem. Phys. 2020, 153, 094106. [4] Sen,
+S.; Ledum, M.; Bore, S. L.; Cascella, M. Soft Matter under Pressure: Pushing
+ParticleâField Molecular Dynamics to the Isobaric Ensemble. ChemRxiv 2023 [5]
+Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM
+J. Sci. Comput. 2013, 35, C213âC236.
```

### Comparing `hymd-1.0.9/hymd.egg-info/SOURCES.txt` & `hymd-2.0.1/hymd.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.py
 hymd/__init__.py
 hymd/__main__.py
+hymd/barostat.py
+hymd/barostat_scr.py
 hymd/compute_angle_forces.f90
 hymd/compute_angle_forces__double.f90
 hymd/compute_bond_forces.f90
 hymd/compute_bond_forces__double.f90
 hymd/compute_dihedral_forces.f90
 hymd/compute_dihedral_forces__double.f90
 hymd/configure_runtime.py
@@ -18,14 +20,15 @@
 hymd/force.py
 hymd/gaussian_core.py
 hymd/hamiltonian.py
 hymd/input_parser.py
 hymd/integrator.py
 hymd/logger.py
 hymd/main.py
+hymd/pressure.py
 hymd/thermostat.py
 hymd/version.py
 hymd.egg-info/PKG-INFO
 hymd.egg-info/SOURCES.txt
 hymd.egg-info/dependency_links.txt
 hymd.egg-info/requires.txt
 hymd.egg-info/top_level.txt
```

### Comparing `hymd-1.0.9/setup.py` & `hymd-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,24 +39,24 @@
     long_description_content_type="text/markdown",
     license="LGPLv3",
     packages=["hymd"],
     version=find_version("hymd/version.py"),
     ext_modules=[force_kernels],
     setup_requires=[
         "cython",
-        "numpy",
+        "numpy<1.24",
         "mpi4py",
     ],
     install_requires=[
         "cython",
         "h5py",
         "mpi4py",
         "mpsort",
         "networkx",
-        "numpy",
+        "numpy<1.24",
         "pfft-python",
         "pmesh",
         "sympy",
         "tomli",
     ],
     python_requires=">=3.6",
     classifiers=[
@@ -66,12 +66,13 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Fortran",
         "Topic :: Scientific/Engineering :: Chemistry",
         "Topic :: Scientific/Engineering :: Physics",
     ],
 )
```

### Comparing `hymd-1.0.9/test/test_configure_runtime.py` & `hymd-2.0.1/test/test_configure_runtime.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,58 +11,58 @@
                            change_tmp_dir, caplog):
     caplog.set_level(logging.ERROR)
     comm = MPI.COMM_WORLD
     config_toml_file, _ = config_toml
 
     basearg = [config_toml_file, h5py_molecules_file]
 
-    parsed, config, prng = configure_runtime(basearg, comm)
+    parsed, config, prng, topol = configure_runtime(basearg, comm)
     assert isinstance(parsed, Namespace)
     assert isinstance(config, Config)
     assert isinstance(prng, np.random.Generator)
     assert parsed.destdir == "."
     assert parsed.logfile == "sim.log"
 
-    parsed, _, _ = configure_runtime(["-v", "2"]+basearg, comm)
+    parsed, _, _, _ = configure_runtime(["-v", "2"]+basearg, comm)
     assert parsed.verbose == 2
 
-    parsed, _, _ = configure_runtime(["--disable-field"]+basearg, comm)
+    parsed, _, _, _ = configure_runtime(["--disable-field"]+basearg, comm)
     assert parsed.disable_field
 
-    parsed, _, _ = configure_runtime(["--disable-bonds"]+basearg, comm)
+    parsed, _, _, _ = configure_runtime(["--disable-bonds"]+basearg, comm)
     assert parsed.disable_bonds
 
-    parsed, _, _ = configure_runtime(["--disable-angle-bonds"]+basearg, comm)
+    parsed, _, _, _ = configure_runtime(["--disable-angle-bonds"]+basearg, comm)
     assert parsed.disable_angle_bonds
 
-    parsed, _, _ = configure_runtime(["--disable-dihedrals"]+basearg, comm)
+    parsed, _, _, _ = configure_runtime(["--disable-dihedrals"]+basearg, comm)
     assert parsed.disable_dihedrals
 
-    parsed, _, _ = configure_runtime(["--disable-dipole"]+basearg, comm)
+    parsed, _, _, _ = configure_runtime(["--disable-dipole"]+basearg, comm)
     assert parsed.disable_dipole
 
-    parsed, _, _ = configure_runtime(["--double-precision"]+basearg, comm)
+    parsed, _, _, _ = configure_runtime(["--double-precision"]+basearg, comm)
     assert parsed.double_precision
 
-    parsed, _, _ = configure_runtime(["--double-output"]+basearg, comm)
+    parsed, _, _, _ = configure_runtime(["--double-output"]+basearg, comm)
     assert parsed.double_output
 
-    parsed, _, _ = configure_runtime(["--dump-per-particle"]+basearg, comm)
+    parsed, _, _, _ = configure_runtime(["--dump-per-particle"]+basearg, comm)
     assert parsed.dump_per_particle
 
-    parsed, _, _ = configure_runtime(["--force-output"]+basearg, comm)
+    parsed, _, _, _ = configure_runtime(["--force-output"]+basearg, comm)
     assert parsed.force_output
 
-    parsed, _, _ = configure_runtime(["--velocity-output"]+basearg, comm)
+    parsed, _, _, _ = configure_runtime(["--velocity-output"]+basearg, comm)
     assert parsed.velocity_output
 
-    parsed, _, _ = configure_runtime(["--disable-mpio"]+basearg, comm)
+    parsed, _, _, _ = configure_runtime(["--disable-mpio"]+basearg, comm)
     assert parsed.disable_mpio
 
-    parsed, _, _ = configure_runtime(["--destdir", "testdir"]+basearg, comm)
+    parsed, _, _, _ = configure_runtime(["--destdir", "testdir"]+basearg, comm)
     assert parsed.destdir == "testdir"
 
-    parsed, _, _ = configure_runtime(["--seed", "54321"]+basearg, comm)
+    parsed, _, _, _ = configure_runtime(["--seed", "54321"]+basearg, comm)
     assert parsed.seed == 54321
 
-    parsed, _, _ = configure_runtime(["--logfile", "test.log"]+basearg, comm)
+    parsed, _, _, _ = configure_runtime(["--logfile", "test.log"]+basearg, comm)
     assert parsed.logfile == "test.log"
```

### Comparing `hymd-1.0.9/test/test_distribute_input.py` & `hymd-2.0.1/test/test_distribute_input.py`

 * *Files identical despite different names*

### Comparing `hymd-1.0.9/test/test_field.py` & `hymd-2.0.1/test/test_field.py`

 * *Files identical despite different names*

### Comparing `hymd-1.0.9/test/test_file_io.py` & `hymd-2.0.1/test/test_file_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import h5py
 from hymd.file_io import (
     OutDataset, setup_time_dependent_element, store_static, store_data,
     distribute_input
 )
 from hymd.input_parser import Config, parse_config_toml, _setup_type_to_name_map
 from hymd.force import prepare_bonds
+from hymd.barostat import Target_pressure
 
 def test_OutDataset(config_toml, tmp_path):
     _, config_toml_str = config_toml
     config = parse_config_toml(config_toml_str)
 
     out = OutDataset(tmp_path, config)
     assert hasattr(out, "config")
@@ -57,19 +58,20 @@
         (config.n_particles, 3),
         "float32",
         units="nm"
     )
 
     assert isinstance(group, h5py.Group)
     assert group.name == "/test/position"
-    assert group.attrs["units"] == "nm"
 
     assert isinstance(step, h5py.Dataset)
     assert isinstance(time, h5py.Dataset)
+    assert time.attrs["unit"] == "ps"
     assert isinstance(value, h5py.Dataset)
+    assert value.attrs["unit"] == "nm"
 
     out.close_file()
 
 
 @pytest.mark.mpi()
 def test_distribute_input():
     # create fake indices and molecules
@@ -104,15 +106,16 @@
 
 @pytest.mark.mpi()
 def test_store_static(molecules_with_solvent, tmp_path):
     indices, positions, molecules, velocities, bonds, names, types = molecules_with_solvent
     box_size = np.array([10, 10, 10], dtype=np.float64)
     config = Config(n_steps=0, n_print=1, time_step=0.03, box_size=box_size,
                     mesh_size=[5, 5, 5], sigma=0.5, kappa=0.05,
-                    n_particles=len(indices))
+                    n_particles=len(indices), 
+                    target_pressure=Target_pressure(P_L=None,P_N=None))
     Bond = collections.namedtuple(
         "Bond", ["atom_1", "atom_2", "equilibrium", "strength"]
     )
     cbonds = (
         Bond("A", "A", 0.27, 10000),
         Bond("A", "B", 0.27, 10000),
         Bond("A", "C", 0.27, 10000),
@@ -181,15 +184,16 @@
 
 @pytest.mark.mpi()
 def test_store_data(molecules_with_solvent, tmp_path):
     indices, positions, molecules, velocities, bonds, names, types = molecules_with_solvent
     box_size = np.array([10, 10, 10], dtype=np.float64)
     config = Config(n_steps=100, n_print=1, time_step=0.03, box_size=box_size,
                     mesh_size=[5, 5, 5], sigma=0.5, kappa=0.05,
-                    n_particles=len(indices), mass=72.)
+                    n_particles=len(indices), mass=72.,
+                    target_pressure=Target_pressure(P_L=None,P_N=None))
     Bond = collections.namedtuple(
         "Bond", ["atom_1", "atom_2", "equilibrium", "strength"]
     )
     cbonds = (
         Bond("A", "A", 0.27, 10000),
         Bond("A", "B", 0.27, 10000),
         Bond("A", "C", 0.27, 10000),
@@ -241,15 +245,15 @@
         bonds_2_atom2, molecules=molecules_
     )
 
     forces = np.copy(positions_)
 
     store_data(
         out, 0, 0, indices_, positions_, velocities_, forces,
-        box_size, 300., 1., 2., 3., 4., 5., 6., 0.02, config
+        box_size, 300., 1., 1., 2., 3., 4., 5., 6., 0.02, config
     )
 
     outdataset_step = [
         out.positions_step,
         out.total_energy_step,
         out.potential_energy_step,
         out.kinetc_energy_step,
@@ -288,13 +292,14 @@
     for dset in outdataset_time:
         assert isinstance(dset, h5py.Dataset)
         assert dset[0] == 0
 
     assert out.potential_energy[0] == pytest.approx(20.)
     assert out.kinetc_energy[0] == pytest.approx(1.)
     assert out.temperature[0] == pytest.approx(300.)
+    assert out.pressure[0] == pytest.approx(1.)
     assert out.bond_energy[0] == pytest.approx(2.)
     assert out.angle_energy[0] == pytest.approx(3.)
     assert out.dihedral_energy[0] == pytest.approx(4.)
     assert out.field_energy[0] == pytest.approx(5.)
 
     out.close_file()
```

### Comparing `hymd-1.0.9/test/test_force.py` & `hymd-2.0.1/test/test_force.py`

 * *Files identical despite different names*

### Comparing `hymd-1.0.9/test/test_hamiltonian.py` & `hymd-2.0.1/test/test_hamiltonian.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     indices, _, names, _, r, _ = dppc_single
     conf_file_name, _ = config_toml
     file_contents = read_config_toml(conf_file_name)
     config = parse_config_toml(file_contents)
 
     config = _find_unique_names(config, names)
     config.sigma = sigma
+    config.type_charges = [0.] * config.n_types
+
     W = DefaultNoChi(config)
 
     k_ = np.array(
         [[0.5321315378106508, -0.6711591309063634,  0.8362051282174443],
          [0.2853046917286570, -0.6542962742862817,  0.3174805390299977],
          [0.6999748102259762, -0.9385345654631219, -0.7383831543700541]]
     )
@@ -78,14 +80,15 @@
          [5.5405900785250210, 6.5585020954226065, 1.3155113935992528],
          [1.6400925628903045, 2.1325438112867725, 3.4149968975443680]]
     )
     types = np.array([0, 0, 1, 1, 1], dtype=int)
     names = np.array([np.string_(x) for x in ["A", "A", "B", "B", "B"]])
     n_types = len(np.unique(types))
     config_conf = _find_unique_names(config_conf, names)
+    config_conf.type_charges = [0.] * config_conf.n_types
 
     W = DefaultNoChi(config_conf)
 
     mesh_size = config_conf.mesh_size
     pm = pmesh.ParticleMesh(
         mesh_size, BoxSize=config_conf.box_size, dtype='f8',
         comm=MPI.COMM_WORLD
@@ -177,14 +180,15 @@
         time_step=0.01,
         n_steps=1,
         sigma=sigma,
         kappa=kappa,
     )
     names = np.array([np.string_(s) for s in ['A', 'A']])
     config = _find_unique_names(config, names)
+    config.type_charges = [0.] * config.n_types
     r = np.array(
         [[1.50, 0.75, 2.25],
          [2.25, 0.00, 3.00],
          [4.50, 1.50, 2.25]]
     )
     pm = pmesh.ParticleMesh(
         config.mesh_size, BoxSize=config.box_size, dtype="f8",
@@ -278,14 +282,16 @@
 
     names = np.array([np.string_(s) for s in ['A', 'A', 'B', 'C', 'C']])
     types = np.array([0, 0, 1, 2, 2])
     config = _find_unique_names(config, names)
     config.box_size = np.array([15.0, 15.0, 15.0])
     config.mesh_size = np.array([160, 160, 160])
     config.n_particles = 5
+    config.type_charges = [0.] * config.n_types
+
     r = np.array(
         [[1.50, 0.75, 2.25],
          [2.25, 0.00, 3.00],
          [4.50, 1.50, 2.25],
          [1.50, 1.50, 0.75],
          [3.00, 4.50, 1.50]]
     )
@@ -362,14 +368,16 @@
 
 def test_get_hamiltonian(config_toml):
     _, config_toml_str = config_toml
     config = parse_config_toml(config_toml_str)
     config.unique_names = ["N","P","G","C","W"]
     config.type_to_name_map = {0: 'N', 1: 'P', 2: 'G', 3: 'C', 4: 'W'}
     config.n_types = 5
+    config.type_charges = [0., 0., 0., 0., 0.]
+
 
     config.hamiltonian = "DefaultNoChi"
     hamiltonian = get_hamiltonian(config)
     assert isinstance(hamiltonian, DefaultNoChi)
 
     config.hamiltonian = "DefaultWithChi"
     hamiltonian = get_hamiltonian(config)
```

### Comparing `hymd-1.0.9/test/test_input_parser.py` & `hymd-2.0.1/test/test_input_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,21 +359,31 @@
     config = parse_config_toml(config_toml_str)
     assert np.allclose(np.array([2.1598, 11.2498, 5.1009]), config.box_size, atol=1e-4)  # noqa: E501
 
     changed_box_toml_str = _change_in_config(
         config_toml_str, "box_size = [", "box_size = [2.25, -3.91, 4.11]"
     )
     config = parse_config_toml(changed_box_toml_str)
+    input_box = np.array([2.25, -3.91, 4.11])
 
     with pytest.raises(ValueError) as recorded_error:
-        _ = check_box_size(config)
+        _ = check_box_size(config, input_box)
         log = caplog.text
         assert all([(s in log) for s in ("Invalid", "box")])
     message = str(recorded_error.value)
     assert all([(s in message) for s in ("Invalid", "box")])
+
+    input_box = np.ones(3)
+    with pytest.raises(ValueError) as recorded_error:
+        _ = check_box_size(config, input_box)
+        log = caplog.text
+        assert all([(s in log) for s in ("Box", "not", "match")])
+    message = str(recorded_error.value)
+    assert all([(s in message) for s in ("Box", "not", "match")])
+
     caplog.clear()
 
 
 def test_input_parser_check_integrator(config_toml, caplog):
     caplog.set_level(logging.INFO)
     _, config_toml_str = config_toml
     config = parse_config_toml(config_toml_str)
@@ -745,24 +755,28 @@
     assert "sim" in config.name
 
 
 def test_input_parser_check_config(config_toml, dppc_single):
     _, config_toml_str = config_toml
     config = parse_config_toml(config_toml_str)
     config.n_particles = 13
+    charges = np.zeros(config.n_particles, dtype=np.float32)
+    input_box = np.array(config.box_size)
+    config.n_b = 1
+    config.barostat_type = "berendsen"
 
     indices, _, names, _, _, _ = dppc_single
 
     indices = np.append(indices, [12])
     names = np.append(names, [b"W"])
     names_to_types = {"N":0, "P": 1, "G": 2, "C": 3, "W": 4}
     types = np.array([names_to_types[n.decode('UTF-8')] for n in names],
                      dtype=int)
 
-    config = check_config(config, indices, names, types)
+    config = check_config(config, indices, names, types, charges, input_box)
     assert isinstance(config, Config)
 
 
 def test_input_parser_check_hamiltonian(config_toml, caplog):
     caplog.set_level(logging.INFO)
     _, config_toml_str = config_toml
     config = parse_config_toml(config_toml_str)
@@ -836,16 +850,21 @@
     assert hasattr(config, "type_to_name_map")
     assert isinstance(config.type_to_name_map, dict)
     assert all([(v in config.type_to_name_map.keys()) 
                  for v in names_to_types.values()])
 
 
 @pytest.mark.mpi()
-def test_input_parser_check_charges(caplog):
+def test_input_parser_check_charges(config_toml, caplog):
     caplog.set_level(logging.WARNING)
+    _, config_toml_str = config_toml
+    config = parse_config_toml(config_toml_str)
+    config.coulombtype = "PIC_Spectral"
+    config.dielectric_const = 80.
+
     charges = np.array(
         [1.0, 0.0, 0.5, 0.2, -0.3, 0.0, 0.3, 0.0, -0.5, 0.0, -0.5, 0.99, -0.2,
         0.3, 0.5, 0.0, 0.0, -0.3, 0.0, 0.0, -0.99, -1.0],
         dtype=float
     )
     # split charges across ranks
     comm = MPI.COMM_WORLD
@@ -856,23 +875,24 @@
     ind_rank = {}
     for i in range(size):
         ind_rank[i] = i * n_charges
     ind_rank[size] = size * n_charges + np.mod(charges.shape[0], size)
 
     rank_charges = charges[ind_rank[rank]:ind_rank[rank+1]]
 
-    check_charges(rank_charges, comm=comm) # warnings are not expected
+    newconf = check_charges(config, rank_charges, comm=comm) # warnings are not expected
     assert len(caplog.text) == 0
+    assert newconf.self_energy != 0. # TODO: compare to the right value
 
     # change charges to generate a warning
     charges[1] = 1000.
     rank_charges = charges[ind_rank[rank]:ind_rank[rank+1]]
 
     with pytest.warns(Warning) as recorded_warning:
-        config = check_charges(rank_charges)
+        newconf = check_charges(config, rank_charges)
         # only rank 0 gives the warning
         if rank == 0:
             message = recorded_warning[0].message.args[0]
             log = caplog.text
             cmp_strings = ("Charges in the input file do not sum to zero.", 
                            "Total charge is ")
             assert all([(s in message) for s in cmp_strings])
```

### Comparing `hymd-1.0.9/test/test_integrator.py` & `hymd-2.0.1/test/test_integrator.py`

 * *Files identical despite different names*

### Comparing `hymd-1.0.9/test/test_logger.py` & `hymd-2.0.1/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `hymd-1.0.9/test/test_thermostat.py` & `hymd-2.0.1/test/test_thermostat.py`

 * *Files identical despite different names*

