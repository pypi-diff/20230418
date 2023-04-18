# Comparing `tmp/pyiron-atomistics-0.2.8.tar.gz` & `tmp/pyiron-atomistics-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron-atomistics-0.2.8.tar", last modified: Thu Mar 18 18:53:18 2021, max compression
+gzip compressed data, was "pyiron-atomistics-0.2.9.tar", last modified: Mon Mar 22 13:30:45 2021, max compression
```

## Comparing `pyiron-atomistics-0.2.8.tar` & `pyiron-atomistics-0.2.9.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.732010 pyiron-atomistics-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      933 2021-03-18 18:53:18.732010 pyiron-atomistics-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5773 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.732010 pyiron-atomistics-0.2.8/pyiron_atomistics/
--rw-r--r--   0 runner    (1001) docker     (121)     3285 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2021-03-18 18:53:18.732010 pyiron-atomistics-0.2.8/pyiron_atomistics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.712010 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.712010 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/generic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2436 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/generic/object_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.712010 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/job/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32123 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/job/atomistic.py
--rw-r--r--   0 runner    (1001) docker     (121)    21935 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     3380 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/job/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     7749 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/job/potentials.py
--rw-r--r--   0 runner    (1001) docker     (121)    10837 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/job/sqs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6046 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/job/structurecontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.716010 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/convergence_volume.py
--rw-r--r--   0 runner    (1001) docker     (121)    22931 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/elastic.py
--rw-r--r--   0 runner    (1001) docker     (121)    28767 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/murnaghan.py
--rw-r--r--   0 runner    (1001) docker     (121)     6823 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)    18408 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (121)     6233 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/quasi.py
--rw-r--r--   0 runner    (1001) docker     (121)     5131 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/serial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1898 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/sqsmaster.py
--rw-r--r--   0 runner    (1001) docker     (121)     7416 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.716010 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32530 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/_visualize.py
--rw-r--r--   0 runner    (1001) docker     (121)    11003 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/analyse.py
--rw-r--r--   0 runner    (1001) docker     (121)     5249 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/atom.py
--rw-r--r--   0 runner    (1001) docker     (121)   126343 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/atoms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.716010 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/factories/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3903 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/factories/aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/factories/ase.py
--rw-r--r--   0 runner    (1001) docker     (121)    13586 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)    42984 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (121)    15375 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/periodic_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/pyironase.py
--rw-r--r--   0 runner    (1001) docker     (121)     8528 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/pyscal.py
--rw-r--r--   0 runner    (1001) docker     (121)    18221 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/sparse_list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.716010 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/thermodynamics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/thermodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12234 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.716010 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/volumetric/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/volumetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16570 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/volumetric/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.716010 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.716010 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/job/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18069 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/job/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.716010 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/master/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3133 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/master/convergence_encut_parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/master/convergence_encut_serial.py
--rw-r--r--   0 runner    (1001) docker     (121)     3372 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/master/murnaghan_dft.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.716010 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/waves/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/waves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10658 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/waves/bandstructure.py
--rw-r--r--   0 runner    (1001) docker     (121)    12121 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/waves/dos.py
--rw-r--r--   0 runner    (1001) docker     (121)    29289 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/dft/waves/electronic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.724010 pyiron-atomistics-0.2.8/pyiron_atomistics/gpaw/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/gpaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5083 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/gpaw/gpaw.py
--rw-r--r--   0 runner    (1001) docker     (121)    18327 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/gpaw/pyiron_ase.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.724010 pyiron-atomistics-0.2.8/pyiron_atomistics/interactive/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6686 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/interactive/activation_relaxation_technique.py
--rw-r--r--   0 runner    (1001) docker     (121)    11723 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/interactive/scipy_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)    15264 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/interactive/sxextoptint.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.724010 pyiron-atomistics-0.2.8/pyiron_atomistics/lammps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/lammps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    52747 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/lammps/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    42436 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/lammps/control.py
--rw-r--r--   0 runner    (1001) docker     (121)    26001 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/lammps/interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/lammps/lammps.py
--rw-r--r--   0 runner    (1001) docker     (121)    10635 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/lammps/potential.py
--rw-r--r--   0 runner    (1001) docker     (121)    22815 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/lammps/structure.py
--rw-r--r--   0 runner    (1001) docker     (121)    25329 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.724010 pyiron-atomistics-0.2.8/pyiron_atomistics/sphinx/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    96057 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/sphinx/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    16251 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/sphinx/interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)     3480 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/sphinx/potential.py
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/sphinx/sphinx.py
--rw-r--r--   0 runner    (1001) docker     (121)     3794 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/sphinx/structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     5885 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/sphinx/volumetric_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.728010 pyiron-atomistics-0.2.8/pyiron_atomistics/table/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4119 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/table/datamining.py
--rw-r--r--   0 runner    (1001) docker     (121)     9045 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/table/funct.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.728010 pyiron-atomistics-0.2.8/pyiron_atomistics/testing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6854 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/testing/executable.py
--rw-r--r--   0 runner    (1001) docker     (121)    16911 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/testing/randomatomistic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.728010 pyiron-atomistics-0.2.8/pyiron_atomistics/thermodynamics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/thermodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8641 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/thermodynamics/hessian.py
--rw-r--r--   0 runner    (1001) docker     (121)    49541 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/thermodynamics/interfacemethod.py
--rw-r--r--   0 runner    (1001) docker     (121)    18446 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/thermodynamics/sxphonons.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.732010 pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    97442 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    14804 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)    13087 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/metadyn.py
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/oszicar.py
--rw-r--r--   0 runner    (1001) docker     (121)    36265 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/outcar.py
--rw-r--r--   0 runner    (1001) docker     (121)    18519 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/potential.py
--rw-r--r--   0 runner    (1001) docker     (121)     3899 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/procar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1607 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/report.py
--rw-r--r--   0 runner    (1001) docker     (121)    15337 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     2399 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (121)    33024 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/vasprun.py
--rw-r--r--   0 runner    (1001) docker     (121)      880 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/vaspsol.py
--rw-r--r--   0 runner    (1001) docker     (121)    12462 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/volumetric_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-18 18:53:18.712010 pyiron-atomistics-0.2.8/pyiron_atomistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      933 2021-03-18 18:53:18.000000 pyiron-atomistics-0.2.8/pyiron_atomistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4588 2021-03-18 18:53:18.000000 pyiron-atomistics-0.2.8/pyiron_atomistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-18 18:53:18.000000 pyiron-atomistics-0.2.8/pyiron_atomistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-03-18 18:53:18.000000 pyiron-atomistics-0.2.8/pyiron_atomistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-03-18 18:53:18.000000 pyiron-atomistics-0.2.8/pyiron_atomistics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      201 2021-03-18 18:53:18.732010 pyiron-atomistics-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2021-03-18 18:53:18.000000 pyiron-atomistics-0.2.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2021-03-18 18:53:15.000000 pyiron-atomistics-0.2.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1593 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      933 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5773 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/pyiron_atomistics/
+-rw-r--r--   0 runner    (1001) docker     (121)     3285 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/pyiron_atomistics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.487854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.487854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/generic/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2436 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/generic/object_type.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.487854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32123 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/atomistic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21935 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3380 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7749 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/potentials.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10845 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6058 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/structurecontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.487854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1765 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/convergence_volume.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22931 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28767 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/murnaghan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6823 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18408 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6233 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/quasi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5131 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/serial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1898 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/sqsmaster.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7416 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32530 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11003 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5249 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/atom.py
+-rw-r--r--   0 runner    (1001) docker     (121)   126343 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factories/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3903 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factories/aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2094 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factories/ase.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13586 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42984 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15375 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/periodic_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2023 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2461 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/pyironase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8528 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18221 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/sparse_list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/thermodynamics/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/thermodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12234 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/volumetric/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/volumetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16570 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/volumetric/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/job/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18069 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/job/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3133 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/convergence_encut_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2003 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/convergence_encut_serial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3372 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2246 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/murnaghan_dft.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10607 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/bandstructure.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12121 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/dos.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29289 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/electronic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/gpaw/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/gpaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5083 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/gpaw/gpaw.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18327 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/gpaw/pyiron_ase.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6694 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/activation_relaxation_technique.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11731 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/scipy_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15264 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/sxextoptint.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.491854 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52747 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42436 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/control.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26001 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1462 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10635 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/potential.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22815 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25329 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/project.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    96079 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16251 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3480 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/potential.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1484 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3794 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5885 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/volumetric_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/pyiron_atomistics/table/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4119 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/table/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9045 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/table/funct.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/pyiron_atomistics/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6854 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/testing/executable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16911 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/testing/randomatomistic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8641 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49541 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/interfacemethod.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18446 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/sxphonons.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    97442 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14804 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13087 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/metadyn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1375 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/oszicar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36265 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/outcar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18519 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/potential.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3899 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/procar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1607 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/report.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15337 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2399 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33024 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/vasprun.py
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/vaspsol.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12462 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/volumetric_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-22 13:30:45.487854 pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      933 2021-03-22 13:30:45.000000 pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4588 2021-03-22 13:30:45.000000 pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-22 13:30:45.000000 pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2021-03-22 13:30:45.000000 pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-03-22 13:30:45.000000 pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2021-03-22 13:30:45.495854 pyiron-atomistics-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1825 2021-03-22 13:30:44.000000 pyiron-atomistics-0.2.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68611 2021-03-22 13:30:41.000000 pyiron-atomistics-0.2.9/versioneer.py
```

### Comparing `pyiron-atomistics-0.2.8/LICENSE` & `pyiron-atomistics-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/PKG-INFO` & `pyiron-atomistics-0.2.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyiron-atomistics
-Version: 0.2.8
+Version: 0.2.9
 Summary: pyiron - an integrated development environment (IDE) for computational materials science.
 Home-page: https://github.com/pyiron/pyiron_atomistics
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Description: http://pyiron.org
 Keywords: pyiron
```

### Comparing `pyiron-atomistics-0.2.8/README.rst` & `pyiron-atomistics-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/__init__.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/generic/object_type.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/generic/object_type.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/job/atomistic.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/atomistic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/job/interactive.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/job/interactivewrapper.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/interactivewrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/job/potentials.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/potentials.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/job/sqs.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/sqs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 from multiprocessing import cpu_count
 from pyiron_atomistics.atomistics.job.atomistic import AtomisticGenericJob
-from pyiron_base import InputList, GenericParameters, Settings, ImportAlarm
+from pyiron_base import DataContainer, GenericParameters, Settings, ImportAlarm
 from pyiron_atomistics.atomistics.structure.atoms import Atoms, ase_to_pyiron, pyiron_to_ase
 from pymatgen.io.ase import AseAtomsAdaptor
 import numpy as np
 
 try:
     from sqsgenerator.core.sqs import ParallelSqsIterator
     import_alarm = ImportAlarm()
@@ -123,15 +123,15 @@
         }
     }
 
     @import_alarm
     def __init__(self, project, job_name):
         super(SQSJob, self).__init__(project, job_name)
         # self.input = InputList(table_name='input')
-        self.input = InputList(table_name='custom_dict')
+        self.input = DataContainer(table_name='custom_dict')
         self.input.mole_fractions = dict()
         self.input.weights = None
         self.input.objective = 0.0
         self.input.iterations = 1e6
         self.input.n_output_structures = 1
         self._python_only_job = True
         self._lst_of_struct = []
```

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/job/structurecontainer.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/job/structurecontainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 )
 __version__ = "0.1"
 __maintainer__ = "Marvin Poul"
 __email__ = "poul@mpie.de"
 __status__ = "development"
 __date__ = "Aug 12, 2020"
 
-from pyiron_base import InputList, GenericJob
+from pyiron_base import DataContainer, GenericJob
 from pyiron_atomistics.atomistics.job.atomistic import AtomisticGenericJob
 from pyiron_atomistics.atomistics.structure.atoms import Atoms
 
 
 class StructureContainer(AtomisticGenericJob):
     """
     Container to save a list of structures in HDF5 together with tags.
@@ -26,21 +26,21 @@
     :attr:`.structure_lst`.  The HDF5 is written when :meth:`.run` is called.
     """
 
     def __init__(self, project, job_name):
         super().__init__(project, job_name)
         self.__version__ = "0.2.0"
         self.__hdf_version__ = "0.2.0"
-        self._structure_lst = InputList(table_name = "structures")
+        self._structure_lst = DataContainer(table_name = "structures")
         self.server.run_mode.interactive = True
 
     @property
     def structure_lst(self):
         """
-        :class:`.InputList`: list of :class:`~.Atoms`
+        :class:`.DataContainer`: list of :class:`~.Atoms`
         """
         return self._structure_lst
 
     @staticmethod
     def _to_structure(structure_or_job):
         """
         Return structure from structure or atomic job.
```

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/convergence_volume.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/convergence_volume.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/elastic.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/elastic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/murnaghan.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/murnaghan.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/parallel.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/phonopy.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/phonopy.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/quasi.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/quasi.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/serial.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/serial.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/sqsmaster.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/sqsmaster.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/master/structure.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/master/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/_visualize.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/_visualize.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/analyse.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/analyse.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/atom.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/atom.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/atoms.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/atoms.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/factories/aimsgb.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factories/aimsgb.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/factories/ase.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factories/ase.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/factory.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/neighbors.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/neighbors.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/periodic_table.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/periodic_table.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/phonopy.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/phonopy.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/pyironase.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/pyironase.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/pyscal.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/pyscal.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/structure/sparse_list.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/structure/sparse_list.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/atomistics/volumetric/generic.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/atomistics/volumetric/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/dft/job/generic.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/job/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/dft/master/convergence_encut_parallel.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/convergence_encut_parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/dft/master/convergence_encut_serial.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/convergence_encut_serial.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/dft/master/murnaghan_dft.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/master/murnaghan_dft.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/dft/waves/bandstructure.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/bandstructure.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 """
 This module is supposed to be common for both electronic and phonon band structures
 """
 from __future__ import print_function
 import numpy as np
 from numpy import transpose as tr
 from numpy.linalg import inv, norm
-from pyiron_base import PyironObject
 
 __author__ = "Joerg Neugebauer, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -40,15 +39,15 @@
         for i, sp in enumerate(self.special_points):
             if i < len(self.special_points) - 1:
                 x1 = np.array(self.special_points[i + 1])
                 x2 = np.array(sp)
                 spl_distances.append(np.linalg.norm(x2 - x1))
 
 
-class Bandstructure(PyironObject):
+class Bandstructure:
     translate_to_pylab = {"Gamma": r"$\Gamma$", "G'": r"$\Gamma^\prime$"}
 
     def __init__(self, structure=None, prec=1e-5):
         self.prec = prec
         self._structure = None
         self.bmat = None
         self.point_group = None
```

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/dft/waves/dos.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/dos.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/dft/waves/electronic.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/dft/waves/electronic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/gpaw/gpaw.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/gpaw/gpaw.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/gpaw/pyiron_ase.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/gpaw/pyiron_ase.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/interactive/activation_relaxation_technique.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/activation_relaxation_technique.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
 from pyiron_atomistics.atomistics.job.interactivewrapper import InteractiveWrapper, ReferenceJobOutput
-from pyiron_base import InputList, Settings
+from pyiron_base import DataContainer, Settings
 
 __author__ = "Osamu Waseda"
 __copyright__ = "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH " \
                 "- Computational Materials Design (CM) Department"
 __version__ = "1.0"
 __maintainer__ = "Osamu Waseda"
 __email__ = "waseda@mpie.de"
@@ -101,15 +101,15 @@
         >>> some_minimizer.run()
 
 
     """
     def __init__(self, project, job_name):
         super(ART, self).__init__(project, job_name)
         self.__name__ = "ART"
-        self.input = InputList(table_name='custom_dict')
+        self.input = DataContainer(table_name='custom_dict')
         self.input.gamma = 0.1
         self.input.fix_layer = False
         self.input.non_art_id = None
         self.input.art_id = None
         self.input.direction = None
         self.output = ARTIntOutput(job=self)
         self.server.run_mode.interactive = True
```

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/interactive/scipy_minimizer.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/scipy_minimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import numpy as np
 from pyiron_atomistics.atomistics.job.interactivewrapper import InteractiveWrapper
-from pyiron_base import InputList
+from pyiron_base import DataContainer
 from pyiron_atomistics.atomistics.job.interactive import GenericInteractiveOutput
 from scipy.optimize import minimize
 import scipy
 import warnings
 
 __author__ = "Osamu Waseda"
 __copyright__ = (
@@ -268,15 +268,15 @@
         self.input.pressure = pressure
         self.input.volume_only = volume_only
         self.input.ionic_force_tolerance = ionic_force_tolerance
         self.input.ionic_energy_tolerance = ionic_energy_tolerance
         self.input.pressure_tolerance = pressure_tolerance
 
 
-class Input(InputList):
+class Input(DataContainer):
     """
     Args:
         minimizer (str): minimizer to use (currently only 'CG' and 'BFGS' run
             reliably)
         ionic_steps (int): max number of steps
         ionic_force_tolerance (float): maximum force tolerance
     """
```

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/interactive/sxextoptint.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/interactive/sxextoptint.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/lammps/base.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/base.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/lammps/control.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/control.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/lammps/interactive.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/lammps/lammps.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/lammps.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/lammps/potential.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/lammps/structure.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/lammps/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/project.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/project.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/sphinx/base.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     find_potential_file as find_potential_file_vasp, \
     VaspPotentialSetter
 from pyiron_atomistics.sphinx.structure import read_atoms
 from pyiron_atomistics.sphinx.potential import SphinxJTHPotentialFile
 from pyiron_atomistics.sphinx.potential import find_potential_file \
     as find_potential_file_jth
 from pyiron_atomistics.sphinx.volumetric_data import SphinxVolumetricData
-from pyiron_base import Settings, InputList, job_status_successful_lst, deprecate
+from pyiron_base import Settings, DataContainer, job_status_successful_lst, deprecate
 
 __author__ = "Osamu Waseda, Jan Janssen"
 __copyright__ = (
     "Copyright 2021, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -417,27 +417,27 @@
         self.input.sphinx.pawPot = Group({"species": []})
         for species_obj in self.structure.get_species_objects():
             if species_obj.Parent is not None:
                 elem = species_obj.Parent
             else:
                 elem = species_obj.Abbreviation
             if potformat == "JTH":
-                self.input.sphinx.pawPot["species"].append({
+                self.input.sphinx.pawPot["species"].append(Group({
                             "name": '"' + elem + '"',
                             "potType": '"AtomPAW"',
                             "element": '"' + elem + '"',
                             "potential": f'"{elem}_GGA.atomicdata"',
-                })
+                }))
             elif potformat == "VASP":
-                self.input.sphinx.pawPot["species"].append({
+                self.input.sphinx.pawPot["species"].append(Group({
                             "name": '"' + elem + '"',
                             "potType": '"VASP"',
                             "element": '"' + elem + '"',
                             "potential": '"' + elem + "_POTCAR" + '"',
-                })
+                }))
             else:
                 raise ValueError('Potential must be JTH or VASP')
         if not check_overlap:
             self.input.sphinx.pawPot["species"][-1]["checkOverlap"] = "false"
         if self.input["KJxc"]:
             self.input.sphinx.pawPot["kjxc"] = True
 
@@ -1805,15 +1805,15 @@
                 file_name = posixpath.join(cwd, file_name)
             with open(file_name, "w") as f:
                 f.write(spins_str)
         else:
             s.logger.debug("No magnetic moments")
 
 
-class Group(InputList):
+class Group(DataContainer):
     """
     Dictionary-like object to store SPHInX inputs.
 
     Attributes (sub-groups, parameters, & flags) can be set
     and accessed via dot notation, or as standard dictionary
     key/values.
```

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/sphinx/interactive.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/sphinx/potential.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/sphinx/sphinx.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/sphinx.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/sphinx/structure.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/sphinx/volumetric_data.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/sphinx/volumetric_data.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/table/datamining.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/table/datamining.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/table/funct.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/table/funct.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/testing/executable.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/testing/executable.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/testing/randomatomistic.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/testing/randomatomistic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/thermodynamics/hessian.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/hessian.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/thermodynamics/interfacemethod.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/interfacemethod.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/thermodynamics/sxphonons.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/thermodynamics/sxphonons.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/base.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/base.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/interactive.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/metadyn.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/metadyn.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/oszicar.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/oszicar.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/outcar.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/outcar.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/potential.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/procar.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/procar.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/report.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/report.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/structure.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/vasp.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/vasprun.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/vasprun.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/vaspsol.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/vaspsol.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics/vasp/volumetric_data.py` & `pyiron-atomistics-0.2.9/pyiron_atomistics/vasp/volumetric_data.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics.egg-info/PKG-INFO` & `pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyiron-atomistics
-Version: 0.2.8
+Version: 0.2.9
 Summary: pyiron - an integrated development environment (IDE) for computational materials science.
 Home-page: https://github.com/pyiron/pyiron_atomistics
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Description: http://pyiron.org
 Keywords: pyiron
```

### Comparing `pyiron-atomistics-0.2.8/pyiron_atomistics.egg-info/SOURCES.txt` & `pyiron-atomistics-0.2.9/pyiron_atomistics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.2.8/setup.py` & `pyiron-atomistics-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,20 +31,20 @@
     install_requires=[
         'aimsgb>=0.1.0',
         'ase>=3.21.1',
         'defusedxml>=0.7.1',
         'future>=0.18.2',
         'h5py>=3.1.0',
         'matplotlib>=3.3.4',
-        'mendeleev>=0.6.1',
+        'mendeleev>=0.7.0',
         'numpy>=1.20.1',
         'pandas>=1.2.3',
         'phonopy>=2.9.3',
-        'pyiron_base>=0.2.4',
-        'pymatgen>=2022.0.4',
+        'pyiron_base>=0.2.7',
+        'pymatgen>=2022.0.5',
         'scipy>=1.6.1',
         'seekpath>=2.0.1',
         'six>=1.15.0',
         'scikit-learn>=0.24.1',
         'spglib>=1.16.1',
         'tables>=3.6.1'
     ],
```

### Comparing `pyiron-atomistics-0.2.8/versioneer.py` & `pyiron-atomistics-0.2.9/versioneer.py`

 * *Files identical despite different names*

